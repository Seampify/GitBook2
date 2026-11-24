# WhatsApp Flows

The **WhatsApp Flows** feature allows you to create interactive forms that customers can complete directly within WhatsApp.

You can use WhatsApp Flows to collect customer information, appointment details, preferences, and other information required by your business.

You can create a WhatsApp Flow manually or generate one using AI.

<figure><img src="../../../../.gitbook/assets/wasap flow (1).png" alt=""><figcaption></figcaption></figure>

## Creating a WhatsApp Flow with AI

The **Create with AI** feature allows you to generate a WhatsApp form by describing what information you want to collect from your customers.

AI will analyze your requirements, design the form structure, and generate the necessary screens and fields.

{% stepper %}
{% step %}
### Describe Your Flow

1. Navigate to **WhatsApp Flows**.
2. Click **Create with AI**.

<figure><img src="../../../../.gitbook/assets/template ai (6).png" alt=""><figcaption></figcaption></figure>

1. The **Create Flow with AI** form will appear.
2. Enter your flow name and describe your requirements.

<figure><img src="../../../../.gitbook/assets/wasap flow ai (1).png" alt=""><figcaption></figcaption></figure>

1. Once you have entered your requirements, click **Generate Flow**.
{% endstep %}

{% step %}
### AI Designing

After clicking **Generate Flow**, AI will begin analyzing your requirements and creating your WhatsApp Flow.

<figure><img src="../../../../.gitbook/assets/wasap flow ai (2).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Preview Your Flow

Review the generated screens, fields, and WhatsApp Preview.

<figure><img src="../../../../.gitbook/assets/wasap flow ai (3).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Publish Your Flow

1. Review the generated flow summary.
2. Confirm or update your Flow Name.
3. Select one of the available actions.
4. Click **Publish Flow** if you are ready to publish.

<figure><img src="../../../../.gitbook/assets/wasap flow ai (4).png" alt=""><figcaption></figcaption></figure>

Alternatively, click **Save as Draft** if you want to make changes later.
{% endstep %}
{% endstepper %}

{% hint style="info" %}
**Note:** AI-generated flows should be reviewed before publishing to ensure the fields, input types, and validation rules meet your business requirements.
{% endhint %}

## Creating a WhatsApp Flow Manually

The **WhatsApp Flow Builder** allows you to manually create and customize interactive WhatsApp forms according to your business requirements.

You can add multiple screens, configure input fields, customize the form layout, and preview how your form will appear to customers before publishing.

{% stepper %}
{% step %}
### Create a New Flow

Click **+ New Flow** to begin creating your WhatsApp form.
{% endstep %}

{% step %}
### Configure Your Flow

<figure><img src="../../../../.gitbook/assets/wasap flow man (1).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Add Form Components

Click **+ Add Component** within your selected screen to open the component library.

<figure><img src="../../../../.gitbook/assets/wasap flow man (2).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Preview and Publish

Once your form is configured:

1. Review the screen structure and components.
2. Check the form using the WhatsApp Preview.
3. Use **Interactive** to test the form.
4. Click **Save** to save your changes.
5. Click **Publish** when your form is ready.
{% endstep %}
{% endstepper %}

### Available Components

The component library includes the following options shown in the screenshot:

| **Component** | **Description**                                                             |
| ------------- | --------------------------------------------------------------------------- |
| Heading       | Add a large heading for your screen.                                        |
| Subheading    | Add a medium-sized heading.                                                 |
| Body Text     | Display standard paragraph text.                                            |
| Caption       | Add smaller supporting text or instructions.                                |
| Rich Text     | Add formatted text with Markdown support.                                   |
| Text Input    | Allow customers to enter a single-line text response.                       |
| Dropdown      | Allow customers to select an option from a dropdown menu.                   |
| Radio Buttons | Allow customers to select a single option.                                  |
| Date Picker   | Allow customers to select a date.                                           |
| Footer Button | Add a primary action button, typically located at the bottom of the screen. |

You can use the **Search components** bar to locate a specific component.

***

## Using WhatsApp Flows in Automations

Once your WhatsApp Flow is published, you can use it within an automation to send an interactive form to your customers.

You can also retrieve the information customers submit and use it in subsequent automation steps.

### _Step 1: Add a WhatsApp Flow Node_

1. Navigate to **Marketing & AI → Automations**.
2. Open an existing automation or create a new one.
3. Add a **WhatsApp Flow** node to your automation.
4. Configure the node to send your WhatsApp Flow to the customer.

<figure><img src="../../../../.gitbook/assets/wasap flow man (3).png" alt=""><figcaption></figcaption></figure>

### _Step 2: Retrieve WhatsApp Flow Responses_

When your customer completes the WhatsApp Flow, the submitted information becomes available as variables in your automation.

For example, if your form collects four fields, the following variables may become available:

| **Variable**           | **Description**                       |
| ---------------------- | ------------------------------------- |
| `{{customer_name}}`    | Customer's submitted name.            |
| `{{preferred_outlet}}` | Customer's selected outlet.           |
| `{{preferred_time}}`   | Customer's selected appointment time. |
| `{{phone_number}}`     | Customer's submitted phone number.    |

These variables can be accessed through the **Insert Variable** menu under the **Node – WhatsApp Flow** category.

{% hint style="info" %}
**Note:** The available variables depend on the fields configured in your WhatsApp Flow.
{% endhint %}

### Step 3: Display Submitted Information

To display the customer's submitted information:

1. Connect a **Send Message** node after the WhatsApp Flow node.
2. Enter the message you want to send.
3. Click the **@** icon to open the Insert Variable menu.

<figure><img src="../../../../.gitbook/assets/wasap flow man (4).png" alt=""><figcaption></figcaption></figure>

1. Locate the **Node – WhatsApp Flow** section.
2. Select the relevant variables.
3. Click **Save**.

You can also configure optional buttons, such as **Confirm** and **Reschedule**, to let customers respond to the submitted information.

### _Step 4: Save Your Automation_

Once the WhatsApp Flow and Send Message nodes are configured:

1. Review the connection between both nodes.
2. Verify that the correct response variables are selected.
3. Save your automation.
4. Test the workflow to ensure the submitted information appears correctly.

{% hint style="info" %}
**Note:** When using WhatsApp Flow responses in your automation, always select the variables from the **Node – WhatsApp Flow** section to ensure the correct submitted values are mapped into your message.
{% endhint %}

## WhatsApp Flow Responses

The **Responses** section allows you to view and manage information submitted by your customers through WhatsApp Flows.

All submitted responses are displayed in a centralized table, allowing you to review customer details, submission dates, and response statuses.

### Accessing Flow Responses

1. Navigate to **Settings → Channels**.
2. Select your WhatsApp channel.
3. Click **Flows**.
4. Select the **Responses** tab beside **Flows**.

<figure><img src="../../../../.gitbook/assets/flow res (1).png" alt=""><figcaption></figcaption></figure>

5. All recorded WhatsApp Flow responses will be displayed.

### Viewing Submitted Responses

To view the details of a submitted form:

1. Navigate to the **Responses** tab.
2. Locate the submission you want to review.
3. Click the three-dot menu under **Actions**.
4. Open the response details.
5. Or you can just click the response to open the details.

<figure><img src="../../../../.gitbook/assets/flow res (3).gif" alt=""><figcaption></figcaption></figure>

