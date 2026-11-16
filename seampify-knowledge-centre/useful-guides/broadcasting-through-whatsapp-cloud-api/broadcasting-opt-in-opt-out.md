# Broadcasting Opt In/Opt Out

Businesses are required to obtain opt-in permission before sending messages to people on WhatsApp.

As per the WhatsApp Business Messaging Policy, businesses must obtain opt-in permission before contacting people on WhatsApp. This permission does not have to be specifically for WhatsApp, provided that businesses comply with applicable local laws.

Businesses may contact people on WhatsApp if:

* They have provided their mobile phone number or WhatsApp username.
* They have given permission to receive subsequent messages or calls from the business.

For more information, refer to the [WhatsApp Business Messaging Policy](https://whatsappbusiness.com/policy/).

***

## 1. Requirements

Businesses must follow the requirements below when obtaining opt-in:

* Clearly state that a person is opting in to receive communications from the business.
* Clearly state the name of the business they are opting in to receive messages from.
* Comply with applicable laws and regulations.

***

## 2. Opt-In Methods

Businesses are responsible for determining how to obtain opt-in permission in a manner that complies with applicable laws, including providing the necessary notices and obtaining the required permissions.

As long as the opt-in method meets the requirements above, businesses may obtain opt-in through various methods, including:

* SMS
* Website
* Phone calls using an interactive voice response (IVR) flow
* In person or on paper, such as signing a physical document
* WhatsApp conversations

***

## 3. Helpful Tips

Businesses should continue to improve the customer experience when obtaining opt-in permission.

Users should expect the messages they receive. Businesses can set this expectation by:

* Obtaining opt-in permission that covers the different categories of messages they intend to send, such as order updates, relevant offers and product recommendations.
* Obtaining separate opt-in permission for specific message categories to reduce the risk of users receiving unwanted messages.
* Providing clear instructions on how users can opt out of receiving messages and respecting their requests.
* Ensuring that opt-in and opt-out flows are clear and easy to use.
* Clearly communicating the benefits of receiving messages from the business.
* Monitoring the phone number's quality rating, especially when introducing new opt-in methods.

***

## 4. Maintaining High Quality

Maintaining high-quality conversations between businesses and customers is a priority.

WhatsApp users can provide feedback on messages, stop receiving offers and announcements, or block and report a business.

Meta may restrict messaging capabilities if a business receives significant negative feedback or consistently delivers a poor customer experience.

***

## 5. How to Set Up an Opt-In / Opt-Out Message

To maintain a high-quality rating and respect customer preferences, businesses should provide customers with a simple way to subscribe to or unsubscribe from broadcast messages.

In Seampify, you can set up an automation to manage these requests automatically.

There are two ways to set up your Opt-in / Opt-out automation.

### i. Method 1: Create an Automation

{% stepper %}
{% step %}
Navigate to **Automations** and click **Create Automation**.

<figure><img src="../../.gitbook/assets/image (386).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
Enter the automation name, such as "Opt in / Opt Out".

Select the WhatsApp channel where the automation should run and configure the priority order.

Click **Next: Choose trigger**.

<figure><img src="../../.gitbook/assets/image (387).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
Select **New Incoming Message** as the trigger and click **Use this trigger**.

<figure><img src="../../.gitbook/assets/image (388).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
Configure the automation flow.

Set up your trigger conditions using **Exact keyword match**. For example:

* Subscribe: Triggers when a customer sends "Subscribe".
* Unsubscribe: Triggers when a customer sends "STOP" or "unsubscribe".

Add the necessary Send Message and Set Contact Attributes nodes to manage the customer's subscription preference.

Configure the appropriate actions to update the customer's subscription status and send a confirmation message.

<figure><img src="../../.gitbook/assets/image (106).png" alt=""><figcaption></figcaption></figure>

{% hint style="warning" %}
**Reminder:** Ensure that opt-out requests are respected immediately and that unsubscribed contacts are excluded from subsequent broadcasts. Customers who have requested to unsubscribe should not be required to confirm their decision again.
{% endhint %}
{% endstep %}

{% step %}
Save and validate your automation. Once everything is configured correctly, publish the automation and ensure that it is active.

Customers can now subscribe to or unsubscribe from receiving broadcast messages based on the configured automation.
{% endstep %}
{% endstepper %}

### ii. Method 2: Import an Existing Automation

If you already have an exported Opt-in / Opt-out automation file, you can import it into Seampify instead of creating the automation manually.

{% stepper %}
{% step %}
Navigate to Automations, click the dropdown beside Create Automation and select Classic mode (3-step).

<figure><img src="../../.gitbook/assets/image (389).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
Enter your automation name.

Under **Import from JSON**, click **Choose file** and upload your existing Opt-in / Opt-out automation file.

<figure><img src="../../.gitbook/assets/image (390).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
Complete the import and review the automation's settings.

Ensure that the selected channel, trigger conditions and subscription status settings are configured correctly.

Validate and publish the automation when you are ready.

{% hint style="info" %}
**Note:** When importing an automation from JSON, the channel IDs included in the file must already exist in your workspace.
{% endhint %}
{% endstep %}
{% endstepper %}
