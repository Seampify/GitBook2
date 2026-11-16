# Choosing a Phone Number

When choosing a phone number for the WhatsApp Business Platform (Cloud API), ensure that it meets the following requirements:

* **Valid Phone Number:** Your phone number must be active, owned by your business, and capable of receiving an SMS or voice call for one-time password (OTP) verification.
*   **Existing WhatsApp Account:** If your number is currently registered on WhatsApp Messenger or the WhatsApp Business app, you may need to delete the existing account before registering it on Cloud API. [Learn how to delete your WhatsApp account here](https://seampify.gitbook.io/seampify/useful-guides/whatsapp-api-business-account/how-to-delete-whatsapp-account-on-mobile-app).

    **Note:** Eligible WhatsApp Business app users may be able to connect to Cloud API without deleting their existing account through Meta's WhatsApp Coexistence feature. Contact Seampify Support to confirm whether this option is available.
* **Country Restrictions:** Your phone number must not be registered in any of Meta's [restricted countries](https://developers.facebook.com/docs/whatsapp/cloud-api/support/troubleshooting#country-restrictions), including:
  * Crimea (+7978)
  * Cuba (+53)
  * Iran (+98)
  * North Korea (+850)
  * Syria (+963)
* **Banned Phone Numbers:** Phone numbers banned from WhatsApp cannot be registered unless the ban is lifted. [Contact Meta Support](https://developers.facebook.com/docs/whatsapp/support) if you wish to appeal.

***

## 1. Eligible Phone Numbers for WhatsApp Cloud API:

The following types of phone numbers may be used:

* **Mobile Numbers:** Can be used if they meet Meta's eligibility requirements and can receive OTP verification codes.
* **Landlines:** Can be used if they can receive voice calls for OTP verification.
* **1-800 or Toll-Free Numbers:** May be used if they support direct SMS or voice-call verification and meet Meta's requirements.

{% hint style="warning" %}
**Important:** Phone numbers connected to an Interactive Voice Response (IVR) system may fail verification if the automated system prevents Meta's verification call from reaching you. Temporarily disable the IVR or ensure the verification call can be received directly.
{% endhint %}

***

## 2. Registered Number Limits <a href="#registered-number-limits" id="registered-number-limits"></a>

New business portfolios are initially limited to **two registered WhatsApp business phone numbers**.

This limit can increase to **20 registered phone numbers** when the business portfolio completes Meta Business Verification or reaches a messaging limit of at least **2,000 unique customers**.

For more information, refer to [Broadcast Messaging Limit](https://seampify.gitbook.io/seampify/useful-guides/broadcasting-through-whatsapp-cloud-api/broadcast-messaging-limit#increasing_messaging_limits).
