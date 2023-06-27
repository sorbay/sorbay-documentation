# sorbay_risk

## Functionality

The sorbay_risk service provides calculation of a risk score as a basis
to selectively omit a second factor during user authentication.
The risk score calculation is based on various information from the
client, including:

* IP and derived info (like country and ASN)
* User-Agent and derived info (like browser and OS versions)
* Browser fingerprint

The calculated risk score is simply a number, between 0 for
practically no risk and 1 (or occasionally more) for maximal risk.
If the risk score is low (typ. below 0.4), most likely a user that had
already logged in successfully in the past with second factor is now
logging in again, and the second factor could be omitted for more
user convenience and still good security (additional factors already
evaluated in the background).
Alternatively or additionally, if a risk score was relatively high,
an email with subject e.g. "login from a new location" could be sent
to the user.

## Configuration

To configure an instance of the sorbay_risk service, click the "Service settings"
option in the popup menu of an entry in the services list:

<img style="margin-left: 80px; width: 35%; border: 1px; border-style: solid; border-color: lightgray" src="../img/services_service_details_popup.png">

You will then be presented with the settings of that instance of the sorbay_risk service.
Its functionality is grouped in **TODO** tabs:

* Tab1 - tab1 info
* Tab2 - tab2 info

### Tab1

#### Tab1/setting1

**TODO**

#### Tab1/setting2

**TODO**

### Tab2

**TODO**
