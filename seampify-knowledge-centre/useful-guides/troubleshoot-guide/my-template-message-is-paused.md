# Why Is My Template Message Paused?

## 1. Template Pacing <a href="#template-pacing" id="template-pacing"></a>

{% hint style="warning" %}
**Warning:** Since 30 April 2024, template pacing has applied to both Marketing and Utility templates, subject to Meta's eligibility criteria.
{% endhint %}

Template pacing is a mechanism that allows time for customers to provide early feedback on message templates. It helps identify templates that receive poor feedback or engagement before they are sent to too many customers, **reducing the likelihood of negative feedback affecting your business**.

Template pacing applies to eligible Marketing and Utility templates. Newly created templates, previously paused templates that have been unpaused, and existing templates without a **High (Green)** quality rating may be subject to pacing.

Template quality history, such as previous Low quality ratings or pauses, is one of the main factors that can trigger pacing.

When a template is paced, messages are initially sent as usual until Meta's delivery threshold is reached. Subsequent messages may then be temporarily held while Meta evaluates customer feedback.

* **Positive Feedback:** Held messages are released, and sending continues.
* **Negative Feedback:** Held messages may be dropped, and the template may be paused. You should review the template's content, targeting, and delivery strategy.

***

## 2. Utility Template Pacing

Utility templates are subject to pacing only if your business has previously had a Utility template paused.

Once a Utility template has been paused, newly created templates, previously paused templates that have been unpaused, and existing templates without a **High (Green)** quality rating may be subject to pacing for the next **7 days**.

***

## 3. Template Pausing <a href="#template-pausing" id="template-pausing"></a>

If a message template reaches the lowest quality rating (**Active – Low Quality**), Meta may automatically pause it to protect messaging quality.

The pause durations are as follows:

* **1st Instance:** Paused for 3 hours.
* **2nd Instance:** Paused for 6 hours.
* **3rd Instance:** Disabled.

When a template is paused, it cannot be sent to customers. You should stop any automated messaging campaigns that rely on the affected template.

Although you will not be charged for attempting to send a paused template, and the attempt will not count towards your [messaging limit](https://seampify.gitbook.io/seampify/useful-guides/broadcasting-through-whatsapp-cloud-api/broadcast-messaging-limit), Meta's API will reject these requests.

You should only resume your campaigns once the template's status has returned to **Active**.

If you believe the template's content is causing negative feedback, you can edit it to improve its quality and customer engagement.

However, once you edit and resubmit a template for approval, its status changes to **In Review**. The template cannot be sent again until Meta approves it and its status returns to **Active**.

You may also need to adjust your business's targeting, delivery frequency, or other messaging practices if they contribute to negative feedback or low engagement.

{% hint style="warning" %}
**Reminder:** A paused template does not automatically reduce your business portfolio's messaging limit. Other active, high-quality templates can continue to be used. However, repeatedly sending low-quality templates may affect your business's messaging reputation and eligibility for future messaging-limit increases.
{% endhint %}

***

## 4. Pause Notifications <a href="#pause-notifications" id="pause-notifications"></a>

When a message template is paused, Meta may notify you through:

* **WhatsApp Manager** notifications.
* Email notifications.
* Webhook notifications, if you have subscribed to message template status updates.

For more information, refer to [Monitoring Status Changes](https://developers.facebook.com/docs/whatsapp/message-templates/guidelines/#monitoring-status-changes) and [Examples – Template Paused](https://developers.facebook.com/docs/whatsapp/business-management-api/webhooks/components#template-paused).

***

## 5. Unpausing <a href="#unpausing" id="unpausing"></a>

A template paused because of a Low quality rating will generally unpause automatically after the applicable pause duration.

Once unpaused, its status returns to **Active**, and you can resume sending messages using the template.

If you did not stop your automated campaigns, they may resume once the template becomes active. However, we recommend pausing affected campaigns until the template is available again, as Meta's API will reject attempts made during the pause.

The template's quality rating will also be recalculated based on its most recent customer feedback.

Meta may notify you through WhatsApp Manager, email, or subscribed webhooks when the template's status returns to **Active**.

{% hint style="info" %}
**Note:** Templates paused during template pacing may require manual unpausing through WhatsApp Manager or the API, depending on the pause reason.
{% endhint %}

***

## 6. Appeals <a href="#appeals" id="appeals"></a>

If your message template is rejected, you may submit an appeal for Meta's review. Appeals may require supporting samples.

If an approved template has been disabled, you can also edit it and resubmit it for approval, where permitted.

To edit and resubmit a template through **WhatsApp Manager**:

1. Open [WhatsApp Manager](https://business.facebook.com/wa/manage/home/) and navigate to **Account Tools → Message Templates**.
2. If you have multiple WhatsApp Business Accounts, select the relevant account from the dropdown menu.
3. Find the message template you want to edit and click it.
4. Update the template's content.
5. Click **Add Sample** and provide the required sample variable values or media.
6. Click **Submit** to send the template for Meta's review.

Meta will review your submission and notify you of the outcome. Review times may vary.

For more information, refer to [Meta's Message Template Guidelines](https://developers.facebook.com/docs/whatsapp/message-templates/guidelines/).
