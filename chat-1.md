# Chat 1 — client safeguards: done and pending

Reviewed: 14 October 2026. Store: Tokyo Nights Coffee.

Connected with Playwright to the user's existing authenticated Chrome/Shopify Admin session. This was a read-only review: no product, SKU, inventory, mapping, theme, sender, payment or fulfillment changes; no Save actions, orders or support messages.

## Client's five requests

| Request | Status | What was checked / what remains |
|---|---|---|
| Keep Ginza Velvet, Harajuku Heat and Shibuya Sunrise unavailable | **Done — safeguard verified** | All three remain **Draft** in Admin on October 14. Earlier October 14 public HTTP checks returned 404 for all three. Keep them unpublished until exact supplier mappings and supported variants are confirmed. |
| Do not replace, modify or overwrite supplier SKUs | **Done — preservation verified for the four audited records** | Read all 74 variant/SKU associations from Shopify's bulk editor. SKU values and displayed grind/size labels match October 12. No fields edited; Save stayed disabled. This is not a store-wide SKU audit. |
| Preserve existing Mint and Honduras records | **Done — records retained; resolution pending** | All four original product IDs remain accessible and Active. Both Mint records have 17 variants; both Honduras records have 20. Do not merge, delete or relink them until Dripshipper supplies its procedure. |
| Do not assume internal SKUs create fulfillment connections | **Done — safeguard documented and respected** | No internal SKU assignment or mapping change performed. Supplier recognition must be validated by Dripshipper; an internal SKU or Shopify product ID is not proof of a working supplier connection. |
| Document recorded SKU mappings and unresolved synchronization risks | **Done — documentation updated** | The report includes all 74 October 12 variant-ID/SKU associations and now links the October 14 Admin comparison. Supplier product mappings, duplicate handling and synchronization are not marked verified. |

“Done” above means the requested preservation/documentation is done. It does not mean the supplier dependencies are resolved.

## Current protected records

| Product | Shopify product ID | October 14 Admin result |
|---|---|---|
| Ginza Velvet | 10979128443153 | Draft |
| Harajuku Heat | 10979129360657 | Draft |
| Shibuya Sunrise | 10979127787793 | Draft |
| Mint (`mint`) | 10952738308369 | Active; 17 variant-label/SKU pairs match October 12 |
| Mint (`mint-1`) | 10952740372753 | Active; 17 variant-label/SKU pairs match October 12 |
| Honduras (`honduras`) | 10952739979537 | Active; 20 variant-label/SKU pairs match October 12 |
| Honduras (`honduras-1`) | 10952740012305 | Active; 20 variant-label/SKU pairs match October 12 |

Both Mint records share the same 17 SKU values; both Honduras records share the same 20 SKU values. This makes duplicate-SKU recognition a supplier question, not permission to remove one record. The current comparison checked displayed labels and SKUs; individual variant IDs remain from the October 12 baseline and were not independently re-read in this bulk-editor review.

## Still not done

| Pending item | Responsible party | Next step / completion evidence |
|---|---|---|
| Exact supported supplier products for the three drafts | Dripshipper | Written mapping/import instructions and exact supplier SKUs for each supported variant. |
| Whole Bean / Ground Coffee support for the three drafts | Dripshipper | Explicit per-product variant confirmation. Existing Mint/Honduras options do not establish support for these drafts. |
| Duplicate Mint/Honduras resolution | Dripshipper | Explain same-SKU recognition and provide the approved preservation/resolution procedure. No changes before confirmation. |
| Supplier synchronization and safe test isolation | Dripshipper + owner | Written isolation procedure and authorized test access/window. SKU equality and payment-before-shipping do not prove safe isolation. |
| Resend sender setup and actual WZ delivery | Owner + developer | Approve business Resend account; verify sending domain; configure SMTP privately; perform an approved isolated delivery/restock test. |
| Safe later sender switch preserving subscriptions/queues/workflows | WZ support | Written switch/rollback procedure; compare records before/after an authorized switch. |
| Payment/order/confirmation-email test | Owner + Dripshipper + developer | Keep on hold until authorization, test-payment access and proven supplier isolation. |
| Original-scope/no-extra-development-fee commitment | Developer | Check original agreement and personally confirm; this review cannot make that commercial commitment. |
| Verified rollback reference | Developer/owner | Attach backup ID/name or ZIP location and timestamp. |
| Publish updated audit | Developer | Deploy reviewed files to existing Vercel project and verify October 14 content at the shared URL. Local edits are not deployment. |

## WZ and Resend

**Fresh WZ observation:** the live app dashboard shows **1 of 2 setup steps complete** and explicitly says **“Use Gmail or any SMTP provider. Emails can't send without this.”** Sender connection remains outstanding. The subsequent sender-form inspection could not finish because the debugging connection stopped responding. Blank sender fields/Gmail “Not connected” remain October 12 evidence, not a fresh October 14 field-by-field verification. The installed billing plan and preservation during a future switch are not yet verified.

Resend is a suitable proposed SMTP provider, not a connected or delivery-tested integration. Its Free quota is **100 emails per UTC day and 3,000 per month**. Both limits apply; other account sending/inbound use consumes quota. WZ plan limits and fees remain separate. No Gmail OAuth is needed for this SMTP route.

1. Owner approves a business-owned Resend account and sending domain/subdomain.
2. Verify the domain using the DNS records Resend supplies.
3. In WZ Manual SMTP, use `smtp.resend.com`, port `587` with STARTTLS (or `465` with implicit TLS if required), username `resend`, and a Resend sending API key as the password.
4. Set an approved From Address on the verified domain; keep credentials out of reports.
5. Preserve the WZ installation, subscriptions, templates and embed. Confirm queue/retry and sender-switch behavior with WZ.
6. After authorization, test using an isolated non-supplier fixture and controlled inbox. Record actual receipt before marking delivery complete.

Sources checked in the preceding October 14 review: [Resend SMTP](https://resend.com/docs/send-with-smtp), [Resend quotas](https://resend.com/docs/knowledge-base/account-quotas-and-limits), [WZ official listing](https://apps.shopify.com/wz-back-in-stock).

## Evidence

- [October 14 Admin product review](evidence-2026-10-14/admin-product-review.json)
- [October 14 SKU and variant-label comparison](evidence-2026-10-14/admin-sku-comparison.json)
- [Ginza Draft screenshot](evidence-2026-10-14/admin-product-10979128443153.png)
- [Harajuku Draft screenshot](evidence-2026-10-14/admin-product-10979129360657.png)
- [Shibuya Draft screenshot](evidence-2026-10-14/admin-product-10979127787793.png)
- [Mint SKU screenshot](evidence-2026-10-14/admin-skus-mint.png) / [second Mint record](evidence-2026-10-14/admin-skus-mint-1.png)
- [Honduras SKU screenshot](evidence-2026-10-14/admin-skus-honduras.png) / [second Honduras record](evidence-2026-10-14/admin-skus-honduras-1.png)
- [October 14 public HTTP checks](evidence-2026-10-14/public-http-checks.json)
- [Updated audit](audit-2026-10-08.html)

The October 12 storefront QA remains dated evidence; this session focused on the client's product safeguards and WZ. It did not rerun every storefront feature or inspect Dripshipper's private fulfillment system.
