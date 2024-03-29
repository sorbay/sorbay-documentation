# sorbay_risk
## Configuration

To configure an instance of the sorbay_risk service, click the "Service settings"
option in the popup menu of an entry in the services list:

<img style="margin-left: 80px; width: 35%; border: 1px; border-style: solid; border-color: lightgray" src="../img/services_service_details_popup.png">

You will then be presented with the settings of that instance of the sorbay_risk service.
Its functionality is grouped into the following tabs:

* General - general settings for this service instance
* Configuration - configuration of this service instance

### General

#### Service name

In the section "Base Settings" you can change the name of the service.
Save your change by clicking the "Save" button in the lower right corner.

#### Delete service

Under "Service deletion", you can delete this service instance entirely.
*NOTE:* This change cannot be undone! It will irrevocably delete the service
and all related data and resources.

Delete the service by clicking the "Delete service" button,
and then confirm the deletion in the following pop-up dialog.

### Configuration

#### API Keys

To access the REST API of the service an API key is required.
You must define or generate at least one for proper functionality.

It's possible to define more than one API key so that you can rotate them regularly.

#### CORS

Only JavaScript served by the login service should be allowed to call the risk service,
which is achieved via standard Cross-Origin Resource Sharing (CORS) headers
that are automatically sent by web browsers.

Define the allowed origin URL(s) of the login service,
i.e. the URL(s) at the login service that are allowed
to serve JavaScript that then calls the risk service.
