# Merged client checklist — Chats 1–3

Updated: 14 October 2026. Store: Tokyo Nights Coffee.

This is the consolidated status register for [Chat 1](chat-1.md), [Chat 2](chat-2.md) and [Chat 3](chat-3.md). Duplicate requests are merged; the originals are retained as source records. This consolidation uses the existing evidence and adds no new store inspection or store changes.

**Overall status:** documented development and preservation checks are complete within their stated scope. Supplier clarification, sender setup/testing, checkout testing and final handoff actions remain open. No new theme feature is identified in the messages. The developer still needs to verify the original-scope/no-extra-fee commitment; the client has offered conditional closure, not final acceptance.

## Done — verified work and documentation

| ID | Completed item | Evidence and limits |
|---|---|---|
| D1 | Published theme and recorded storefront QA | Main theme 185649430801 confirmed October 14. October 12 QA covers shipping copy, Tokyo-inspired wording, all 11 tea pages/cart presentation, coffee filters and Discovery Boxes navigation. Completed checkout and supplier fulfillment are excluded. [October 12 functional QA](evidence-2026-10-12/live-verification.json). |
| D2 | Three unpublished products protected | Ginza Velvet, Harajuku Heat and Shibuya Sunrise remain Draft in October 14 Admin checks; public URLs return 404. Keep this safeguard in place. [October 14 Admin checks](evidence-2026-10-14/admin-product-review.json). |
| D3 | Mint/Honduras records and audited SKUs preserved | Both Mint and both Honduras records remain Active. All 74 displayed variant-label/SKU pairs match October 12: 17 per Mint record and 20 per Honduras record. No fields edited or saved. This is not a store-wide or private supplier-mapping audit. [74-pair comparison](evidence-2026-10-14/admin-sku-comparison.json). |
| D4 | Supplier reply and SKU risks documented | Forwarded Raheel reply records supplier-SKU recognition, imported SKUs, order synchronization and payment before processing/shipping. Internal SKUs and Shopify product IDs do not prove fulfillment readiness. Duplicate and product-specific questions remain open. [Supplier reply review](chat-3.md). |
| D5 | WZ SMTP alternative and proposed Resend cost documented | October 14 WZ dashboard offers Gmail or any SMTP provider. Resend Free is proposed at $0 within 100 emails per UTC day and 3,000/month. Both limits apply; other account usage consumes quota. WZ limits/fees are separate. No sender was configured or tested. [WZ review](chat-2.md). |
| D6 | Checkout procedure and restrictions preserved | Access, isolation, test execution and restoration steps are documented. No payment testing, real charge or supplier order was activated by this review. [Historical test procedure](HANDOFF-STATUS-2026-10-12.md). |
| D7 | Evidence and responsibility register assembled | Dated evidence, safeguards and owners are documented. No personal sender was used or Gmail password requested. External dependencies are tracked separately from verified development. [Merged checklist](chat-merged.md). |

“Done” for documentation or preservation does not mean supplier mapping, notification delivery or checkout testing has passed.

## Pending — owners and completion steps

| ID | Pending item | Owner | Required next step / closure evidence |
|---|---|---|---|
| P1 | Exact supplier mapping and supported variants | Dripshipper | Written mapping/import instructions, supplier products/SKUs and Whole Bean/Ground support for each of the three drafts. Keep them Draft. |
| P2 | Duplicate SKU resolution and supplier synchronization | Dripshipper | Confirm recognition of repeated Mint/Honduras SKUs and the approved resolution procedure. Preserve both pairs; do not infer synchronization from SKU equality. |
| P3 | Original supplier thread metadata | Client | Retain/forward original email date, headers and ticket reference if available. Forwarded text has already been received; this is a recordkeeping follow-up. |
| P4 | WZ sender switching, queues and default option | WZ support | Confirm subscriber/queued-alert/template/workflow preservation, retry and rollback behavior; whether a temporary/default sender exists and its costs; collaborator versus direct-owner authorization requirements. |
| P5 | Installed WZ plan and sender/template inspection | Developer + WZ support | Finish sender-form/template and installed-plan checks. Dashboard SMTP support is verified; the follow-up form inspection stopped when the browser connection timed out. |
| P6 | Resend authorization, setup and actual delivery | Owner/business administrator + developer | Approve business account and verified sending domain, enter SMTP credentials privately, preserve WZ records and verify an authorized isolated email/restock test. No personal sender or Gmail password. |
| P7 | Controlled checkout test | Owner + Dripshipper + developer | Obtain explicit authorization, payment-test access/window and written supplier isolation before any order. Then record simulated payment, order, inbox receipt and settings restoration. Payment-before-shipping is not isolation proof. |
| P8 | Original-scope/no-extra-development-charge confirmation | Developer | Check the original agreement and personally confirm item 6. No new theme feature is identified, but the agreement and billing terms are not in the evidence. Disclose optional third-party fees separately. |
| P9 | Verified rollback reference | Developer/owner | Attach the existing backup ID/name or ZIP location and timestamp. A historical theme ID alone is not a verified backup. |
| P10 | Publish the updated audit and obtain acceptance | Developer, then client | Deploy reviewed files through the existing Vercel project, verify the shared URL, send the handoff and record actual client acceptance. Local edits and conditional readiness to close are not deployment or acceptance. |

## The client’s six final confirmations

| Requested confirmation | Status | Reference |
|---|---|---|
| 1. Published and functioning theme | Verified within dated QA scope | D1; payment/fulfillment excluded. |
| 2. Supporting evidence for completed QA | Done for listed checks | D1–D7; retain evidence dates and limitations. |
| 3. Three unpublished products protected | Done — safeguard verified | D2; keep unpublished pending P1. |
| 4. Supplier SKUs and existing records unchanged | Verified for audited records/fields | D3; private supplier mapping and current variant IDs not independently reverified. |
| 5. Dependencies have owners and next steps | Done — documented | P1–P10; resolving dependencies remains pending. |
| 6. No additional work/charges for original scope | Pending developer confirmation | P8; verify against the original agreement. |

## Evidence dates and limits

- **October 14:** public theme/404 checks; authenticated Admin checks of three drafts and four retained Active records; all 74 displayed variant-label/SKU pairs compared with October 12; WZ dashboard showed 1 of 2 setup steps complete and SMTP availability.
- **October 12:** detailed storefront screenshots and functional QA; original variant-ID/SKU register; Gmail Not connected and blank SMTP-field inspection. Those field-level sender observations were not reverified after the October 14 connection timeout.
- **October 11:** historical exhaustive filters/catalog/cart checks, shipping configuration and original supplier support request.
- Individual variant IDs and Dripshipper's private mappings were not independently re-read in the October 14 bulk-editor comparison. Supplier-side synchronization was not exercised.
- No product/SKU/inventory/mapping/payment/fulfillment changes, orders or messages were made by this review. Client screenshots were not republished.

## Resend setup after approval

WZ supports SMTP; Resend is a suitable proposed provider, not a connected or delivery-tested integration. The earlier October 14 research verified **100 emails per UTC day and 3,000/month** on Resend Free. Both caps and WZ's separate allowance apply. Confirm available quota and WZ retry behavior before any restock burst.

1. Use an owner-approved business Resend account; verify the intended sending domain/subdomain through DNS.
2. In WZ Manual SMTP use host `smtp.resend.com`, port `587` with STARTTLS (or `465` with implicit TLS if required), username `resend`, and a Resend sending API key as the password.
3. Set an approved From Address on the verified domain. Keep the key private; Gmail OAuth is unnecessary for this route.
4. Confirm template/send-method selection and preserve subscriptions, queues, templates and embed. Do not assume later switching is lossless without WZ confirmation.
5. After authorization, test with a controlled inbox and isolated non-supplier fixture; record actual delivery and restock behavior before marking P6 complete.

Sources already checked October 14: [Resend SMTP](https://resend.com/docs/send-with-smtp), [Resend quotas](https://resend.com/docs/knowledge-base/account-quotas-and-limits), [WZ listing](https://apps.shopify.com/wz-back-in-stock). A Resend account is not a WZ-provided default sender. Any paid upgrade requires separate disclosure and approval.

## Next actions in order

1. Developer: confirm P8 against the agreement and attach the existing backup reference (P9).
2. Follow the client's existing Dripshipper thread for P1–P3; preserve records meanwhile.
3. Finish WZ clarification/inspection (P4–P5), then propose the business Resend setup for owner approval (P6).
4. Leave checkout testing on hold until all P7 conditions are met; complete unrelated handoff work meanwhile.
5. Deploy the updated audit and verify the [shared URL](https://tokyocoffeeauditreport.vercel.app/audit-2026-10-08.html), then share it and request acceptance of the verified development scope, tracking external dependencies separately.

## Supporting records

- [Updated audit](audit-2026-10-08.html)
- [October 14 public checks](evidence-2026-10-14/public-http-checks.json)
- [October 14 Admin products](evidence-2026-10-14/admin-product-review.json)
- [October 14 SKU comparison](evidence-2026-10-14/admin-sku-comparison.json)
- [October 12 functional QA](evidence-2026-10-12/live-verification.json)
- [October 12 complete variant-ID/SKU baseline](evidence-2026-10-12/supplier-record-check.json)
- [Historical checkout/rollback procedure](HANDOFF-STATUS-2026-10-12.md) — its no-supplier-reply status is superseded by the October 14 forwarded response.
- [Simple setup/deployment steps and unsent drafts](NEXT-STEPS-2026-10-14.txt)

**Publication status:** local report files updated; no deployment or client message was performed by this consolidation.
