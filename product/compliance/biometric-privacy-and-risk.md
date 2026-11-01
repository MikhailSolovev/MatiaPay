# Biometric Privacy, Payments Compliance and Risk

Product-side checklist. This is not legal advice: every item marked *confirm* needs sign-off from legal / compliance before launch.

## Launch region(s)

TBD — determines which of the regimes below apply.

## Regulatory checklist

| Area | Question | Owner | Status |
|---|---|---|---|
| Biometric data law (e.g. GDPR special-category data, Illinois BIPA, other local law) | Which apply in our regions, and what do they require? *confirm* | TBD | open |
| Payment authentication (e.g. PSD2 strong customer authentication) | Does a face match count as an authentication factor, and which one? *confirm* | TBD | open |
| Card scheme / PCI DSS | What is our scope if we store or tokenise payment methods? *confirm* | TBD | open |
| Financial licensing (KYC/AML) | Do we need a licence or a licensed partner? *confirm* | TBD | open |

## Consent and data handling

- **Consent:** explicit, separate from terms of service, easy to withdraw. Wording: TBD
- **What we store:** face template vs. raw image — default to template only, raw images discarded. Decision: TBD
- **Retention and deletion:** TBD; a user can delete their face data at any time
- **Access and encryption:** TBD
- **Minors / people who cannot consent:** TBD

## Fraud and abuse risks

| Risk | Example | Mitigation | Status |
|---|---|---|---|
| Spoofing | Photo, video or mask presented to the camera | Liveness detection | open |
| Look-alikes / false accepts | Wrong person charged | Match threshold, amount limits, step-up | open |
| Template breach | Stolen face templates cannot be rotated like a password | Encryption, separate storage, breach plan | open |
| Account takeover at enrolment | Attacker enrols their face on a victim's account | Verify identity and payment method at enrolment | open |
| Bias | Accuracy differs across demographic groups | Measure per group before launch | open |

## Pre-release gate

A release that changes face capture, matching, storage or payment authorisation needs: this file reviewed, the checklist above current, and legal sign-off recorded in [decisions](../decisions/).
