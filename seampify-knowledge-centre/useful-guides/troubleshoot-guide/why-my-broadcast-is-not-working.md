---
description: >-
  If your broadcast is not sending messages or is not working as expected, check
  the following possible causes.
---

# Why Is My Broadcast Not Working?

## 1. Check Error Messages

{% stepper %}
{% step %}
#### Go to Campaigns

Navigate to **Campaigns** and locate the campaign you wish to troubleshoot.
{% endstep %}

{% step %}
#### Click on "See Details" of the Campaign

Locate the specific campaign and click **See Details** to view its campaign details.
{% endstep %}

{% step %}
#### Scroll Down and Look for Error Messages

Scroll down within the campaign details page to view any error messages associated with your broadcast.

<figure><img src="../../.gitbook/assets/image (365).png" alt=""><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

***

## 2. Types of Error Messages

#### i. Media Upload Error

**Meaning:** The media you have uploaded may exceed the supported file size limit or be in an unsupported file format.

**Solution:** Ensure that your media meets WhatsApp's supported file types and size limits.

Refer to [Supported Media Types and Sizes on WhatsApp Cloud API](https://seampify.gitbook.io/seampify/useful-guides/conversation-through-whatsapp-cloud-api/supported-media-types-and-sizes-on-whatsapp-cloud-api) for more information.

#### **ii. Business Eligibility Payment Issue**

**Meaning:** Your broadcast may fail due to a payment issue, such as a missing or invalid payment method or outstanding payments on your WhatsApp Business Account.

**Solutions:**

* Ensure that you have a valid payment method linked to your WhatsApp Business Account.
* Check for any outstanding payments or failed transactions.

To check your payment settings:

1. Go to [Meta Business Suite](https://business.facebook.com/).
2. Navigate to **Settings → WhatsApp accounts**.
3. Select your WhatsApp Business Account and click **Payment settings**.
4. Check your payment method and resolve any outstanding payments.

For more information, refer to Setting Up Payment Method.

{% hint style="info" %}
**Note:** Meta's WhatsApp messaging charges are separate from your Seampify subscription or platform fees.
{% endhint %}

#### **iii. Delivery Failed**

**Meaning:** Your broadcast message may fail to deliver for various reasons, such as an invalid phone number, messaging limits, template restrictions or recipient-level messaging restrictions.

**Solution:** Check the error message to identify the cause of the delivery failure before attempting to resend the message.

Refer to [Possible Reasons for Message Undeliverable](https://seampify.gitbook.io/seampify/useful-guides/conversation-through-whatsapp-cloud-api/possible-reason-for-message-undeliverable) to understand the possible reasons and how to resolve them.

By following these steps and referring to the appropriate guides, you should be able to troubleshoot and resolve common issues with your broadcast.
