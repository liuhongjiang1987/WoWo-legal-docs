---
layout: default
title: Privacy Policy - WoWo
---

# Privacy Policy

**Last updated: February 2025**

WoWo ("we," "our," or "us") is committed to protecting your privacy. This Privacy Policy explains what data we collect, how we use it, where we store it, and your rights regarding your information when you use the WoWo Chrome extension ("Extension").

**Definitions**: "Personal data" means information that identifies or can reasonably be linked to you. "Aggregated or de-identified data" means data that has been processed so that it cannot reasonably identify you (e.g., statistical summaries, anonymized analytics).

---

## 1. Data We Collect

### 1.1 Account Information

When you sign in, we receive:

| Data | Source | Purpose |
|------|--------|--------|
| Email address | Google OAuth or email OTP | Account identification, authentication |
| Name / Display name | Google OAuth | Display in the Extension (e.g., popup header) |
| Profile picture | Google OAuth | Display as avatar in the Extension |

If you sign in with email OTP only (without Google), we receive only your email address.

### 1.2 Page and Bookmark Data

To provide AI-powered bookmark recommendations, we collect:

| Data | Description | When |
|------|-------------|------|
| **Current page info** | Page title, URL, and meta description (from `meta[name="description"]`) of the tab you are viewing | When you trigger analysis by clicking the Extension icon |
| **Bookmark structure** | Your bookmark folder tree (folder names and hierarchy) | When you trigger analysis |
| **Bookmark samples** | Up to **4 bookmarks per folder** (title and URL only) — we intentionally limit this to minimize data transfer and protect privacy | When you trigger analysis |

We do **not** collect your full bookmark list. We use a pruned structure so the AI can infer your organization preferences while keeping the amount of data sent to a minimum.

### 1.3 Analysis and Usage Data

| Data | Description |
|------|-------------|
| Pending analysis results | AI-recommended folder, your confirmations or rejections, and (if you confirm) the final bookmark location |
| Snapshot data | A pruned copy of your bookmark structure at the time of analysis, stored to support the recommendation and for potential future features (e.g., rollback) |
| LLM usage metrics | Token counts for AI calls (for cost and performance monitoring; not linked to your identity beyond your account) |

---

## 2. How We Use Your Data

We use the data described above to:

- **Provide the Service**: Analyze pages, recommend folders, and add bookmarks where you confirm
- **Authenticate you**: Verify your identity when you sign in
- **Improve the Service**: Monitor performance, debug issues, and optimize the AI pipeline
- **Comply with legal obligations**: Where required by law

We do **not** sell your personal data to third parties. We do **not** share your personal data with third parties for targeted advertising or third-party marketing. We may use aggregated or de-identified data for analytics, product improvement, or other lawful purposes.

We may update our data practices from time to time. Material changes will be disclosed in an updated policy. Where required by applicable law, we will obtain your consent before using your personal data for substantively new purposes.

---

## 3. Where We Store Your Data

### 3.1 Local Storage (Your Device)

The Extension uses Chrome's local storage (`chrome.storage.local`) to store:

- Session and authentication tokens
- Cached tab information (title, URL) for recently viewed tabs (up to 10)
- Cached bookmark folder structure
- Pending analysis results (as a fallback when the server is unavailable)

This data stays on your device and is not sent to our servers except as needed for the Service (e.g., when you trigger analysis).

### 3.2 Our Servers (Supabase)

We use [Supabase](https://supabase.com) to store:

- **Authentication data**: Managed by Supabase Auth (email, OAuth tokens)
- **Pending analyses**: Page URL, title, description, recommended folder, your confirmations, and related metadata
- **Bookmark snapshots**: Pruned bookmark structure (folder tree + up to 4 bookmarks per folder) at the time of each analysis

Supabase stores data in secure data centers. To the extent permitted by applicable law, we do not physically delete analysis records; we mark them as "confirmed" or "discarded" for audit and potential future features (e.g., rollback). You may request deletion of your personal data (see Section 7).

---

## 4. Third-Party Services

We use the following third parties to operate the Extension:

| Service | Purpose | Data shared |
|---------|---------|-------------|
| **Supabase** | Authentication, database, hosting | Account info, page info, bookmark structure (pruned), analysis results |
| **Google** | Sign-in (OAuth) | Email, name, profile picture (only if you choose Google sign-in) |
| **SiliconFlow** | AI/LLM for folder recommendations | Page title, URL, description, pruned bookmark structure |

Each of these services has its own privacy policy. We encourage you to review them:

- [Supabase Privacy Policy](https://supabase.com/privacy)
- [Google Privacy Policy](https://policies.google.com/privacy)
- [SiliconFlow](https://siliconflow.cn/) — please refer to their website for their privacy practices

---

## 5. Data Retention

- **Account data**: Retained while your account is active. You may request deletion (see Section 7).
- **Analysis records**: To the extent permitted by applicable law, we retain analysis records (including snapshots) with state markers (pending, confirmed, discarded) and do not physically delete them for audit and potential rollback features.
- **Local storage**: Cleared when you uninstall the Extension or clear extension data.

---

## 6. Data Security

We implement reasonable technical and organizational measures to protect your data, including:

- Use of HTTPS for all communications
- Secure authentication (OAuth, OTP)
- Access controls and encryption where applicable

However, no method of transmission or storage is 100% secure. We cannot guarantee absolute security.

---

## 7. Your Rights

Depending on your jurisdiction, you may have the right to:

- **Access**: Request a copy of the personal data we hold about you
- **Correction**: Request correction of inaccurate data
- **Deletion**: Request deletion of your data (subject to legal retention requirements)
- **Portability**: Request your data in a portable format (to the extent technically feasible)
- **Object or restrict processing**: Object to or request restriction of certain processing
- **Withdraw consent**: Where processing is based on consent, withdraw it at any time

To exercise these rights, contact us through the feedback channel in the Extension or via the project repository. We will respond within the timeframes required by applicable law, to the extent technically feasible.

You may also uninstall the Extension at any time to stop further data collection. Note that data already stored on our servers may remain until you request deletion.

---

## 8. Children's Privacy

The Extension is not intended for users under 13 years of age (or the applicable minimum age in your jurisdiction). We do not knowingly collect personal data from children. If we become aware that we have inadvertently collected data from a child, we will take steps to delete it promptly. If you believe we have collected data from a child, please contact us.

---

## 9. International Transfers

Your data may be processed in jurisdictions other than your own (e.g., Supabase and SiliconFlow may use servers in different countries). By using the Extension, you consent to such transfers. We take steps to ensure appropriate safeguards are in place where required by law.

---

## 10. Changes to This Policy

We may update this Privacy Policy from time to time. We will notify you of material changes by posting the updated policy at this URL and updating the "Last updated" date. Your continued use of the Extension after such changes constitutes acceptance of the revised policy.

For significant changes, we may provide additional notice (e.g., within the Extension). Where required by applicable law, we will obtain your consent before applying materially different data practices to your existing personal data.

---

## 11. Contact

If you have questions about this Privacy Policy or our data practices, please contact us through the feedback channel provided in the Extension or via the repository associated with this project.

---

*By using WoWo, you acknowledge that you have read and understood this Privacy Policy.*
