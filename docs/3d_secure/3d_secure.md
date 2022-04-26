---
tags: [3dsecure]
---
# 3D secure

<!-- textlint-disable stop-words -->
3D (three-domain) Secure, also known as 3DS, is a security layer for checkout. It helps prevent fraud by requiring cardholders to authenticate with their issuing bank when making online purchases.

To comply with the PSD2’s Strong Customer Authentication (SCA) requirements, especially in regions where mandated,
merchants should ensure transactions are properly authenticated with 3DS prior to being processed.
<!-- textlint-enable stop-words -->

Nexio uses 3DS 2.x protocol whenever possible, with 3DS 1.x fallback enabled for cases where issuers do not yet support 2.x.

When a transaction is attempted, card issuers use the transactional data provided to determine whether a challenge is required. If a challenge is issued, additional information from the cardholder will be needed, such as a password or one-time code sent to the cardholder by their issuing bank.

## 3D secure through Nexio

Through Nexio, the 3DS authentication workflow happens through a redirect provided by the cardholder’s issuing bank.

With 3DS 2.x, shoppers experience a frictionless flow during which they are redirected from Nexio's secure ecommerce iframe to their bank page and then immediately redirected back to the shopping page.

With 3DS 1.x, shoppers experience a challenge flow during which Nexio’s iframe prompts them to confirm they are being redirected to their bank's page for authentication. After confirmation, the iframe opens a new tab for completing the authentication. After a shopper completes authentication, the transaction is processed.

Merchants using only the Nexio API to process transactions will need to handle the redirect separately.

## Learn more
For more information about 3DS, see [3DS requirements <i role="img" aria-hidden="true" class="sl-icon far fa-external-link-alt fa-xs"></i>](https://docs-beta.nexiopay.com/docs/tutorials/docs/3d_secure/requirements.md) and [Using 3DS to run transactions <i role="img" aria-hidden="true" class="sl-icon far fa-external-link-alt fa-xs"></i>](https://docs-beta.nexiopay.com/docs/tutorials/docs/3d_secure/using_3d_secure.md) in Tutorials.
