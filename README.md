# Demo theme for Plutus

This theme is a starting point for building your theme for Plutus.  Please note that
Plutus uses Smarty for parsing templates and rendering the results to the web browser.
Generally the demo theme is way out of date and is in the progress of being brought
up to date again.

| URL                         | Template                  | Notes                                                                             |
| --------------------------- | ------------------------- | --------------------------------------------------------------------------------- |
| non existant urls           | 404.tpl                   | File not found page                                                               |
| /accounts                   | accounts.tpl              | User dashboard that shows their accounts                                          |
| /accounts/UUID/statements   | account__statements.tpl   | Shows the user the links for downloadable statements.                             |
| /accounts/UUID/transactions | account__transactions.tpl | Shows the transactions that have occurred on an account.                          |
| /howtodeposit               | howtodeposit.tpl          | How to deposit instructions                                                       |
| /login                      | login.tpl                 | Login Page -- shown to users before they login                                    |
| /prepaid/airtime            | prepaid__airtime.tpl      | Prepaid Airtime page -- used to show networks and vouchers available for purchase |
| /prepaid/electricity        | prepaid__electricity.tpl  | Prepaid Electricity page -- used for starting the purchase of prepaid electricity |
| /settings                   | settings.tpl              | Change your password page.                                                        |
| /settings/autoload          | settings__autoload.tpl    | Configures the users autoload settings.                                           |
| /settings/tfa               | settings__tfa.tpl         | Two Factor Authentication settings                                                |
| /sms                        | sms.tpl                   | SMS Sending page                                                                  |
| /transfer                   | transfer.tpl              | Interaccount transfer                                                             |
| /transfer                   | transfer__otp.tpl         | Template that is used when an OTP is requested to complete the transfer.          |

## Common Templates

A number of templates are symlinked in from ../../common and live are available from
https://github.com/jacques/common-smarty-templates

To clone the common template repo from the command line:

```
git clone https://github.com/jacques/common-smarty-templates.git
```

| Template                        | Notes                                                                              |
| ------------------------------- | ---------------------------------------------------------------------------------- |
| _partials/header-bsfa.tpl       | Includes Bootstrap 3.3.7 and Font Awesome 4.7.0 Stylesheets                        |
| _partials/header-csrf.tpl       | Used for jquery-rails-ui to have the CSRF token for POST, PUT and DELETE requests. |
| _partials/header-shims.tpl      | Includes HTML5 Shim and Respond.js for IE8                                         |
| _partials/footer-datepicker.tpl | Includes Bootstrap Datepicker javascript                                           |
| _partials/footer-jqbs.tpl       | Includes Bootstrap 3.3.7 and jQuery 2.1.4 javascript                               |

## Quick Start Guide

Including another template:

```
{include file="header.tpl" nav="home"}
```


```
{include file="footer.tpl"}
```

## License

The Demo Theme for Plutus is licensed under the [MPL v.2.0](LICENSE).
These templates are distributed under the License is distributed
on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND,
either express or implied. See the License for the specific language
governing permissions and limitations under the License.
