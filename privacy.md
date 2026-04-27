---
layout: default
title: Privacy Policy
permalink: /privacy
---

# Privacy Policy

**Effective date:** April 20, 2026

This Privacy Policy describes how Ghostnote Labs LLC ("we," "us," "Ghostnote Labs") collects, uses, and handles information when you use our mobile application ("the App").

The App is currently in **private Alpha testing** with a small cohort under non-disclosure agreement. This policy applies to that Alpha test. We will publish a revised policy if and when the App moves to public release.

---

## 1. Who we are

Ghostnote Labs LLC is an Oregon limited liability company.

- **Company:** Ghostnote Labs LLC
- **Oregon Registry:** #255831597
- **Contact:** ghostnotelabsllc@gmail.com

---

## 2. Information the App accesses

### 2.1 Health and fitness data (read-only)

The App reads workout data from your device's Health Connect platform. We **never write** data to Health Connect. The data fields we read are:

- Exercise session records (activity type, start time, duration)
- Distance records (for distance-based activities)
- Heart rate records (where available)
- Step counts
- Total calories burned

This data is read on your device and used exclusively to compute in-game progression. **It is stored locally on your device only.** It is never transmitted to our servers (we do not currently operate any servers for the App), uploaded to any cloud service, or shared with any third party except as described in §3.

You can revoke the App's Health Connect permission at any time through your device's Settings → Apps → Health Connect → App permissions.

### 2.2 Conversations with our AI familiar

The App includes a conversational AI familiar character, powered by an external AI service (see §3). When you send a message to the familiar:

- Your message is sent to the AI service for processing.
- The reply is returned to your device and displayed.
- Both your message and the reply are stored locally on your device for conversation history.

**No conversation data is stored on our servers** (we do not operate any). The AI service receives the messages as part of providing a response and processes them per the AI service's own privacy policy (see §3).

### 2.3 Survey responses (Alpha only)

During Alpha testing, we collect feedback responses through Google Forms. Survey responses are stored in Google Workspace under the Ghostnote Labs account. Responses are tied to your tester identity (so we can correlate with interview notes) but are not shared publicly. See §4 for retention.

### 2.4 Anonymous usage telemetry (Alpha only)

To understand how the App is being used during Alpha — whether the post-workout reveal feels rewarding enough that you come back, where the experience drags or surprises, whether the AI familiar is being used at all — the App sends anonymous usage events to our backend.

What is captured:

- An anonymous, randomly-generated install identifier — created the first time you open the App and stored only on your device. Not tied to your name, email, account, or any device-identifying ID.
- A per-launch session identifier (also random).
- Event type and timing for these specific moments: app open, post-workout reveal start / completion, level-up crossings, AI familiar message exchanges (count and length only), screen views.
- Numeric properties of those events — durations in milliseconds, character counts of messages sent and received, the level number crossed, the in-game thread name.

What is **not** captured:

- We never capture the **content** of your messages with the AI familiar (only how long they are).
- We never capture **values** from your workouts (no heart rate numbers, no distances, no calorie counts, no workout type, no health metrics of any kind).
- No personally identifiable information ever leaves the device through this channel.

Telemetry events are stored in our backend (AWS DynamoDB, region us-west-2) for 90 days, then automatically deleted. They are used solely for understanding Alpha-cohort engagement and are never sold, shared, or used for advertising.

### 2.5 What we do NOT collect

- We do not collect advertising identifiers.
- We do not run third-party analytics platforms (no Firebase Analytics, no Mixpanel, no Google Analytics).
- We do not collect location data beyond what Health Connect surfaces from your workouts.
- We do not collect contacts, photos, or messages outside the App.
- The App contains no advertising.

---

## 3. Subprocessors and third-party services

### 3.1 Anthropic (Claude AI service)

The App uses Anthropic's Claude API to power the familiar's conversational responses. When you send a message to the AI familiar:

- Your message text is transmitted to Anthropic's API endpoints.
- Anthropic processes the message and returns a response.
- Anthropic's processing is governed by their privacy policy: https://www.anthropic.com/legal/privacy

We pass Anthropic the minimum information needed to generate a response (your message + a system prompt describing the familiar's character and game context). We do not pass your real name, contact information, or health data to Anthropic.

### 3.2 Google (Health Connect, Play Store, Google Forms)

- **Health Connect** is provided by Google as part of Android. Your health data is governed by Google's Health Connect privacy practices.
- **Google Play Store** distributes the App. Your interaction with the Play Store is governed by Google's policies.
- **Google Forms** hosts the Alpha feedback survey. Your survey responses are stored in Google Workspace; Google's privacy policy applies to that storage.

---

## 4. Data retention

- **Local app data** (workouts, conversation history, in-game progression): retained on your device until you uninstall the App or clear app data through your device settings. Uninstalling the App deletes all locally stored data.
- **Survey responses**: retained for the duration of the Alpha test plus six months for analysis, then deleted from Google Workspace storage. Aggregate, non-identifying insights derived from survey responses (e.g. average ratings, common themes) may be retained indefinitely.
- **Interview notes**: retained for the duration of the Alpha test plus six months, then deleted.
- **Anonymous usage telemetry**: retained in our backend for 90 days from the event timestamp, then automatically deleted via DynamoDB time-to-live. We do not connect telemetry events to your identity (no real name, email, or device ID), so deletion-by-request applies to the anonymous install identifier rather than to "you" specifically — emailing ghostnotelabsllc@gmail.com with your install identifier (visible in a future settings screen) will purge the events tied to it within 7 days.

You may request deletion of your survey responses and interview notes at any time by emailing ghostnotelabsllc@gmail.com.

---

## 5. Your choices

- **Health permissions:** revoke at any time through your device Settings.
- **Local data:** clear by uninstalling the App or via Settings → Apps → [the App] → Storage → Clear data.
- **AI familiar chat:** simply do not use the chat feature; no message means no transmission to Anthropic.
- **Anonymous usage telemetry:** opt out via the App's settings (forthcoming). Until the in-app toggle ships, you may email ghostnotelabsllc@gmail.com to be excluded from telemetry collection on your install.
- **Survey responses:** request deletion by email to ghostnotelabsllc@gmail.com.

---

## 6. Children

The App is not intended for use by anyone under 13. We do not knowingly collect information from children under 13. If you believe a child under 13 has used the App, please contact us at ghostnotelabsllc@gmail.com and we will take appropriate action.

For users in the European Economic Area, United Kingdom, or other jurisdictions with a higher age of digital consent (typically 16): the App is not intended for use by anyone under that age without parental consent.

---

## 7. Security

We do not currently store user data on servers we operate. Local-only storage means data security depends primarily on the security of your device. Use a strong device lock, keep your operating system updated, and only install apps from trusted sources.

For data transmitted to third-party services (Anthropic, Google), we rely on those services' security practices as described in their respective policies.

---

## 8. Changes to this Privacy Policy

We may update this Privacy Policy as the App evolves. If we make material changes, we will notify Alpha testers by email and update the effective date at the top of this document. Continued use of the App after a change indicates acceptance.

---

## 9. Contact

Questions about this Privacy Policy or your data:

- Email: ghostnotelabsllc@gmail.com

---

*This Privacy Policy is governed by the laws of the State of Oregon, USA.*
