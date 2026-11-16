# Calling API Pricing

Placing business-initiated calls is charged based on:

* The duration of the call (calculated in six-second increments, rounded up).
* The country code of the phone number associated with the user being called.
* The monthly calling volume, which determines the applicable pricing tier.

All user-initiated calls are free of Meta's calling connectivity charges.

A valid payment method is required to place business-initiated calls.

**Note:** Call permission request template messages are subject to [messaging charges](https://seampify.gitbook.io/seampify/useful-guides/conversation-through-whatsapp-cloud-api/whatsapp-conversation-based-pricing).

***

## 1. Volume-Based Pricing (VBP) Rate card <a href="#volume-based-pricing--vbp--rate-card" id="volume-based-pricing--vbp--rate-card"></a>

The following rate card shows Meta's volume-based pricing for the WhatsApp Business Calling API.

{% hint style="info" %}
**Note:** Cost per minute in MYR on the WhatsApp Business Platform, effective 1 April 2026.
{% endhint %}

<table data-header-hidden><thead><tr><th valign="top"></th><th valign="top"></th></tr></thead><tbody><tr><td valign="top"><strong>Business-initiated call minutes (per month)</strong></td><td valign="top"><strong>Meta rate (MYR) for Malaysia recipient numbers +60</strong></td></tr><tr><td valign="top">1 -50,000</td><td valign="top">0.0435</td></tr><tr><td valign="top">50,001 - 250,000</td><td valign="top">0.0379</td></tr><tr><td valign="top">250,001 - 1,000,000</td><td valign="top">0.0286</td></tr><tr><td valign="top">1,000,001 -2,500,000</td><td valign="top">0.0278</td></tr><tr><td valign="top">2,500,001 - 5,000,000</td><td valign="top">0.0238</td></tr><tr><td valign="top">5,000,001 and above</td><td valign="top">0.0213</td></tr></tbody></table>

{% hint style="warning" %}
**Important:** [Click here to view the Meta's latest Calling API rate card.](https://developers.facebook.com/documentation/business-messaging/whatsapp/calling/pricing)
{% endhint %}

## Example Charges

Meta calculates call charges in **six-second increments**, rather than per second or per full minute.

Each six-second block is called a **pulse**.

**Examples:**

* If your call lasts **4 seconds**, you are charged for **6 seconds**.
* If your call lasts **7 seconds**, you are charged for **12 seconds**.
* If your call lasts **20 seconds**, you are charged for **24 seconds**.

The billed duration is always rounded up to the next six-second block.

Here's an example calculation for a business-initiated call to a Malaysian phone number:

**Rate card:** MYR 0.0435 per minute

**Actual call length:** 22 seconds

**Billed duration:** 24 seconds (4 pulses)

**Calculation:** MYR 0.0435 × (24 ÷ 60)

**Cost: MYR 0.0174**

***

## 2. How Calling Changes the 24-Hour Customer Service Window <a href="#how-calling-changes-the-24-hour-customer-service-window" id="how-calling-changes-the-24-hour-customer-service-window"></a>

{% hint style="info" %}
Available since October 1, 2024
{% endhint %}

When a WhatsApp user messages your business, a [24-hour customer service window](https://seampify.gitbook.io/seampify/useful-guides/conversation-through-whatsapp-cloud-api/understanding-24-hour-customer-service-window) opens or refreshes.

Within this window, your business can send non-template messages to the customer. Outside the window, approved message templates are required to initiate contact.

With the Calling API, the customer service window also opens or refreshes:

* When a WhatsApp user calls your business, regardless of whether you answer the call.
* When a WhatsApp user accepts a call from your business.

{% hint style="info" %}
**Note:** From 1 October 2026, Meta charges for service messages after the first 1,000 free service messages per business phone number each month. Utility template messages sent within the customer service window are also chargeable. See [WhatsApp Conversation-Based Pricing](https://seampify.gitbook.io/seampify/useful-guides/conversation-through-whatsapp-cloud-api/whatsapp-conversation-based-pricing) for details.
{% endhint %}
