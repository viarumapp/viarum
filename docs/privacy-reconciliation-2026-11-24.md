# VIARUM privacy reconciliation website candidate

**Implementation date: November 24, 2026**

**Status: approved for implementation; unpublished review candidate**

## Scope and approval

The owner approved inputting the reviewed privacy reconciliation changes. This
branch applies the reviewed replacement website policy and companion support
copy for inspection. That implementation approval does not authorize publication,
merging into the website's publishing branch, an App Store privacy declaration,
or an app release. The publication gates below remain open.

The website baseline is `viarumapp/viarum` at
`526ae494252ef2f3b6f462b70efaf6be4404370f`. The reviewed app source is
`viarumapp/rork-viarum` at `f39fff57a8a4629b99fcc31d92e7b9d529dd2b84`.
Its tree is identical to the audited parent `aedf88c2456e41016e337295b775f185829fbe07`.
The latest commit records a build 127 upload; its message does not independently
establish the contents of that build or any submitted archive.

The starting reference is the
[November 22 privacy proposal](https://github.com/viarumapp/rork-viarum/blob/f39fff57a8a4629b99fcc31d92e7b9d529dd2b84/docs/privacy-policy-update-proposal-2026-11-22.md),
reconciled against the November 24 source and the reviewed approval packet.

## Changes included

- `privacy.html`: the reviewed replacement copy covering All Access, Workshop
  still images and local speech transcription, local documents, online trip and
  memory data, location, providers, retention, exports and deletion limits.
  The unpublished-review banner, draft title and `noindex,nofollow` metadata
  are intentionally retained. There is no new policy effective date.
- `support.html`: the existing subscription section now covers VIARUM+ and All
  Access, restoration, Apple subscription management, the distinction between
  account deletion and billing cancellation, and separate Stripe rally-payment
  support. The existing Apple refund link and section anchor remain available.
- This record documents implementation scope and outstanding publication gates.

The black-and-gold design, repaired mark, existing responsive stylesheet,
navigation, footer, worldwide positioning, slogan and destination links are
preserved. No changes are made to `legal.css`, Terms of Service or brand assets.

## Publication gates retained

| Gate | Evidence still required before publication |
| --- | --- |
| B1. Runtime AI/provider handling | Identify the production endpoints, recipients, intermediaries/fallbacks and governing end-user processing terms. Verify the upstream AI product/tier, permitted inputs, training/human access, logging/caching, retention, deletion, regions and safeguards, including relevant age/region restrictions. Public provider documentation alone does not verify VIARUM's settings. |
| B2. Complete account deletion | Verify an approved implementation for ordinary, paid-rally and organizer accounts, relevant authentication/session revocation, processor erasure, lawful retained records and partial-failure recovery. The reviewed `rally_orders` profile restriction and missing Rork identity-deletion path are source risks, not observed production failures. |
| B3. Chat/media retention and deployment | Verify deployed Worker/handler versions, legacy-chat cleanup inventory and flag, media-object cleanup, erasure-marker purpose/retention and provider/CDN/backup behavior. Hiding an item is not proof of physical erasure. |
| B4. Retention and privacy-rights operation | Approve and implement category-specific durations or objective criteria, deletion ownership/jobs, backup expiry, lawful exceptions and access/erasure response and completion procedures. Incorporate verified outcomes into the public wording. |
| B5. Candidate archive and App Store baseline | Obtain the actual candidate build/source mapping, resolved SDK dependencies, aggregated privacy manifests and existing App Store Connect answers. Resolve conditional audio, search-history, hosted payment/contact, crash/performance and tracking disclosures for all distributed platforms and versions. |
| B6. Native notices and policy alignment | Verify companion app text and translations, device-scoped AI controls and relevant notices. Establish consent coverage for other participants whose names or rally details may enter an AI request, or remove/minimize that information. The requester's approval alone does not establish permission from everyone represented. |
| B7. Operator and business attestations | Confirm the responsible operator's public identity/contact details, applicable regional rights/transfer notices and contractual safeguards. Verify business/provider practices before restoring any categorical no-sale or no-cross-company-ad-tracking claim. |

This website change does not close any gate merely by describing a limitation.
Once evidence is available, update the copy to match the verified behavior and
obtain approval of the exact publication version. Keep this candidate out of the
publishing branch until publication is expressly authorized.

## App Store boundary

The reconciliation packet contains proposed App Store classifications, not a
record of existing App Store Connect answers and not final certified
declarations. This branch does not enter, publish or approve any App Store
privacy response. It does not alter the app's bundled privacy manifest.

## Validation and operational boundary

Local review checks the complete diff, HTML structure, duplicate IDs, local
fragment targets, relative page/style links, retained legacy privacy anchors,
draft metadata, exact parity with the reviewed privacy candidate, and unchanged
brand/style/Terms files. External destinations retain their existing URLs; no
network link test or provider operation is needed for these edits.

No deployment, build, paid AI request, paid service change, production data
operation, provider message or App Store edit is part of this implementation.
Commits, pushes and pull requests, if later authorized and performed by the
coordinating workflow, do not themselves clear the publication gates.
