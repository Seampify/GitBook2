# Alias Login

The **Alias Login** feature allows Seampify's support team to temporarily access your organization as one of your users without requiring your account password.

This feature is designed to assist with troubleshooting and technical support while maintaining account security.

## Accessing Alias Login

1. Log in to your Seampify account.
2. Navigate to **Settings → Alias Login**.
3. The Alias Login settings page will be displayed.

<figure><img src="../../../.gitbook/assets/alias login.png" alt=""><figcaption></figcaption></figure>

## Allow Alias Login

The **Allow alias login** setting controls whether your reseller's support team can temporarily access your organization.

* Enabled - Allows Seampify's support team to initiate temporary access sessions for troubleshooting.
* Disabled - Prevents Seampify's support team from initiating alias login sessions for your organization.

To enable or disable Alias Login, toggle the setting and click Save changes.

## Security Restrictions

Alias Login includes the following security measures:

| **Security Feature** | **Description**                                                                      |
| -------------------- | ------------------------------------------------------------------------------------ |
| Password-Free Access | Support personnel can access the organization without requiring the user's password. |
| Session Duration     | Each session is limited to 30 minutes.                                               |
| IP-Pinned Sessions   | Sessions are restricted to the IP address associated with the session.               |
| Session Revocation   | Active sessions can be revoked immediately.                                          |
| Restricted Settings  | Certain sensitive account and organization settings remain inaccessible.             |

### Always Blocked Actions

For security purposes, the following actions are always blocked during an Alias Login session:

* Password changes
* Email changes
* Two-factor authentication
* Team Members
* Roles & Permissions
* Alias Login settings

These restrictions help prevent support personnel from making sensitive account or permission changes.

## Active Sessions

The **Active sessions** section displays whether anyone is currently accessing your organization through Alias Login.

If there are no active sessions, the system displays:

> No one is currently accessing your organization.

Users can monitor active access sessions and revoke them when necessary.

{% hint style="info" %}
**Note:** Alias Login is optional and can be disabled when support access is not required.
{% endhint %}
