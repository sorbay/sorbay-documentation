# sorbay_risk

**for secure authentication with highest user comfort**

## Functionality
sorbay_risk combines the highest level of security with the highest level
of user comfort and enables companies to reduce the friction of repeated
multiple authentications for customers, employees and partners to a necessary
minimum (Zero Friction).

### Why sorbay_risk?
sorbay_risk is an innovative cloud-based risk scoring service that
calculates the risk of whether a user is who he claims to be. The sorbay_risk
service provides the calculation of a risk score as a basis for e.g. selectively
omitting a second factor during user authentication. By implementing sorbay_risk,
organizations can not only minimize the risk of unauthorized access, but also
comply with regulatory requirements. This leads to an improved user experience
and engagement by ensuring a secure and optimized digital interaction.

<img style="margin-left: 5px; border: 0px;" src="../img/sorbay_risk_flow_diagramm_en.jpg">

With sorbay_risk, a login service can dynamically select the optimal
authentication mechanism. The login service used, such as the
USP Secure Entry Server, can take various measures based on this evaluation.
If the risk is low, e.g. if the device and location are known, access
can be granted without additional effort and without querying a second
factor. sorbay_risk thus forms the solid basis for risk-based authentication (RBA).

### How does it work?

sorbay_risk uses various contextual data from past user logins as well
as the current login attempt. Using risk-based authenticators and self-learning
risk engines, sorbay_risk calculates a trust score. By evaluating the risk score,
sorbay_risk assesses the security of the correct user identity.

The calculated risk score puts out a number between 0 for virtually no risk
and infinity for maximum risk. The organization decides how to handle the
output value, by creating rules in the used login service. One possible scenario
could be:

* If the risk score is low (typically below 0.4), it is most likely that
the user who has successfully logged in with the second factor in the
past is now logging in again, and the second factor could be omitted for
greater user convenience and even greater security (thanks to the additional
factors already evaluated in the background). 
* For a high risk score your login service could notify the user of a "login
from a new client" by email or SMS in addition of asking for the second factor.


### Use Cases

#### Use Case 1: Improve the user experience with existing 2FA
Some organizations are still reluctant to use 2FA because it dramatically 
degrades the user experience. Suddenly, users must enter a second factor 
every time they log in. This creates friction.

However, constant second-factor authentication is tedious, time-consuming
and negatively impacts the customer experience as well as employee productivity.
Each time a user logs in, they must enter their username, password and second
factor - often on a second device. This often involves waiting for the second
factor to arrive. Depending on the application - VPN applications, for 
example - re-authentication is required every time the connection is lost.
Employees spend an average of 25 hours per year entering passwords and other factors.

With sorbay_risk, the user experience is greatly improved and streamlined while
maintaining the same level of security - so-called zero friction. sorbay_risk enables
companies to drastically reduce this friction to a necessary minimum for their
customers, employees and partners. Adaptive authentication, also known as risk-based
authentication (RBA) or context-based authentication, assesses the risk associated 
with each authentication request.

#### Use Case 2: On top security for 2FA
If the organization uses or wants to use 2FA, and also wants both factors to be
checked for each access, the Risk Service can help to increase security by informing
the user about suspicious activities via the login service (e.g. MFA Prompt Bombing).

#### Use Case 3: Improve security with 1 factor in use
The customer currently uses only one factor (username-password) for logins. This is not
considered secure. However, if the organizations do not want to enforce second factor,
the Risk Score can help to detect credential stuffing or password spraying attacks.
In addition, sorbay_risk notifies the login service if anomalies has been detected
(unusual location, unusual device, etc.).

### The benefits of sorbay_risk:
**Enhanced user experience:** users find adaptive authentication far easier to use than
two-factor authentication and just as secure. Create a secure and smooth digital experience
for your users.

**Zero Trust Security:** sorbay_risk adapts to the ever-changing threat landscape and provides robust protection.

**Regulatory compliance:** Meet regulatory requirements and minimize the risk of unauthorized access.

**Flexible customization:** Set individual risk levels for applications and data to minimize friction.

**Fraud prevention:** Tailor your login service authentication preventing fraud, account takeover,
and MFA prompt bombing.

**Competitive advantage:** The ability to balance security and convenience is a clear competitive
advantage. With sorbay_risk, you achieve just that. With our Risk Score service, you'll be one step
ahead and effectively protect your business. 
