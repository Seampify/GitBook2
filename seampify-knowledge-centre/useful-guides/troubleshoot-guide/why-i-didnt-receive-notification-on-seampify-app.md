---
description: >-
  If you are not receiving notifications from the Seampify app, follow these
  troubleshooting steps to resolve the issue.
---

# Why Am I Not Receiving Notifications on the Seampify App?

## 1. **Verify That You're Logged In**

Ensure that you are logged in to your Seampify account on the mobile app. Notifications will only be sent to authenticated users.

***

## **2.** Check App Notification Settings

#### For iOS:

* Go to **Settings → Notifications**.
* Locate the Seampify app.
* Ensure that **Allow Notifications** is enabled.

#### For Android:

* Go to **Settings → Apps**.
* Locate the Seampify app.
* Select **Notifications**.
* Ensure that notifications are enabled.

***

## **3.** Assign Users to Conversations Using Automation

Follow these steps to automatically assign conversations to users and receive notifications:

{% stepper %}
{% step %}
#### **Go to Automations**

Navigate to **Automations** in Seampify and create a new automation.
{% endstep %}

{% step %}
#### **Configure the Trigger**

Select **New Incoming Message** as the trigger and set the trigger condition to **All messages (no filter)**.
{% endstep %}

{% step %}
#### **Add an Assign Agent Node**

Add an **Assign Agent** node and connect it to the Trigger node.

Under **Assign to**, select **Specific user** and choose your name or the agent you wish to assign conversations to.

You can also configure the following optional settings:

* **Don't assign if already assigned:** Skip conversations that already have an assigned agent.
* **Only assign during working hours:** Assign conversations based on the channel's configured working hours.
{% endstep %}

{% step %}
#### **Save and Activate the Automation**

Click **Save** to save the node settings.

Validate your automation, publish your changes and ensure that the automation is active.
{% endstep %}
{% endstepper %}

Once configured, incoming conversations that meet the trigger conditions will be automatically assigned to the selected user.

For more details on setting up automations, refer to the Seampify Automation Guide.

<figure><img src="../../.gitbook/assets/Why I Didn&#x27;t Receive Notification on Seampify App.gif" alt=""><figcaption></figcaption></figure>

For more details on setting up automations, refer to the [Seampify Automation Guide.](../../seampifys-modules/automations/)

***

## **4.** Manually Assign Users to Conversations

If you prefer to manually assign yourself to a conversation, follow these steps:

{% stepper %}
{% step %}
#### **Go to Inbox**

Navigate to **Inbox** in Seampify.
{% endstep %}

{% step %}
#### **Select a Conversation**

Open the conversation you wish to assign.
{% endstep %}

{% step %}
#### **Assign Yourself**

In the right-hand panel, under **Conversation Actions**, locate **Assigned Agent**.

Click **Assign to me** to assign the conversation to yourself.

<figure><img src="../../.gitbook/assets/image (369).png" alt=""><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

Once assigned, you should receive notifications on your Seampify app when new incoming messages are received in the conversation, provided your app notifications are enabled.
