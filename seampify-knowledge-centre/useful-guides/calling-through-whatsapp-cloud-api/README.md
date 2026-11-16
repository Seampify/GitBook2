# Calling through WhatsApp Cloud API

On 15 July 2025, Meta introduced the Cloud API Calling solution, allowing businesses to make and receive WhatsApp voice calls using Voice over Internet Protocol (VoIP).

***

## **1. Get Started with Cloud API Calling**

### Prerequisites

Before getting started with the Calling API, ensure that:

1. Your business phone number is registered on WhatsApp Cloud API, rather than using only the WhatsApp Business app.
2. Your business portfolio has a messaging limit of at least **2,000 (2K) unique customers within a rolling 24-hour period**. [Learn more about messaging limits here](https://seampify.gitbook.io/seampify/useful-guides/broadcasting-through-whatsapp-cloud-api/broadcast-messaging-limit).
3. Calling features are enabled for your business phone number.

#### i. How to Enable Calling

{% stepper %}
{% step %}
Go to **Channels** from the left-hand navigation menu in Seampify.

Click **Settings** on the WhatsApp channel you wish to configure.

<figure><img src="../../.gitbook/assets/image (133).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
Click the **Calls** tab and enable **Allow voice calls**.

Click **Save Settings** to apply your changes.

<figure><img src="../../.gitbook/assets/image (137).png" alt=""><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

{% hint style="warning" %}
**Reminder:** Calling is not enabled by default on a WhatsApp business phone number.
{% endhint %}

***

## 2. Configure Optional Calling Features

The WhatsApp Business Calling API offers several settings that control when and how customers can call your business through WhatsApp.

#### i. Allow voice calls

This is the main setting for enabling or disabling voice calls on your WhatsApp business phone number.

<figure><img src="../../.gitbook/assets/image (379).png" alt=""><figcaption></figcaption></figure>

#### ii. Display call buttons

When Calling API features are enabled for your business phone number, you can choose whether to display the call button in WhatsApp using the **Display call buttons** setting.

{% hint style="info" %}
**Note:** Disabling call button visibility does not completely prevent WhatsApp users from calling your business through other supported entry points.
{% endhint %}

The available options are as follows:

**DEFAULT**

The call button is displayed in the WhatsApp chat, allowing customers to initiate calls directly to your business.

<figure><img src="../../.gitbook/assets/image (382).png" alt=""><figcaption></figcaption></figure>

**DISABLE ALL**

The call button is hidden from the WhatsApp chat.

Your business can still send interactive messages or message templates containing a WhatsApp Call Button, allowing selected customers to initiate calls.

<figure><img src="../../.gitbook/assets/image (383).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
**Note:** Customers may still be able to call your business through other supported entry points, such as previous call records or call buttons in messages.
{% endhint %}

#### **iii. Available Call Hours**

The **Available Call Hours** setting allows you to specify your business's time zone, weekly operating hours, and holiday schedules for user-initiated calls.

When this setting is configured, customers can only initiate calls during your available operating hours.

User-initiated calls will be unavailable outside your configured hours and on designated holidays.

During these periods, WhatsApp may offer customers the option to:

* Send a message to your business.
* Request a callback, if **Allow people to request a callback for missed calls** is enabled.
* View the next available calling time.

<figure><img src="../../.gitbook/assets/image (149).png" alt=""><figcaption></figcaption></figure>

#### iv. Callback Permissions

Businesses must obtain explicit permission from a WhatsApp user before initiating a call.

One way to obtain call permission is to request it when a customer calls your business.

You can configure the callback permission setting to automatically display a permission request in the customer's WhatsApp application after they call your business.

Customers can change or revoke their call permissions at any time.

<figure><img src="../../.gitbook/assets/image (385).png" alt=""><figcaption></figcaption></figure>

***

## 3. Make and Receive Calls

Cloud API Calling supports two types of calls:

[**User-Initiated Calls:**](user-initiated-calls.md)\
Calls initiated by a WhatsApp user to your business.\
\
[**Business-Initiated Calls:**](business-initiated-calls.md)\
Calls initiated by your business to a WhatsApp user. Customer permission is required before your business can initiate a call.

User-initiated calls are free of Meta's calling connectivity charges, while business-initiated calls are subject to applicable calling charges.

For more information, refer to [Calling API Pricing](https://seampify.gitbook.io/seampify/useful-guides/calling-through-whatsapp-cloud-api/calling-api-pricing).

#### i. Availability

**User-Initiated Calling (UIC)**

User-initiated calling is available in countries where WhatsApp Cloud API is supported, subject to Meta's applicable restrictions.

**Business-Initiated Calling (BIC)**

Business-initiated calling is currently available in countries where WhatsApp Cloud API is supported, except for the following:

* United States (USA)
* Canada
* Türkiye (Turkey)
* Egypt
* Vietnam
* Nigeria

{% hint style="warning" %}
**Important:** Eligibility is determined by the country code of your WhatsApp business phone number. The customer's phone number can be from any country where WhatsApp Cloud API is supported.
{% endhint %}
