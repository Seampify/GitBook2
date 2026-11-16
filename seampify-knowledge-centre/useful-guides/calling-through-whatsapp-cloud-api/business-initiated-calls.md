# Business-initiated Calls

The Calling API supports making calls to WhatsApp users from your business.

WhatsApp users control whether they can receive calls by granting call permissions to your business phone number.

***

## 1. Obtain User Call Permissions <a href="#part-1--obtain-permission-to-call-the-whatsapp-user" id="part-1--obtain-permission-to-call-the-whatsapp-user"></a>

If you want to place a call to a WhatsApp user, your business must receive user permission first.

When a WhatsApp user grants call permission, it can be temporary for 7 calendar days (168 hours) or permanent until the user revokes it.

You can obtain calling permission from a WhatsApp user in any of the following ways:

* Send a call permission request to the user.
* Receive callback permission when a WhatsApp user calls your business, regardless of whether you accept the call, provided callback permissions are enabled.
* The WhatsApp user grants call permission directly through your WhatsApp business profile.

### Send a Call Permission Request to the User

A call permission request message can be sent to users in one of the following ways:

* [Create and send a template message](business-initiated-calls.md#create-and-send-a-template-message)
* [Send a free form message](business-initiated-calls.md#send-a-free-form-message)

#### **i. Create and Send a Template Message**

To request call permission from a WhatsApp user, your business can create and send a Call Permission Request template message.

Call Permission Request template messages are available under the Marketing and Utility categories.

Once the template message is approved, you can send it to your contact, including outside the 24-hour customer service window.

For more information, refer to [Meta's User Call Permissions documentation](https://developers.facebook.com/documentation/business-messaging/whatsapp/calling/user-call-permissions/).

{% hint style="info" %}
**Note:** Call permission request template messages are subject to applicable messaging charges.
{% endhint %}

This is what your customer will see when they receive the call permission request.

<figure><img src="../../.gitbook/assets/image (161).png" alt=""><figcaption></figcaption></figure>

#### **ii. Send a Free-Form Message**

When you are within an open 24-hour customer service window with a WhatsApp user, you can send a free-form message with a call permission request.

Send an interactive message using the Call Permission Request message type to ask the customer for permission to call them.

This is what your customer will see when they receive the call permission request.

<figure><img src="../../.gitbook/assets/Allow call.jpg" alt=""><figcaption></figcaption></figure>

### Callback Permission Is Provided by the WhatsApp User

The WhatsApp user automatically provides temporary call permission by placing a call to the business.

The callback setting must be enabled on the business phone number.

<figure><img src="../../.gitbook/assets/image (5).png" alt=""><figcaption></figcaption></figure>

### Performing a Business-initiated Calls <a href="#limits-per-business-whatsapp-user-pair" id="limits-per-business-whatsapp-user-pair"></a>

The WhatsApp user may approve, decline or simply not respond to a call permission request.

Once you have user permission, your business can initiate a WhatsApp voice call to the contact.

Business-initiated calls are subject to [Calling API Pricing](https://seampify.gitbook.io/seampify/useful-guides/calling-through-whatsapp-cloud-api/calling-api-pricing).

***

## 2. Limits (Per business + WhatsApp User Pair) <a href="#limits-per-business-whatsapp-user-pair" id="limits-per-business-whatsapp-user-pair"></a>

* Temporary permissions are granted for 7 calendar days (168 hours), including when the user calls your business first and callback permissions are enabled.
* The temporary permission period is calculated from the time the permission is granted.
* Businesses can make up to 100 connected calls within a 24-hour period, subject to Meta's applicable calling limits.
* These limits apply to the business phone number.

These limits are in place to protect WhatsApp users from unwanted calls.

***

## 3. User Preference Options

When your business sends a call permission request on WhatsApp, the customer is presented with three distinct options to manage their privacy: **Allow**, **Allow temporarily**, and **Not at this time**.

These preferences determine how long your business has permission to initiate voice calls to that specific contact.

**Allow:** This grants your business ongoing permission to initiate calls to the customer. The permission remains active until the user manually changes their preference or blocks the business.

**Allow temporarily:** This grants permission for 7 calendar days (168 hours). After this period expires, your business must obtain call permission again before initiating another call.

**Not at this time:** This declines the current request. Your business will not be able to initiate a call unless the customer subsequently grants permission. You must comply with Meta's call permission request limits before sending another request.

<figure><img src="../../.gitbook/assets/image (177).png" alt=""><figcaption></figcaption></figure>

***

## 4. Call Permission Request Basics <a href="#call-permission-request-basics" id="call-permission-request-basics"></a>

The WhatsApp user is in control. Even if the user provides calling permission, they can revoke that permission at any time.

Conversely, if the user declines a permission request, they can still grant calling permission until the permission request expires.

A call permission request expires when any of the following occurs:

* The WhatsApp user interacts with a subsequent new call permission request from the business.
* 7 days after the permission request was accepted or declined by the user.
* 7 days after the permission request was delivered if the user does not respond to the request.

<figure><img src="../../.gitbook/assets/image (184).png" alt=""><figcaption><p>Permission request expires after 7 days — User interacts with request</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (185).png" alt=""><figcaption><p>Permission request expires after 7 days — User does not interact</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (187).png" alt=""><figcaption><p>Previous permission request expires immediately — User does not interact / New call permission request is received</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (190).png" alt=""><figcaption><p>Previous permission request expires immediately — User allows / Interacts with the new request</p></figcaption></figure>

***

## 5. Call Permission Request Limits

These limits reset when any connected call (business-initiated or user-initiated) is made between the business and the WhatsApp user.

These limits apply to permission requests sent either as free-form or template messages.

#### i. When Business-Initiated Calls Go Unanswered or Are Rejected

* 2 consecutive unanswered calls result in a system message asking the user to reconsider the approved permission.

<figure><img src="../../.gitbook/assets/2 consecutive unasnwered.jpg" alt=""><figcaption></figcaption></figure>

* 4 consecutive unanswered calls result in the approved permission being automatically revoked. The user may grant permission again if they choose to do so.

<figure><img src="../../.gitbook/assets/4 consecutive unasnwered.jpg" alt=""><figcaption></figcaption></figure>

***

## 6. Frequently Asked Questions&#x20;

<details>

<summary>Am I eligible for WhatsApp calling?</summary>

Before you get started with the Calling API, ensure that:

1. Your business number is in use with Cloud API (not the WhatsApp Business app)
2. The business phone number should be in the Messaging Tier of at-least 2,000 (2K) messages. [More details about Messaging Tier Limit here](../messaging-limits-for-click-to-whatsapp-ads-ctwa/)
3. [Enable Calling features on your business phone number](./#step-1-prerequisites)

</details>

<details>

<summary>What are the countries supported for calling?</summary>

**User-initiated Calling (UIC)**\
UIC is available in every location Cloud API is available

**Business-initiated Calling (BIC)**\
BIC is currently available in every location Cloud API is available, except the following countries:

USA\
Canada\
Turkey\
Egypt\
Vietnam\
Nigeria

{% hint style="warning" %}
Note: The business phone number’s country code must be in this supported list. The consumer phone number can be from any country where Cloud API is available.
{% endhint %}

</details>

<details>

<summary>Does the WABA need to have an attached credit line for using Calling APIs?</summary>

Yes, you need a credit line attached to your WABA in order to use the Calling API. [Refer to Calling API Pricing for the rate card.](calling-api-pricing.md#volume-based-pricing--vbp--rate-card)

</details>

<details>

<summary>What WhatsApp versions and client platforms support the business initiated calling feature?</summary>

WhatsApp Client versions 2.24.14.x and onwards support the call permission requests and business initiated calling feature.

Both WhatsApp Android and iOS platforms support the feature.

</details>

<details>

<summary>Does the permission expire after five connected calls have been made?</summary>

5 connected calls in 24 hours is simply a time window based running limit. Reaching that limit does not close the permission, permission remains open until the full 7 days. The 6th call can happen 24hrs after the 1st call.

We can simply think of this as a rate limit for business initiated calls. A maximum of 35 calls can happen over 7 days.

</details>

<details>

<summary>Is there a way to reset the call permission request limits?</summary>

A connected call will reset the [call permission request limits](business-initiated-calls.md#call-permission-request-limits)

</details>

<details>

<summary>What happens if the WhatsApp user has set up <a href="https://faq.whatsapp.com/1238612517047244/?cms_platform=android&#x26;fbclid=IwZXh0bgNhZW0CMTEAYnJpZBExQTBLZ01YQkJxVTNZSTRiQgEevQ9SUDauHlsOFgILu6BxDC2AeMO--nIma1RftSUnLXCs9Pk7RuLyt3T_zoU_aem_owpp5XKRKRdFeuaOYRrrCg">Silence Unknown Callers</a> settings?</summary>

Business initiated calls bypass ‘Silence Unknown Callers’ settings since the call can only happen after explicit permission provided by the user.

</details>

<details>

<summary>Can we place a call with an ongoing number?</summary>

No, you are not able to place a call when it is already ongoing with the receiver.

</details>
