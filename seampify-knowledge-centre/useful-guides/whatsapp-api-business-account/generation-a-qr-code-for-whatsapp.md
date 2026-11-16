# Generating a QR Code for WhatsApp

[WA.link](https://create.wa.link/) is a tool that helps you create a clickable WhatsApp link or QR code, allowing customers to start a conversation with your business without saving your phone number.

***

## 1. What Does It Do?

It generates a **custom link** as shown here:

```
https://wa.link/abc123
```

WA.link generates a custom WhatsApp link, as shown below:

`https://wa.link/abc123`

When customers click the link, it opens a WhatsApp chat with your business number and displays a pre-filled message, making it easier for them to start a conversation.

Customers can edit the pre-filled message before sending it.

WA.link also allows you to generate QR codes that customers can scan to open the same conversation.

You can create basic WhatsApp links and QR codes without registering an account.

<figure><img src="../../.gitbook/assets/image (828).png" alt=""><figcaption></figcaption></figure>

***

## 2. How to Set Up the Link

Follow these steps to create your WhatsApp link using WA.link.

{% stepper %}
{% step %}
Select the country code associated with your WhatsApp business phone number.
{% endstep %}

{% step %}
Enter the WhatsApp phone number you want customers to contact.
{% endstep %}

{% step %}
Enter a pre-filled message that customers can send to your business.

{% hint style="warning" %}
**Warning:** If you want to trigger a specific Seampify automation, ensure the pre-filled message matches the keyword configured in your automation. Learn how to set up an automation trigger.
{% endhint %}
{% endstep %}

{% step %}
(Optional) Click **Preview** to check whether the message appears as expected.
{% endstep %}

{% step %}
Click **Generate my wa.link** to create your WhatsApp link and QR code.
{% endstep %}
{% endstepper %}

<figure><img src="../../.gitbook/assets/demo3.gif" alt=""><figcaption><p>Step by step video on how to generate a QR &#x26; custom link</p></figcaption></figure>

***

## 3. Set Up a Trigger for an Automation Using a QR Code or Custom Link

Once you've created your WA.link QR code or custom link, you can use the pre-filled message to trigger an automation in Seampify.

Follow these steps to connect your link to an automation:

1. Copy the pre-filled message you entered in WA.link.
2. Go to the automation you want to trigger in Seampify.
3. Click the **⚡ icon** in the top-right corner and select **Trigger Node** under **Starting Point**.
4. Double-click the node and click **Add Trigger Condition**.
5. From the dropdown menu, select **Message text exactly matches any of keywords**.
6. Paste your pre-filled message into the **Text Keyword** field and click **Add**.
7. Click **Update Node**, complete the necessary connections, and click **Save** in the top-right corner.
8. Test your automation by opening the WA.link and sending the pre-filled message to your WhatsApp business number.

{% hint style="success" %}
**Note:** The automation will only trigger when the customer's incoming message matches the configured keyword condition. Scanning the QR code or opening the link alone will not trigger the automation.
{% endhint %}

<figure><img src="../../.gitbook/assets/demo4.gif" alt=""><figcaption><p>Video on how to setup a trigger to automation with the QR/link</p></figcaption></figure>
