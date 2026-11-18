---
description: >-
  There are several reasons why your automation may not be working as expected.
  Below are some common reasons and how you can troubleshoot them.
---

# Why Is My Automation Not Working?

## **1.** Check Whether Your Automation Is Active

First, ensure that your automation is active.

Navigate to **Automations** and check the status of the automation you wish to troubleshoot.

If your automation is paused, activate it before testing again. Also, ensure that the automation is assigned to the correct channel.

<figure><img src="../../.gitbook/assets/image (348).png" alt=""><figcaption></figcaption></figure>

You can also check the total number of runs and the last run time to see whether your automation has been triggered.

***

## **2.** Check Your Trigger Condition

Ensure that you have selected the correct trigger condition for your automation.

If you want your automation to run whenever a new incoming message is received, select **All messages (no filter)**.

<figure><img src="../../.gitbook/assets/image (349).png" alt=""><figcaption></figcaption></figure>

If you have configured a specific trigger condition, the incoming message must meet that condition before the automation can run.

#### i. Ensure Keyword Match

If you have selected **Exact keyword match**, the customer's message must match the keyword configured in your Trigger node.

For example, if you have set your keyword as "Seampify", the automation will be triggered when the customer sends "Seampify".

<figure><img src="../../.gitbook/assets/image (350).png" alt=""><figcaption></figcaption></figure>

Once the keyword matches, the automation will proceed to the next node and send the configured response.

<figure><img src="../../.gitbook/assets/image (351).png" alt=""><figcaption></figcaption></figure>

If the customer sends a different message, such as "Hi Seampify", the automation will not be triggered by this exact keyword condition.

#### ii. First Message or After 24h Window

If you have selected **First message or after 24h window**, the automation will only run when:

* A customer sends their first message to your business.
* A customer sends a new message after the previous 24-hour customer service window has expired.

<figure><img src="../../.gitbook/assets/image (353).png" alt=""><figcaption></figcaption></figure>

If the customer sends another message within an existing 24-hour customer service window, the automation will not be triggered by this condition.

If you wish to trigger the automation for every new incoming message, select **All messages (no filter)** instead.

***

## 3. Automation Not Working for Click-to-WhatsApp (CTWA) Ads

If you are running Click-to-WhatsApp (CTWA) ads and your automation is not working, check whether your automation is configured to identify conversations initiated through your ads.

You can use the **Criteria Router** node to identify incoming conversations based on their source information and trigger the appropriate automation.

#### i. How to Set Up an Automation for Click-to-WhatsApp Ads

{% stepper %}
{% step %}
Create an automation with a **New Incoming Message** trigger and select **All messages (no filter)**.
{% endstep %}

{% step %}
Add a **Criteria Router** node to your automation.
{% endstep %}

{% step %}
Under Conditions, select the appropriate field:

* **Source Id:** Identify conversations associated with a specific source ID.
* **Source Type:** Identify conversations based on their source type.
* **Source Url:** Identify conversations associated with a specific source URL.

<figure><img src="../../.gitbook/assets/image (350).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
Select the appropriate condition (e.g. equals) and enter the corresponding value for your CTWA ad or source.
{% endstep %}

{% step %}
Connect the matching branch to the next action, such as **Send Message**, to send an automated welcome message or continue with your desired automation flow.

Save your changes and ensure that the automation is published and active.

Once configured, the Criteria Router will identify incoming conversations that match your conditions and proceed with the appropriate automation.
{% endstep %}
{% endstepper %}

{% hint style="success" %}
**Tip:** Ensure that the source information configured in your Criteria Router matches the actual source information of the incoming conversation. If the conditions do not match, the automation will not proceed along the intended branch.
{% endhint %}

For more information about setting up Click-to-WhatsApp ads, refer to [How to Set Up CTWA Ads from Ads Manager](https://seampify.gitbook.io/seampify/useful-guides/messaging-limits-for-click-to-whatsapp-ads-ctwa/how-to-setup-ctwa-ads-from-ads-manager).

***

## 4. Still Having Issues?

If your automation is still not working, check the following:

* Ensure that your automation is active and your latest changes are published.
* Ensure that the correct channel is selected.
* Check whether the incoming message meets your trigger conditions.
* Ensure that your automation nodes are connected correctly.
* Check your Criteria Router conditions, if applicable.

If the issue persists, please contact the Seampify support team for further assistance.
