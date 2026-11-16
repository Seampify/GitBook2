---
icon: message-exclamation
---

# Possible Reason for "Message Undeliverable"

When sending message templates to your contacts through Seampify, you may occasionally encounter a **"Message Undeliverable"** error.

This means Meta was unable to deliver your message to the recipient.

<figure><img src="../../.gitbook/assets/image (31).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (32).png" alt=""><figcaption></figcaption></figure>

***

## **1. Possible Reasons**

The following situations may cause a message to appear as sent but not delivered. Meta may not disclose the exact reason due to privacy and policy restrictions.

* **Invalid WhatsApp number:** The recipient's phone number is not registered with WhatsApp.
* **Blocked business number:** The recipient has blocked your WhatsApp business number.
* **Recipient offline:** The recipient did not come online before the message expired.
* **Terms of Service:** The recipient has not accepted WhatsApp's latest Terms of Service and Privacy Policy.
* **Outdated WhatsApp version:** The recipient is using an older version of WhatsApp that may not support certain messages. This includes WhatsApp on Android, iOS, and other supported platforms.
* **Country restrictions:** The recipient is located in a [restricted or sanctioned country](https://developers.facebook.com/docs/whatsapp/cloud-api/support#country-restrictions).

Other delivery restrictions may include:

* **Marketing message limits:** Meta may limit the number of marketing templates a customer receives to maintain a positive messaging experience. Learn more about [Per-User Marketing Template Message Limits](https://developers.facebook.com/docs/whatsapp/cloud-api/guides/send-message-templates#per-user-marketing-template-message-limits).
* **Experiment-related restrictions:** Some recipients may be included in Meta's [marketing message experiments](https://developers.facebook.com/docs/whatsapp/cloud-api/guides/experiments), which can affect message delivery.

{% hint style="warning" %}
**Important:** Marketing message limits and experiment-related restrictions may have different error codes from "Message Undeliverable". Check the error details to identify the appropriate solution.
{% endhint %}

***

## 2. How to Solve This?

If your message fails to deliver, contact the recipient through another communication method, such as email, SMS, or phone call, and ask them to:

1. **Verify their WhatsApp number:** Confirm that their phone number is registered with WhatsApp and that they can send messages to your business.
2. **Check blocked contacts:** Ensure your business number is not blocked under **WhatsApp Settings > Privacy > Blocked Contacts**.
3. **Accept the latest terms:** Check for any pending WhatsApp Terms of Service or Privacy Policy updates.
4. **Update WhatsApp:** Install the latest available version of WhatsApp for their device.

If the issue persists, review the message error details in Seampify or contact our support team for further assistance.
