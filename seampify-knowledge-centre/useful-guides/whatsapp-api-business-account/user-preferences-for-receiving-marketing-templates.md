# User Preferences for Receiving Marketing Templates

Meta emphasises that WhatsApp users should always have control over their inboxes. Users can decide how and when they receive messages from businesses through features such as message opt-ins and marketing preferences.

With **Offers and announcements**, WhatsApp users can indicate their interest in marketing messages from your business, or stop and resume receiving them entirely.

{% hint style="warning" %}
**Important:** This is a WhatsApp platform feature and cannot be directly controlled by Seampify.
{% endhint %}

***

## 1. Interested/Not Interested Feedback

<figure><img src="../../.gitbook/assets/image (298).png" alt=""><figcaption></figcaption></figure>

WhatsApp users can use the **Offers and announcements** setting to indicate how interested they are in receiving marketing template messages from your business.

If a user selects **Not interested**, it may affect the [per-user marketing template messaging limits](https://developers.facebook.com/docs/whatsapp/cloud-api/guides/send-message-templates#per-user-marketing-template-message-limits) between your business and the user.

Selecting this option also displays a second prompt, allowing the user to stop receiving marketing messages from your business entirely.

**Note:** Selecting Not interested does not automatically stop all marketing messages. Users must choose to stop delivery if they no longer wish to receive them.

***

## 2. Stop/Resume Controls <a href="#stop-resume-controls" id="stop-resume-controls"></a>

<figure><img src="../../.gitbook/assets/image (301).png" alt=""><figcaption></figcaption></figure>

WhatsApp users can use the **Offers and announcements** setting to stop or resume receiving marketing template messages from your business.

If you attempt to send a marketing template to a user who has stopped receiving marketing messages from your business, the API will process the request, but the message will not be delivered.

{% hint style="success" %}
**Tip:** When a user turns off Offers and announcements for your business, marketing template messages will no longer be delivered to them. However, eligible Utility and Authentication template messages can still be sent for their intended purposes, subject to Meta's policies.
{% endhint %}

***

## 3. Why This Matters for Your Business

By respecting user preferences and limiting message overload, businesses can make their WhatsApp communications more valuable and less intrusive.

Customers are more likely to engage with messages when they trust that they will not be overwhelmed by unwanted promotions.

Although fewer marketing messages may reach users with low engagement or restricted preferences, businesses can focus on **quality interactions over quantity**, helping to improve engagement and customer relationships.

***

## What Businesses Can Do

To adapt, businesses can:

* **Leverage Utility Messages:** Use approved Utility templates for genuine transactional updates, such as order confirmations, appointment reminders, and account notifications. Do not use Utility templates to bypass marketing restrictions.
* **Encourage Opt-Ins:** Obtain customer permission to receive relevant messages through your website, in-store registrations, or direct conversations.
* **Focus on Timing and Value:** Send timely, relevant messages that provide value and encourage positive customer engagement.

By combining appropriate message templates with effective opt-in strategies, businesses can maintain meaningful customer communications while respecting WhatsApp's messaging policies and user preferences.
