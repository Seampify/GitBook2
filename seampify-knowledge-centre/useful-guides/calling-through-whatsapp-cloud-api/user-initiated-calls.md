# User-initiated Calls

WhatsApp Business Calling allows customers to call your business directly through WhatsApp.

**User-initiated calls are free of Meta's calling connectivity charges.**

Your business can manage call availability by configuring business hours and holiday schedules through the calling settings.

{% hint style="success" %}
**Tip:** Before you begin, ensure WhatsApp Business Calling is enabled for your business phone number. Refer to [Calling through WhatsApp Cloud API](https://seampify.gitbook.io/seampify/useful-guides/calling-through-whatsapp-cloud-api) for setup instructions.
{% endhint %}

Once a customer initiates a call, your business must answer within the available ringing period. Otherwise, the call will end and appear as unanswered.

***

## 1. Promoting Your WhatsApp Call

After enabling WhatsApp Business Calling, you can encourage customers to call your business through two methods:

* [Send a message with a WhatsApp Call Button](user-initiated-calls.md#send-interactive-message-with-a-whatsapp-call-button)
* [Embed a Calling Deep Link](user-initiated-calls.md#calling-deep-links) on your website, application, or other communication channels.

#### i. Send Message with a WhatsApp Call Button <a href="#send-interactive-message-with-a-whatsapp-call-button" id="send-interactive-message-with-a-whatsapp-call-button"></a>

There are 2 types of message where you can allow your customer to perform a call to your number:

1. **Interactive Message:** Send a regular interactive message with a WhatsApp Call Button within the [24-hour customer service window](../conversation-through-whatsapp-cloud-api-1/understanding-24-hour-customer-service-window.md).
2. **Template Message:** Send an approved Marketing or Utility template containing a WhatsApp Call Button, including outside the [24-hour customer service window](../conversation-through-whatsapp-cloud-api-1/understanding-24-hour-customer-service-window.md).

When customers tap the call button, they can initiate a WhatsApp voice call to your business.

<figure><img src="../../.gitbook/assets/image (132).png" alt=""><figcaption></figcaption></figure>

#### ii. Creating Calling Deep Links

Calling deep links allow customers to initiate a WhatsApp voice call to your business through a clickable URL.

Use the following format:

`https://wa.me/call/<BUSINESS_PHONE_NUMBER>`

Replace `<BUSINESS_PHONE_NUMBER>` with your WhatsApp business phone number in international format, without the `+` symbol, spaces, brackets, or hyphens.

**Examples:**

**Correct formats:**

* Malaysia (+60): `https://wa.me/call/60123456789`
* Singapore (+65): `https://wa.me/call/6591234567`
* General example: `https://wa.me/call/1XXXXXXXXXX`

**Incorrect format:**

`https://wa.me/call/+001-(XXX)XXXXXXX`

_Note: The phone numbers above are examples only. Replace them with your actual WhatsApp business number._

{% hint style="danger" %}
**Caution:** Calling deep-link support may vary depending on the customer's device and WhatsApp application. Test your link before sharing it publicly.
{% endhint %}

#### iii. Embed calling deep links <a href="#embed-calling-deep-links" id="embed-calling-deep-links"></a>

You can embed calling deep links on your website, mobile application, or other platforms to allow customers to initiate WhatsApp calls directly.

Calling deep links can also be converted into QR codes for use on printed materials or promotional campaigns.

<figure><img src="../../.gitbook/assets/image (118).png" alt=""><figcaption></figcaption></figure>

#### **iv. Send Calling Deep Links**

You can also share calling deep links directly with customers through supported messaging channels.

Each calling deep link is associated with a specific WhatsApp business phone number. This allows you to direct customers to the appropriate business number with calling enabled.

<figure><img src="../../.gitbook/assets/image (119).png" alt=""><figcaption></figcaption></figure>

***

## 2. Frequently Asked Questions

<details>

<summary>Am I eligible for WhatsApp calling?</summary>

Before getting started with the Calling API, ensure that:

1. Your business phone number is connected to the WhatsApp Cloud API.
2. Your business portfolio has a messaging limit of at least 2,000 unique customers within a rolling 24-hour period.
3. You have [enabled the Calling API feature](https://seampify.gitbook.io/seampify/useful-guides/calling-through-whatsapp-cloud-api#step-1-prerequisites) for your business phone number.

</details>

<details>

<summary>What is the maximum number of concurrent calls a single Cloud API phone number can receive?</summary>

Meta supports up to **1,000 concurrent calls per WhatsApp business phone number**.

If this limit is exceeded, customers may be unable to place additional calls until capacity becomes available.

Calling limits are separate from WhatsApp messaging limits.

</details>

<details>

<summary>What is the maximum supported call duration?</summary>

Meta does not specify a general maximum call duration for WhatsApp Business Calling. However, actual call duration may depend on network conditions and your calling provider.

</details>

<details>

<summary>Can I send or receive messages while a call is in progress?</summary>

Yes. You can continue sending and receiving WhatsApp messages while a voice call is in progress.

</details>

<details>

<summary>Does the WABA need to be a verified business for calling?</summary>

Meta Business Verification is not necessarily required solely to enable user-initiated calling.

However, your business phone number must meet the applicable Calling API eligibility and configuration requirements.

</details>

<details>

<summary>Does Calling API usage affect my messaging limits?</summary>

No. WhatsApp calling and messaging limits are managed separately.

Calling activity does not count towards your business portfolio's template messaging limit.

[More details about Messaging Tier Limit here](../messaging-limits-for-click-to-whatsapp-ads-ctwa/)

</details>

<details>

<summary>When is the call icon visible in a customer's WhatsApp chat?</summary>

It is visible when **all the following conditions are met:**

* The business phone number's calling status is set to `ENABLED` in the [Call Settings API](./#step-2-configure-optional-calling-features).
* The call button visibility setting is enabled.
* The customer's WhatsApp application supports the calling feature.

</details>

<details>

<summary>Can we limit calling access to specific or individual WhatsApp users instead of all users?</summary>

For example, can we allow only qualified leads or premium customers to call?

No. Meta does not currently provide a way to control call icon visibility individually for each WhatsApp user.

However, you can use the [Call Settings API](./#step-2-configure-optional-calling-features) to set `call_icon_visibility` to `DISABLE_ALL`, hiding the call icon from all users.

You can then send WhatsApp Call Buttons to selected customers, allowing them to initiate calls directly from those messages.

**Note:** Hiding the call icon does not completely restrict calling access. Additional filtering may be required through your Seampify automation or business logic.&#x20;

</details>

<details>

<summary>When the call icon is hidden using Call Settings API, can customers still call the business?</summary>

Yes. Customers may still call your business through other entry points, including:

* Saving your business number as a contact and initiating a new call.
* Previous call records under **Calls > Recent**.
* WhatsApp Call Buttons in messages.
* Call bubbles displayed in the chat after a previous call.

Therefore, `DISABLE_ALL` should only be treated as a first-level visibility control.

</details>

<details>

<summary>What is the minimum version of WhatsApp mobile apps that support the voice call button?</summary>

Customers should use the latest available version of WhatsApp on Android or iOS.

Older application versions may not support certain WhatsApp Calling features.

</details>

<details>

<summary>Is calling supported for end users from WhatsApp Web or WhatsApp Desktop apps?</summary>

WhatsApp Business Calling support varies across WhatsApp Web, Desktop, and mobile applications.

For the most reliable experience, customers should use the latest WhatsApp mobile application on Android or iOS.

</details>

<details>

<summary>What countries are supported for calling?</summary>

**User-Initiated Calling (UIC)**

User-initiated calling is generally available in locations where WhatsApp Cloud API supports business calling, subject to Meta's country restrictions.

**Business-Initiated Calling (BIC)**

Business-initiated calling is available in supported countries, subject to Meta's restrictions and eligibility requirements.

Some countries, including the United States, Canada, Egypt, Nigeria, and Vietnam, have restrictions on business-initiated calling.

For the latest information, refer to [Meta's WhatsApp Business Calling API documentation](https://developers.facebook.com/docs/whatsapp/cloud-api/calling/).

{% hint style="warning" %}
**Important:** Eligibility generally depends on the business phone number's country code. Supported countries and restrictions may change.
{% endhint %}

</details>
