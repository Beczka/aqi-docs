---
title: Technical application
page-toc:
  active: true
---

> **Follow our step-by-step instruction guide to fill out your technical application for your live account.**

! Please note that this section does not cover any contractual parts of your live account application. Make sure you've been in touch with a [sales contact](/contact-us) for all non-technical contractual topics

Aqount is a powerful system that on the one hand can be considered a predefined product, but on the other hand is highly configurable to meet customers' needs. To do so, additional information is needed to set up and configure your live account.

To make your technical onboarding process as easy as possible, we have created a [technical application form (EXCEL file)](./technical-application-form.xlsx) to be filled out and send to us. Please [download the form](./technical-application-form.xlsx) and follow the step-by-step instruction guide below to compile all relevant information. Once you complete the form, you can send us your EXCEL document via email to `aqount@arvato.com`.

## Step-by-step instruction guide

The following instructions will be help you to fill out the technical application. Please download the [application template (EXCEL file)](./technical-application-form.xlsx) to start.

### Step 1: Define business codes

!!! The following information refers to the sheet `Step 1 - Business codes` of the [application template (EXCEL file)](./technical-application-form.xlsx).

[Aquont's month-end report concept is based on business codes](/getting-started/application/business-codes) which are defined as a tuple represented by the combination of a country and a currency (e.g. `DE/EUR`, `FR/EUR`, `UK/GBP`, etc.). Given that business codes are fundamental to Aqount, most of the configuration details must therefore be specified per business code.

Therefore the first step is to specify the complete list of business codes relevant for your business. All of the following steps will need to be defined or provided per business code.

---

### Step 2: Provide general information per business code

!!! The following information refers to the sheet `Step 2 - General data` of the [application template (EXCEL file)](./technical-application-form.xlsx).

!! **TODO**: Content migration to be reviewed by Hauke / Complete additional notes per field.

Once the list of business codes has been defined, the following general information will need to be provided per business code.

| Field | Additional notes |
|-------|------------------|
| Company legal name | Will be used as part of the name for the business code |
| Fiscal year | Start date of the legal entity's fiscal year |
| Shipping destination | List of countries |
| Invoicing countries | Needed in order to know in which countries an invoice is issued and for tax-setup.
| Expected Go-Live date | - |
| Number range orderID | - |
| Number range invoice number | - |
| Number range customer account number | - |
| Number range contract number | - |
| Number range goodwill number | - |

The following information is required to define number rangers by business codes.

| Field | Additional notes |
|-------|------------------|
| Amount for write offs to define booking rules | - |
| Migration from previous system | YES/NO |
| Write-off date of non-withdrawable credits | - |
| Write-off date of claims not to be brought in | - |

---

### Step 3: Define payment methods

!!! The following information refers to the sheet `Step 3 - Payment` of the [application template (EXCEL file)](./technical-application-form.xlsx).

The payment setup includes the connection to your PSPs/Aquirer and the setup in Aqount. As part of the setup procedure, you will have to select from the [list of payment methods](./payment-methods) per business code that you want to offer to your shoppers.

---

### Step 4: Provide bank account information

!!! The following information refers to the sheet `Step 4 - Bank setup` of the [application template (EXCEL file)](./technical-application-form.xlsx).

For every business code, a dedicated bank account needs to be specified. Once the contract is signed, the information will be used to get access to these accounts to receive the bank statements.

Relevant bank setup information is supposed to be:

| Field | Additional notes |
|-------|------------------|
| Risk service provider | - |
| Return debit fee | - |
| Chargeback handling | - |
| Paynext integration in frontend | - |
| Name of bank | - |
| Account number | - |
| IBAN | - |
| BIC | - |
| Country of bank | - |
| EBIC setup | We need the information in order to be able to instruct a (technical) EBICS user to pick up account statements / deliver payment files to the bank |
| Bank contact | - |

---

### Step 5: Define communication handling

!!! The following information refers to the sheet `Step 5 - Communication` of the [application template (EXCEL file)](./technical-application-form.xlsx).

!! **TODO**: Add standard forms for communication and mention that adaptations are possible

Part of Aqount's service provision is to (optionally) take over the communication to your customers in case of invoices and payment reminder/dunning notifications. In case these service options shall be enabled, additional information will be need.

#### Invoice process

Aqount allows to manage your entire invoice process from sending out the invoices to the follow-up. Depending on your needs we can take care over invoice queries and we also offer to take over the full credit risk. We pay up to 100% of the invoice amount depending on credit, invoice amount, invoice volume and your end customer's creditworthiness.

#### Dunning-process

If you want Aqount to send out dunning notifications, these have to be set up in our system. Our standard dunning escalation process looks as follows:

- **Level 1:** Payment reminder (14 days over due) via Email
- **Level 2:** First dunning notification (14 days after payment reminder) via Email
- **Level 3:** Second dunning notification (14 days after first dunning notification) via letter
- **Level 4:** Collecting agency

In addition, we can define if the communication shall only be send out if the amount reaches a certain level (e.g. 5 EUR)

In case of the dunning process being taken over over by Aqount, the following information will be needed:

| Field | Additional notes |
|-------|------------------|
| Email address sender | - |
| Minimum value for dunning | - |
| Dunning fee | - |
| Collection agency | - |
| Minimum value for hand over to collection agency | - |
| Supported languages | - |
| Address | - |
| Postal code | - |
| City | - |
| Country | - |
| General phone number | - |
| Official email address | - |
| VAT-ID | - |
| Managing directors | - |
| Website URL of the company | - |

#### Booking confirmation

If Aqount takes over your booking confirmations, you will be informed on the following events and actions:

* As soon as an incoming payment on a claim from an end customer has been received and booked
* In case of bookings of returns or goodwill letters
* In case of payments to the end customer

---

### Step 6: Enable back interfaces

!!! The following information refers to the sheet `Step 6 - Notifications` of the [application template (EXCEL file)](./technical-application-form.xlsx).

!! **TODO:** To be reviewed with Hauke. Assumption: Qualified response should not be part of the list as it is mandatory and therefore not configurable. More detailed information about each back interface should be move to the accounting section (most probably to the section "Notifications")

Aqount offers the possibility to send notification upon on certain system events. The following back interfaces are available and can be enabled with each one handling a certain type of notification.

| Back interface | Mandatory | Additional notes |
|----------------|-----------|------------------|
| setBalance | No | - |
| setPaymentInformation | No | - |
| setChargeBackInformation | No | - |
| setReminderLevel | No | - |
| setVerificationStatus | No | - |
| setDocumentLink | No | - |

---

### Step 7: Configure month-end reporting

!!! The following information refers to the sheet `Step 7 - Month-end-reporting` of the [application template (EXCEL file)](./technical-application-form.xlsx).

The following configuration options are available when it comes to the configuration of your month-end reporting.

#### Format options

Your month-end report can be provided to you based on the following format:

| Format | Additional notes |
|-------|------------------|
| CSV | - |
| XML | - |
| iDoc-interface | - |
| GL-interface | - |

#### Transfer options:

Your month-end report can be transfered to you based on one of the following options:

| Tranfer options | Additional notes |
|-----------------|------------------|
| Via EMail | Directly from the transaction or manually. You will need to provide the email address or list of email addresses to which the month-end report should be sent. |
| Via SFTP upload | You need to provide information on sFTP-connection for the upload of month-end reports |

#### Account number mapping

You can either select the standard GL account numbering within Aqount or define alternative GL account numbers - GL account master data - for each business code.

If the second case applies, you need to provide alternative account numbers. You can provide these information via Email or sFTP. If Email, please download the list of accounts to provide the mapped account numbers.

---

### Step 8: Configure access to the accounting user interface

!!! The following information refers to the sheet `Step 8 - MyAccount user` of the [application template (EXCEL file)](./technical-application-form.xlsx).

Aqount provides a user interface as part of its accounting component to be used by the client's accounting department when searching for specific information. In case you would like to provide access to the accounting user interface you need to provide the list users.

---

### Step 9: Configure PowerBI

!!! The following information refers to the sheet `Step 9 - PowerBI User` of the [application template (EXCEL file)](./technical-application-form.xlsx).

!! **TODO** Discuss about the configuration option that are available for this step

---

### Step 10: Configure support

!!! The following information refers to the sheet `Step 10 - 2nd level JIRA` of the [application template (EXCEL file)](./technical-application-form.xlsx).

!! **TODO** Discuss about the configuration option that are available for this step
