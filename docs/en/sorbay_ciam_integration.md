# Integration of a sorbay_ciam service

This guide will show you how to integrate your service into sorbay_ciam using our demo ui application.

Let's assume that your domain name is "example.com" and you have already created a service with the name "my-ciam-service".

## Configure the sorbay_ciam service

Navigate to the "Settings" of your service, then go to the "Pages" tab.

Configure the "Page Locations" section as follows:

<img style="width: 100%; border: 1px; border-style: solid; border-color: lightgray" src="../img/services_pages_locations.png">

Now scroll down, until you reach the "CORS" and "Custom" sections. Enter the values according to the following illustration.

<img style="width: 100%; border: 1px; border-style: solid; border-color: lightgray" src="../img/services_pages_cors_custom.png">

## Run the Docker Demo UI

You can test the sorbay_ciam service with our [pre-built demo ui container](https://quay.io/usp/sorbay-ciam-self-service-demo:1.0.0-demo-ref-ui).

In order to run the container, it must be configured as follows:

* Define the name for the container `<container-name>`
* Define the environment variable for the host name for the web server `<your-service>.<your-domain>`
* Define the environment variable for the API URI `<your-domain>`
* Map the container port to the host `<host-port>`
* Mount the server certificate for SSL into the container `<absolute-path-to-certificate>`
* Mount the server private key for SSL into the container `<absolute-path-to-private-key>`
* Specify the image version `<version>`

To run the container use the following command:

```bash
docker run --rm --name <container-name> -e HOST_NAME="<your-service>.<your-domain>" -e API_URI="<your-domain>" -p <host-port>:8443 -v <absolute-path-to-certificate>:/etc/nginx/certs/ssl.crt -v <absolute-path-to-private-key>:/etc/nginx/certs/ssl.key quay.io/usp/sorbay-ciam-self-service-demo:<version>
```

This is a concrete example according to the settings above. Ensure you provide the server certificate and private key for the demo application.

```bash
docker run --rm --name sorbay_ciam_demo -e HOST_NAME="customer-app.my-ciam-service.example.org" -v /location/to/my-ciam-service.key:/etc/nginx/certs/ssl.key -v /location/to/my-ciam-service.crt:/etc/nginx/certs/ssl.crt -e API_URI="https://my-ciam-service.example.org" -p 4200:8443 quay.io/usp/sorbay-ciam-self-service-demo:1.0.0-demo-ref-ui
```