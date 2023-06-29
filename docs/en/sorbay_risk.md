# sorbay_risk

## Functionality

The sorbay_risk service provides calculation of a risk score as a basis
to e.g. selectively omit a second factor during user authentication.
The risk score calculation is based on various information from the
client accumulated over logins, including:

- IP and derived info (like country and ASN)
- User-Agent and derived info (like browser and OS)
- Browser fingerprint

The calculated risk score is simply a number, between 0 for
practically no risk and 1 (or occasionally larger) for maximal risk.

- If the risk score is low (typ. below 0.4), most likely a user that had
already logged in successfully in the past with second factor is now
logging in again, and the second factor could be omitted for more
user convenience and still more security
(thanks to the additional factors already evaluated in the background).
- Alternatively or additionally, if a risk score was relatively high,
your login service might notify the user of a
"login from a new location", e.g. via email or SMS.

## Configuration

To configure an instance of the sorbay_risk service, click the "Service settings"
option in the popup menu of an entry in the services list:

<img style="margin-left: 80px; width: 35%; border: 1px; border-style: solid; border-color: lightgray" src="../img/services_service_details_popup.png">

You will then be presented with the settings of that instance of the sorbay_risk service.
Its functionality is grouped in the following tabs:

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

#### API-Keys

In the section "API Keys" one or more API-keys can be defined.
You need at least one to use the service, more precisely for the REST APIs of the service.
The GUI proposes an API-key (a random UUID), but you can change that as desired.
