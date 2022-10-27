# IDLight Service

## Functionality

The IDLight Service provides user management with authentication and 
self-service capabilities for the End Users. The overall strategy is a 
"Bring your own UI" so you may use the provided API from 
IDLight to integrate the capabilities in your app.

### Authentication

It provides the means to authenticate users, including two-factor
authentication with the Google Authenticator app (iOS and Android).

### Self-Service

The IDlight service includes self-service functionality that allows
your users to manage their account and profile themselves, such as
changing the password, changing user attributes or enabling
two-factor authentication.

## Configuration

To configure an instance of the IDlight service, click the "Service settings"
option in the popup menu of an entry in the services list:

<img style="margin-left: 80px; width: 35%; border: 1px; border-style: solid; border-color: lightgray" src="../img/services_service_details_popup.png">

You will then be presented with the settings of that instance of the IDlight service.
Its functionality is grouped in 4 tabs:

* General - general settings for this IDlight service instance
* Users - user-related configuration settings
* Pages - custom UI URL configuration
* Accounts - management of service user accounts

### General

#### Open service UI

At the top, you find the button "Open interfaces" which will open a new
browser window with the URL of this instance of the IDlight service. What 
you see here exactly may vary if you configure custom UI URLs in the "Pages"
section.

#### Service name

In the "Base" section, you can change the name of the service. Save your change
by clicking the "Save" button in the lower right corner.

#### Delete service

Under "Service deletion", you can delete this service instance entirely. 
*NOTE:* This change cannot be undone! It will irrevocably delete the service
and all related data and resources.

Delete the service by clicking the "Delete service" button, and then confirm
the deletion in the following pop-up dialog.

### Users

Under the "Users" tab, you find various sections where you can configure 
several aspects related to the authentication and data storage of service users.

#### Authentication

Set the required minimum length for the password by adjusting the
slider to the desired value.

Enable the checkbox to enforce a check that prevents passwords that
are equal to the username.

#### Two Factor

By enabling the "Enforce two factor authentication" checkbox in this
section, users will be forced to enable two-factor authentication.

#### Schema

Here you will be able to adapt the data schema for storing user accounts.

_This functionality is not yet available during the beta testing phase!_

### Pages

Following the "Bring your own UI" philosophy, the IDlight service allows you
to configure custom frontend URLs here. This could be custom-written 
JavaScript frontends that integrate with the service API.

* "Login URL" - Login application URL
* "Registration URL" - Registration application URL
* "Verification URL" - Verification application URL
* "Recovery URL" - Recovery application URL
* "Settings URL" - Settings application URL
* "Error URL" - Error application URL

#### Redirects 

* "Default URL" - 
* "Login URL" - Login redirect URL
* "Registration URL" - Registration redirect URL
* "Settings URL" - Settings redirect URL
* "Verification URL" - Verification redirect URL
* "Logout URL" - Logout redirect URL

#### CORS

Add any custom allowed origin URLs in this section by clicking
the "+ Allowed Origin URL" button. Click the "Save" button in the
lower right corner to save the new URL.

#### Custom

Finally you may set a custom domain name, and define a custom 
domain for the session cookie, depending on your application's requirements.

### Accounts

Under this tab, you can manage user accounts for users of the service.

#### Create user

To create a new service user, click the "+ Create user" button:

<img style="margin-left: 80px; width: 25%; border: 1px; border-style: solid; border-color: lightgray" src="../img/services_accounts_create_user_button.png">

This will open the following popup dialog where you can enter the 
details of the new user account:

<img style="margin-left: 80px; width: 75%; border: 1px; border-style: solid; border-color: lightgray" src="../img/services_accounts_create_user_popup.png">

Chose the status for the new user account ("active" or "inactive") and then 
create the new account by clicking the "Create user" button.

#### User list

Once you have created one or more service users, they will be listed 
under the "Accounts" tab:

<img style="margin-left: 80px; width: 75%; border: 1px; border-style: solid; border-color: lightgray" src="../img/services_accounts_user_list.png">

#### Edit user

To edit a user account, click the <img src="../img/button_open_details.png" /> symbol, or the "Open user" option in the popup menu:

<img style="margin-left: 80px; width: 35%; border: 1px; border-style: solid; border-color: lightgray" src="../img/services_accounts_open_user_popup.png">

#### Delete user

To delete a user account, click the "Delete user" option in the popup menu:

<img style="margin-left: 80px; width: 35%; border: 1px; border-style: solid; border-color: lightgray" src="../img/services_accounts_open_user_popup.png">

