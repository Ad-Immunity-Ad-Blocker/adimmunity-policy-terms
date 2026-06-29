# AdImmunity Privacy Policy

**Last updated:** 28 June 2026

*The current version of this policy is published at*  
https://omarayman23.github.io/adimmunity-legal/privacy.html  
*and is linked from the Chrome Web Store listing and from within the extension.*

---

# 1. Who We Are / Contact

AdImmunity is a Chrome browser extension that blocks ads, trackers, and phishing attempts. It is developed and maintained by an independent maker based in the United States.

If you have any questions or requests regarding this Privacy Policy or your personal data, please contact:

**Email:** omiteyt@gmail.com

We will respond to all privacy-related enquiries within a reasonable time, and no later than 30 days where required under applicable data protection law.

---

# 2. Summary

AdImmunity is built with a privacy-first design.

The extension performs all ad and tracker blocking locally on your device using Chrome's `declarativeNetRequest` API and content scripts. Your browsing activity never leaves your device as part of normal extension operation.

Creating an account is **completely optional**. Every blocking and filtering feature works without an account or providing any personal information.

An account is only required if you wish to sync settings or use future authenticated features.

Optional anonymous diagnostics are also available, but they are:

- **Off by default**
- Enabled only after you explicitly opt in
- Disabled at any time from Settings

---

# 3. What Stays on Your Device

AdImmunity relies exclusively on local browser storage for its core functionality.

The following information is stored in `chrome.storage.local` and **is never transmitted to any server**:

- **Blocking statistics** — counts of ads, trackers, and phishing attempts blocked.
- **Extension settings** — your preferences and blocking configuration.
- **Whitelist (allowlist)** — domains or pages you choose to exclude.
- **Element Zapper rules** — your custom element hiding rules.

This information remains entirely on your device.

It is not uploaded, synchronized, or accessible to us unless you choose to use an optional future synchronization feature, which would be disclosed in an updated Privacy Policy.

The blocking engine works using Chrome's `declarativeNetRequest` API. We do **not** intercept, log, or store:

- URLs you visit
- Network requests
- Browsing history
- Any browsing data

### Anonymous Tool

The optional **Anonymous** feature simply opens the current page inside Chrome's Incognito mode.

It:

- Uses Chrome's built-in Incognito feature
- Sends nothing to us
- Records nothing
- Does not transmit URLs or page content

Incognito mode does **not** make you anonymous to websites, your ISP, or your network.

---

# 4. Data We Collect with an Optional Account

Creating an account is completely optional.

If you choose to create one, we collect:

- **Email address**
  - Used only for authentication.
  - Stored securely in Supabase Auth.

- **Password**
  - Sent over HTTPS.
  - Stored only as a salted hash by Supabase.
  - The extension never stores your raw password.
  - Only temporary session tokens are stored locally.

We **do not** collect:

- Name
- Phone number
- Payment information
- Any other personal details

Your email is never:

- Used for marketing
- Sold
- Shared for advertising
- Combined with browsing data

You may permanently delete your account at any time using the **Delete account** button inside the extension.

---

# 5. Optional Anonymous Diagnostics

AdImmunity includes an optional diagnostics feature to help identify software bugs.

This feature is:

- Off by default
- Entirely optional
- Enabled only after you opt in

When enabled, diagnostic reports may include:

- Error signature (hash)
- Truncated stack trace
- Extension version
- Browser version
- Operating system version

## Diagnostics Never Include

- URLs
- Page content
- HTML
- Email address
- Account identifiers
- Browsing history
- Search queries
- Passwords
- Credentials
- Local extension storage
- Settings
- Whitelist
- Zapper rules

Diagnostic reports cannot identify you personally.

You may disable diagnostics at any time.

---

# 6. What We Never Collect

Regardless of whether you create an account or enable diagnostics, AdImmunity **never** collects:

- Browsing history
- URLs visited
- Webpage content
- Search queries
- Browsing behavior analytics
- Persistent identifiers tied to browsing
- Location data
- Financial or payment information

We have no technical capability to collect this information.

---

# 7. Processor & Data Location

We use **Supabase** as our authentication and database provider.

Account data is stored in:

**European Union**  
**Frankfurt, Germany (eu-central-1)**

Supabase acts solely as our data processor under a Data Processing Agreement.

Supabase:

- Does not use your data for its own purposes
- Does not sell your data

More information:

https://supabase.com/security

If diagnostics are enabled, anonymous diagnostic reports are stored in the same EU region.

---

# 8. Legal Bases (GDPR Article 6)

For users in the EEA, UK, and Switzerland, we process personal data only when a lawful basis exists.

We rely solely on:

**Consent (Article 6(1)(a))**

Consent applies to:

- Creating an account
- Enabling diagnostics

You may withdraw consent at any time.

We do **not** rely on legitimate interests or process special category data under Article 9 GDPR.

---

# 9. Your GDPR Rights

If you are located in the EEA, UK, or Switzerland, you have the right to:

- Access your personal data
- Correct inaccurate data
- Delete your data ("right to be forgotten")
- Receive your data in a portable format
- Withdraw consent
- Lodge a complaint with your supervisory authority

You may also delete your account using the **Delete account** button within the extension.

For requests, contact:

**omiteyt@gmail.com**

We normally respond within one month.

---

# 10. California Privacy Rights (CCPA / CPRA)

California residents have the right to:

- Know what personal information we collect
- Request deletion
- Receive equal service without discrimination

You may request deletion by:

- Using the Delete Account feature
- Contacting us at **omiteyt@gmail.com**

## No Sale or Sharing

AdImmunity:

- Does **not** sell personal information.
- Does **not** share personal information for cross-context behavioral advertising.

Therefore, no sale/sharing opt-out is required.

---

# 11. Data Retention

### Account Data

Your email address is retained only while your account exists.

Deleting your account permanently removes it from Supabase Auth.

### Anonymous Diagnostics

- Raw reports are retained for **no more than 90 days**.
- Aggregated anonymous statistics may be retained longer.

### Local Device Data

Your:

- Settings
- Statistics
- Whitelist
- Zapper Rules

remain only on your device until:

- You uninstall the extension
- You clear browser storage

We cannot delete this information because we never receive it.

---

# 12. Children

AdImmunity is not intended for children.

You must be at least **16 years old** to:

- Create an account
- Enable diagnostics

If we learn that someone under 16 has provided personal information, we will promptly delete it.

---

# 13. Changes to This Policy

We may update this Privacy Policy to reflect:

- New features
- Legal changes
- Changes to our data practices

When material changes occur, we will:

- Update the **Last updated** date
- Notify users within the extension where practical

Continued use of AdImmunity after an update constitutes acceptance of the revised policy, subject to applicable legal rights.

The version history of this document is available in the public GitHub repository.

---

**Last updated:** 28 June 2026

---

*AdImmunity — Privacy-first ad & tracker blocking.*

**Contact:** omiteyt@gmail.com
