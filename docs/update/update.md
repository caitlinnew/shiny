---
tags: [update]
---
# Update
the Update feature allows you to auto-update subscriptions with saved cards by using the account updater service.

This service allows merchants to automatically update saved cards due to changes in card number or expiration date.

Merchants that process recurring transactions will see fewer declines due to invalid or expired cards
by having the most recent card information before the transaction is attempted.

**By default, each new card token is tagged for registration with account updater.**
However, they will not be registered until you have enrolled your merchant account with account updater.
We recommend [checking card enrollment tags <i role="img" aria-hidden="true" class="sl-icon far fa-external-link-alt fa-xs"></i>](docs/update/checking_existing.md) prior to enrolling your merchant account with account updater.

Contact your Nexio sales agent to enroll your merchant account in account updater.

You may also want to configure webhooks for the various event types that may be returned due to changes or actions from the account updater service. For more information and examples of possible responses, see [Event Types <i role="img" aria-hidden="true" class="sl-icon far fa-external-link-alt fa-xs"></i>](https://docs-beta.nexiopay.com/docs/developer-tools/docs/webhooks/webhooks.md#event-types) in Developer Tools.

## Learn more
For additional information, see [Working with account updater <i role="img" aria-hidden="true" class="sl-icon far fa-external-link-alt fa-xs"></i>](docs/update/update.md) in Tutorials.