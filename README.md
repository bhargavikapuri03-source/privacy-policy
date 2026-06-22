# privacy-policy for AI Email Reply generator

**Last updated:** 22 JUNE 2026

We operates AI Email Reply generator, an application that helps users draft email replies using
artificial intelligence. This policy explains what information we collect,
how we use it, and the choices you have.

### 1. Information We Collect

**Account information.** When you sign in with Google, we receive your
Google account email address and a unique Google account identifier. **We
never request, see, or store your Google password.**

**Gmail access.** With your explicit consent via Google's OAuth screen, we
access:

- Your email messages (read-only) — to display your inbox and let you
  select an email to reply to
- The ability to send email on your behalf — only when you click "Send"
  after reviewing and optionally editing an AI-generated draft

We request the minimum necessary Gmail permissions (`gmail.readonly` and
`gmail.send`) — not full account access.

**Email content sent to our AI provider.** When you select an email and
request a generated reply, the text of that email is sent to OpenAI
(our AI provider) to analyze tone/intent and draft a response. [State
whether email content is stored by you beyond this — in the reference
implementation, it is not persisted to our database; it is processed
in-memory per request only.]

**Usage data.** We log aggregate metrics about your use of AI features
(token counts, estimated cost, timestamps, which feature was used) to
monitor system health and costs. This log does not include the content of
your emails.

**2FA data.** If you enable two-factor authentication, we store an
encrypted TOTP secret used to verify your authenticator app codes.

### 2. How We Use Your Information

- To authenticate you and maintain your session
- To display your inbox and individual email content to you
- To generate AI-drafted replies based on email content you select
- To send replies you've reviewed and approved, on your behalf
- To monitor and limit AI usage costs
- To maintain and improve the security and reliability of the Service

We do **not** use your email content to train AI models, and we do **not**
sell your data to third parties.

### 3. How We Protect Your Information

- OAuth tokens are encrypted at rest using industry-standard encryption
  (AES via Fernet) and are never stored in plaintext.
- We never store your Google account password — authentication is handled
  entirely by Google.
- All data in transit is encrypted via HTTPS/TLS.
- Access to production systems and databases is restricted to authorized
  personnel only.

### 4. Third-Party Services

We share data with the following third parties, only as necessary to
provide the Service:

| Provider                | Purpose                               | Data shared                          |
| ----------------------- | ------------------------------------- | ------------------------------------ |
| Google (Gmail API)      | Read/send email on your behalf        | OAuth-scoped Gmail access            |
| OpenAI                  | Generate AI replies and tone analysis | Text content of the email you select |
| Hosting provider        | Application hosting                   | Encrypted database contents          |

### 5. Data Retention

- Account and OAuth token data is retained until you delete your account or
  revoke access.
- Usage logs are retained for 2 months for cost-monitoring purposes.
- Email content itself is **not** persisted to our database — it is fetched
  from Gmail and processed transiently per request. 

### 6. Your Rights

You can:

- **Revoke access** at any time via your
  [Google Account permissions page](https://myaccount.google.com/permissions),
  which immediately invalidates our stored tokens.
- **Request deletion** of your account and all associated data by
  [contacting us at email/contact method, or via an in-app delete-account option].
- **Request a copy** of the data we hold about you.

Residents of the EU/EEA have rights under GDPR including access,
rectification, erasure, and data portability. Residents of California have
rights under the CCPA/CPRA including the right to know, delete, and opt out
of the sale of personal information (we do not sell personal information).

### 7. Children's Privacy

This Service is not directed to individuals under 16, and we do not
knowingly collect data from children.

### 8. Changes to This Policy

We may update this policy from time to time. We will post the updated
version here with a revised "Last updated" date, and notify users of
material changes via [email/in-app notice].

### 9. Contact Us

Questions about this policy or your data? Contact us at:
bhargavikapuri03@gmail.com

