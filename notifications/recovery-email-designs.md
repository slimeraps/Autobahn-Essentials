# Shopify recovery emails

Both designs were activated in Shopify Messaging on November 21, 2026. The source files are the Custom Liquid sections placed below Shopify's native logo header. The approved [design preview](recovery-email-previews.png) shows sample products.

| Active message | Custom Liquid section | Shopify recovery action |
| --- | --- | --- |
| [You left items in your cart](https://admin.shopify.com/store/autobahnessentials/apps/shopify-messaging/automations/flows/19677708345) | [Cart header](abandoned-cart-header.liquid) | View cart |
| [You left items at checkout](https://admin.shopify.com/store/autobahnessentials/apps/shopify-messaging/automations/flows/19651657785) | [Checkout header](abandoned-checkout-header.liquid) | Continue checkout |

Shopify manages the item images, titles, variants and quantities, recovery links, and unsubscribe footer through native sections. The content background is charcoal, item titles are white, item details are muted, and the recovery buttons are red. Workflow triggers, delays, and recipients are configured in Shopify. GitHub stores the Custom Liquid sections and does not deploy changes to the active messages.

Both active previews passed checks at 600 px and 375 px. The logo and sample product images loaded, the headings and copy fit, and Shopify rendered a recovery link and an unsubscribe link in each message. The preview links were checked for presence without opening customer recovery or unsubscribe flows.

The two header files rendered without horizontal overflow in Chrome at 320 px, 375 px, and 600 px. One Shopify test email of each type reached the store's Gmail inbox on November 21, 2026. Both rendered the gradient, readable headline, sample products, HTTPS recovery link, and unsubscribe link. The recovery links were inspected without placing an order. Both messages returned to Active in Shopify Messaging after the tests.
