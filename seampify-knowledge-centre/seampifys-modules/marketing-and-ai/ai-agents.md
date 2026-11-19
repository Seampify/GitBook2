---
icon: robot
---

# AI Agents

The **AI Agents** page allows users to create and manage AI agents trained on business content to answer customer questions automatically.

To create a new AI Agent, navigate to **Marketing & AI → AI Agents → + New Agent**.

The AI Agent creation form consists of seven configuration sections.

## 1. Basic Information

The **Basic Information** section allows users to configure the AI Agent's name, description, and basic response settings.

<figure><img src="../../.gitbook/assets/ai (1).png" alt=""><figcaption></figcaption></figure>

| **Field**                         | **Description**                                                                                                                             |
| --------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------- |
| Name                              | Enter a name for the AI Agent. This field is required.                                                                                      |
| Description                       | Provide a brief description of the AI Agent's purpose (maximum 500 characters).                                                             |
| Text-only Replies                 | When enabled, the AI Agent will only send plain text replies and matching images from the Images tab, without buttons, lists, or carousels. |
| Turn AI Off When an Agent Replies | Automatically stops the AI Agent from responding when a human agent sends a manual reply in the conversation.                               |

## 2. **Behavior & Instructions**

The **Behavior & Instructions** section allows users to define how the AI Agent should communicate with customers and configure its response behavior.

<figure><img src="../../.gitbook/assets/ai (2).png" alt=""><figcaption></figcaption></figure>

### Agent Instructions

| **Field**              | **Description**                                                              |
| ---------------------- | ---------------------------------------------------------------------------- |
| Persona / Instructions | Define the AI Agent's role, tone, communication style, and behavioral rules. |
| Import from File       | Import instructions from an existing file.                                   |

The instructions are included in the AI Agent's responses to guide its communication behavior.

### Response Configuration

* Confidence Threshold - Set the minimum retrieval confidence required before the AI Agent answers using your content.
* Fallback Message  - Define the message sent when the AI Agent is not confident enough to answer. This field is required.
* Conversational Mode - When enabled, the AI Agent can respond to greetings, small talk, and qualifying questions using its persona, even without a confident content match.
* Max Messages per Reply - Configure the maximum number of WhatsApp messages the AI Agent can split a single reply into. Maximum: 5.
* Wait and Group Messages - Configure how many seconds the AI Agent waits before replying, allowing multiple incoming messages to be grouped into one response. Maximum: 30 seconds.
* Nightly AI-training Exemplar Cap - Set the maximum number of auto-discovered conversation examples queued for nightly review.
* AI Model - Select the Claude model used to generate the AI Agent's responses.

> **Note:** When Conversational Mode is disabled, low-confidence responses use the configured fallback message. When enabled, the AI Agent can respond more conversationally but still uses the fallback message when it cannot answer the customer's question.

## 3. Autonomous Lead Capture

The **Autonomous Lead Capture** feature allows the AI Agent to determine when a CRM lead should be created based on customer conversations.

<figure><img src="../../.gitbook/assets/ai (3).png" alt=""><figcaption></figcaption></figure>

* Enable / Disable - Turn Autonomous Lead Capture on or off.
* Instructions - Configure the instructions used to decide when a CRM lead should be created for a contact.

This feature applies to automation-triggered conversations only and does not operate in Test Chat.

## 4. Autonomous Task Creation

The **Autonomous Task Creation** feature allows the AI Agent to determine when a follow-up task should be created for staff.

This feature applies to automation-triggered conversations only and does not operate in Test Chat.

* Enable / Disable - Turn Autonomous Task Creation on or off.
* Instructions - Configure when the AI Agent should create a follow-up task.

## 5. Data Collection

The **Data Collection** feature allows the AI Agent to ask customers specific questions and automatically save their answers throughout the conversation.

* Enable / Disable - Turn Data Collection on or off.
* Questions - Configure the questions that the AI Agent should ask customers.
* Answer Collection - Automatically save customer answers collected during the conversation.

This feature applies to automation-triggered conversations only and does not operate in Test Chat.

## 6. **Appointment Booking**

The **Appointment Booking** feature allows the AI Agent to check available calendar slots and book appointments for customers during conversations.

<figure><img src="../../.gitbook/assets/ai (4).png" alt=""><figcaption></figcaption></figure>

* Enable / Disable - Turn Appointment Booking on or off.
* Calendar Availability - Allow the AI Agent to check available calendar slots.
* Appointment Booking - Allow the AI Agent to book appointments for customers during the conversation.

This feature applies to automation-triggered conversations only and does not operate in Test Chat.

## 7. Handover to Human

The **Handover to Human** feature allows the AI Agent to transfer a conversation to a human agent when additional assistance is required.

When this feature is triggered, the system can:

* Hand the conversation over to a human agent.
* Assign the conversation.
* Stop further AI replies.
* Send an email notification to the team.

Users can enable or disable this feature depending on their customer support requirements.

## 8. Creating the AI Agent

Once all required configurations are completed:

1. Enter the AI Agent's name under **Basic Information**.
2. Configure the AI Agent's persona and instructions.
3. Set the confidence threshold and fallback message.
4. Configure additional response settings as required.
5. Enable any relevant autonomous features.
6. Review the AI Agent's configuration.
7. Click **Create agent** to save.

> **Important:** The AI Agent cannot be created until the required fields are completed. The system will highlight missing information, such as the Agent Name or Fallback Message, before allowing users to proceed.

Once created, the AI Agent will appear in the **AI Agents** dashboard, where users can view its status, confidence threshold, creation date, and available management actions.
