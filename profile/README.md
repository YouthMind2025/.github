<div align="center">

# Youniverse by YouthMind

### A calmer place to share, reflect, and feel understood.

An iOS community and AI companion designed for everyday emotional support.

**Private beta** · **Built for iOS** · **Production hardening in progress**

[Product](#the-product) · [Experience](#inside-youniverse) · [Engineering](#built-as-a-complete-system) · [Status](#current-status)

</div>

---

## Launch film

<p align="center">
  <a href="https://youthmind2025.github.io/.github/">
    <img src="assets/youthmind-launch-preview.gif" alt="Animated preview of the Youniverse launch film" width="420">
  </a>
</p>

<p align="center">
  <strong><a href="https://youthmind2025.github.io/.github/">▶ Watch “Fine. Take 47.”</a></strong><br>
  <sub>30 seconds · sound on · private-beta campaign film</sub>
</p>

## The product

Youniverse combines an anonymous, emotion-aware community with **Aura**, an AI
companion for thoughtful, ongoing conversations. It is designed around four
simple ideas:

| Share | Discover | Talk | Reflect |
| :---: | :---: | :---: | :---: |
| Express what is on your mind without public popularity pressure. | Find experiences across a genuine range of emotions. | Continue streamed conversations with clear consent and history. | Revisit saved moments, themes, and personal activity. |

> [!IMPORTANT]
> Youniverse supports general wellbeing and peer connection. It is not a medical
> device, diagnostic product, emergency service, or replacement for professional care.

## Inside Youniverse

<table>
  <tr>
    <td width="33%" align="center"><img src="assets/app-feed.jpeg" alt="Youniverse community feed" width="230"><br><strong>Emotion-aware discovery</strong><br><sub>A varied feed shaped by relevance, freshness, safety, and diversity.</sub></td>
    <td width="33%" align="center"><img src="assets/app-aura-home.jpeg" alt="Aura AI companion home" width="230"><br><strong>Aura conversations</strong><br><sub>Streaming chat with visible history and user-controlled memory.</sub></td>
    <td width="33%" align="center"><img src="assets/app-activity.jpeg" alt="Youniverse resonance activity" width="230"><br><strong>Human resonance</strong><br><sub>Supportive activity without a public popularity scorecard.</sub></td>
  </tr>
  <tr>
    <td width="33%" align="center"><img src="assets/app-profile.jpeg" alt="Youniverse personal profile" width="230"><br><strong>Personal reflection</strong><br><sub>Activity-backed themes and evolving, non-clinical reflections.</sub></td>
    <td width="33%" align="center"><img src="assets/app-saved.jpeg" alt="Youniverse saved posts" width="230"><br><strong>Keep what matters</strong><br><sub>Return to posts that helped, inspired, or felt familiar.</sub></td>
    <td width="33%" align="center"><img src="assets/app-aura-history.jpeg" alt="Aura conversation history" width="230"><br><strong>Continue naturally</strong><br><sub>Conversation summaries make the right thread easy to find.</sub></td>
  </tr>
</table>

<p align="center"><sub>Real simulator captures from a synthetic Staging QA account. No real user data is shown.</sub></p>

## Built as a complete system

```mermaid
flowchart LR
    IOS[iOS · SwiftUI] -->|HTTPS + SSE| API[Spring Boot API]
    OPS[Operations console] --> API
    API --> PG[(PostgreSQL)]
    API --> REDIS[(Redis)]
    API --> QDRANT[(Qdrant)]
    API --> AI[AI provider]
    API --> SAFETY[Moderation + safety operations]
```

| Layer | Responsibility |
| --- | --- |
| **iOS experience** | Product flows, secure sessions, resilient networking, and offline-aware state. |
| **Product API** | Authentication, community, recommendation, chat, memory, privacy, and moderation. |
| **Data systems** | PostgreSQL as system of record, Redis for coordination, and opt-in Qdrant retrieval. |
| **Quality system** | Contract tests, UI journeys, load scenarios, observability, recovery, and release gates. |

Our recommendation pipeline separates candidate sourcing, eligibility, scoring,
reranking, hydration, and exposure logging. Aura combines durable conversations,
streaming responses, opt-in semantic recall, consent controls, and explicit
safety boundaries.

## How we work

- **Privacy before personalization** — consent, minimization, deletion, and clear data boundaries.
- **Evidence before claims** — local tests, CI, staging, recovery, and production are kept distinct.
- **Safety by design** — reporting, blocking, moderation, crisis boundaries, and human escalation.
- **Calm product craft** — expressive interaction without engagement pressure or clinical overclaiming.

Organization-wide contribution, security, and support guidance lives in this
repository. Product source remains private while beta and launch gates are completed.

## Current status

Youniverse is in **private beta and production hardening**. We are validating
real user journeys, recommendation quality, AI reliability, privacy controls,
moderation operations, recovery procedures, and regional launch requirements.

Public launch is gated on accountable legal, clinical-safety, privacy,
credential-rotation, backup-recovery, and app-store approvals. Passing tests or
a healthy deployment is not presented as proof that those external gates are complete.

---

<p align="center"><strong>SwiftUI · Spring Boot · PostgreSQL · Redis · Qdrant</strong><br><sub>© 2026 YouthMind · Technology for more human connection.</sub></p>
