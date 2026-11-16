# Answering Call from Seampify

With Seampify, you can receive and answer WhatsApp voice calls directly from the platform, allowing your team to communicate with customers without switching between applications.

Before receiving calls, ensure that Calling API features are enabled for your WhatsApp business phone number.

[Learn how to enable Calling through WhatsApp Cloud API](https://seampify.gitbook.io/seampify/useful-guides/calling-through-whatsapp-cloud-api).

***

## 1. Setting Up Automation for Incoming Call

You can set up an automation to automatically assign incoming WhatsApp calls to a specific agent or team.

{% stepper %}
{% step %}
#### Navigate to **Automations** from the left-hand navigation menu.

Click **Create Automation** and enter your desired automation name. Select the WhatsApp channel you wish to use for calling.

<figure><img src="../../.gitbook/assets/image (391).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
#### Select **New Voice Call** as the automation trigger.

Click **Use this trigger** to proceed to the automation builder.

<figure><img src="../../.gitbook/assets/image (152).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
#### Add an **Assign Agent** action to your automation flow.

Under **Assign to**, select your preferred assignment method:

* **Specific user:** Assign the conversation to a specific agent.
* **Team wise Round Robin:** Assign the conversation to an agent within a selected team.
* **Organization wise Round Robin:** Assign the conversation to an agent within the organisation.

You can also configure the following optional settings:

* **Don't assign if already assigned:** Skip the assignment if the conversation already has an assigned agent.
* **Only assign during working hours:** Assign conversations based on the channel's configured working hours.

<figure><img src="../../.gitbook/assets/image (153).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
#### Click **Save** to save your automation settings.

Activate the automation to allow it to run when a new voice call event is received.
{% endstep %}
{% endstepper %}

***

## 2. Answering Call from Seampify

Answering an Incoming Call

When a customer calls your business through WhatsApp, an incoming call notification will appear in Seampify.

You can choose to:

* **Accept:** Answer the incoming call.
* **Decline:** Reject the incoming call.

<figure><img src="../../.gitbook/assets/image (154).png" alt=""><figcaption></figcaption></figure>

***

## 3. Managing an Active Call

Once you accept the call, the call interface will appear in Seampify.

During the call, you can view the call duration, call status and channel information.

Click **Call details** to view additional information, including:

* Direction
* Channel
* Owner
* Call ID

To end the conversation, click **End call**.

<figure><img src="../../.gitbook/assets/image (392).png" alt=""><figcaption></figcaption></figure>

***

## 4. Call Recording

If call recording is enabled in your WhatsApp channel settings, available call recordings can be accessed directly from the conversation in Seampify.

After the call has ended, you can click the **Play** button to listen to the recording.

<figure><img src="../../.gitbook/assets/image (159).png" alt=""><figcaption></figcaption></figure>

{% hint style="warning" %}
**Note:** Call recording must be enabled in your channel settings. Businesses are responsible for complying with applicable laws and consent requirements when recording calls.
{% endhint %}

***

## 5. Call Logs

Seampify allows you to view your WhatsApp call history through System Logs.

Navigate to **System Logs** and select the **Calls** tab.

You can filter your call records by:

* Call direction
* Call status
* Channel
* Date range

The Call Logs table displays information such as the contact, phone number, call direction, outcome, duration, assigned agent, channel and date.

Click **View** under the Actions column to view the details of an individual call.

<figure><img src="../../.gitbook/assets/image (160).png" alt=""><figcaption></figcaption></figure>

{% hint style="warning" %}
**Important:** Call logs can currently be viewed in Seampify. Exporting call logs is not supported.
{% endhint %}

{% hint style="success" %}
**Tip:** When a WhatsApp user calls you, regardless of if you accept the call or not, they will give you a temporary call permissions **for 7 calendar days (168 hours).**
{% endhint %}
