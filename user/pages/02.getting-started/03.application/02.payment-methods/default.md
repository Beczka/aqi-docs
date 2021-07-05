---
title: Payments method options
---

The following options are avaiable per payment methods:

| Payment method | Captured before delivery (*) | Captured after delivery (by client) (**) | Captured by Aqount (***) |
|----------------|---------------------------|---------------------------------------|-----------------------|
|Direct Debit| No | No | Yes |
|Open Invoice| _No capture required_ | - | - |
|Prepayment| _No capture required_ | - | - |
|Credit card|AMEX, VISA, MasterCard, Diners, Discover|AMEX, VISA, MasterCard, Diners, Discover|AMEX, VISA, MasterCard|
|Cash on delivery|	DHL, Hermes, GLS, Bartolini | - | - |
|SOFORT| Yes | Yes | Yes |
|Customer card|	Yes | Yes | No |
|PayPal| Yes | Yes | Yes |
|IBAN verification| _No capture_ | - | - |
|In-store payment (prepayment)| - | - | No |
|In-store payment (open invoice)| - | - | - |
|In-store payment (with pickup)| - | - | - |
|In-store payment (without revenue)| - | - | - |
|Gift card (100% payment)| Yes | Yes | - |
|iDEAL| Yes | Yes | Yes |
|EPS| Yes| Yes | Yes |
|Bancontact / Mr. Cash| - | - | - |
|P24| Yes | Yes | Yes |
|Afterpay (Open invoice)| _No capture_ | Yes | - |
|Afterpay (Direct debit)| _Mo capture_ | Yes | - |
|Afterpay (Installment payment)| _No capture_ | Yes | - |
|iTunes store payment| Yes | - | - |
|Google play store payment| Yes | - | - |
|Amazon app store payment| Yes | - | - |
|BFS collected (Direct debit)| - | - | - |
|Klarna (Installment payment)| Yes | Yes | Yes |
|Klarna (Open invoice)| Yes | Yes | Yes |
|Klarna (Direct debit)| Yes | Yes | Yes |
|Amazon Pay| Yes | Yes | Yes |
|Huawei Pay| - | - | - |

!! **TODO:** Comments need to be revised and where possible linked to existing content.

(*) If you capture in the frontend with order creation, a payout needs to take place with every cancellation. Aqount does not take over the capture but books the incoming payment and takes over the payout process in case of returns / goodwills.

(**) If the capture is done with the fulfillment of the service/goods, a payout with cancellation is not required. Aqount does not take over the capture but books the incoming payment and takes over the payout process in case of returns / goodwills.

(***) If Aqount shall take over the capture process (request capture from PSP), this option has to be selected.
