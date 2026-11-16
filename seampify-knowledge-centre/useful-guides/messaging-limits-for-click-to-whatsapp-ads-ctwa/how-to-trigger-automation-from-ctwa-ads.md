# How to Trigger Automation from CTWA Ads

This guide explains how to trigger an automation in Seampify when a customer sends a message through [Click-to-WhatsApp Ads (CTWA)](https://seampify.gitbook.io/seampify/useful-guides/messaging-limits-for-click-to-whatsapp-ads-ctwa/how-to-setup-ctwa-ads-from-ads-manager).

After creating your automation, you need to configure its trigger conditions.

There are two ways to trigger an automation from CTWA ads:

1. [Using a Pre-Filled Message](how-to-trigger-automation-from-ctwa-ads.md#how-to-trigger-automation-using-ctwa-a-ds-pre-filled-message)
2. [Using an Ad ID](how-to-trigger-automation-from-ctwa-ads.md#how-to-trigger-automation-using-ctwa-a-ds-id)

{% hint style="info" %}
I**nfo:** If you have not created an automation, refer to [How to Import an Automation Template](https://seampify.gitbook.io/seampify/seampifys-modules/automations/import-automation-template).
{% endhint %}

***

## 1. How to Trigger Automation Using a CTWA Pre-Filled Message

Double-click the **Trigger Node** in your automation and configure the following settings:

* **Trigger Condition:** Message text include any of keywords
* **Text Keywords:** Enter the pre-filled message configured in your CTWA ad.

<figure><img src="../../.gitbook/assets/image (130).png" alt=""><figcaption></figcaption></figure>

{% hint style="success" %}
**Tip:** [Click here to learn how to set up a pre-filled message for CTWA ads.](https://seampify.gitbook.io/seampify/useful-guides/messaging-limits-for-click-to-whatsapp-ads-ctwa/how-to-setup-ctwa-ads-from-ads-manager#setup-pre-filled-message-for-ctwa)
{% endhint %}

{% hint style="info" %}
**Note:** The automation is triggered when the customer sends a message containing the configured keyword. Simply clicking the ad does not trigger the automation.
{% endhint %}

***

## 2. How to Trigger Automation Using a CTWA Ad ID

Another way to trigger an automation is by using the **Ad ID** from Meta Ads Manager.

You can find the Ad ID in your advertisement's details or Ads Manager URL.

For example, an Ads Manager URL may contain:

`selected_ad_ids=123456789012345`

In this example, `123456789012345` is the Ad ID.

Once you have identified your Ad ID, double-click the **Trigger Node** and configure the following settings:

* **Trigger Condition:** Custom Condition
* **Payload Key:** Referral Source Id
* **Operator:** Is Any One
* **Match String:** Enter your Ad ID.

<figure><img src="../../.gitbook/assets/image (131).png" alt=""><figcaption></figcaption></figure>

This allows Seampify to trigger the automation when a customer sends a message originating from the specified CTWA ad.

{% hint style="info" %}
**Note:** The Ad ID method relies on referral information provided by Meta when a customer initiates a conversation through an eligible CTWA ad.
{% endhint %}

Make sure your automation is saved and activated before testing it.
