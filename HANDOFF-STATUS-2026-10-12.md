# Tokyo Nights Coffee — completion and dependency register

Updated: 12 October 2026. Store: tokyo-nights-coffee / 0c3u4u-pe.myshopify.com. Public site: https://tokyonightscoffee.com/.

## Acceptance status

The client has offered conditional acceptance of completed development, with external dependencies documented. This handoff completes the requested documentation for items 2–4 and supplies the evidence register for item 5. It does not represent a completed payment test, permanent WZ authorization, supplier confirmation, or formal client acceptance.

Item 1 was completed by the user and excluded from this session's change scope. Public storefront verification on 12 October independently confirms theme **185649430801**, **COFFEE | JCI | WORKING | SEP 2026**, role **main**. No theme publication or theme-code changes were performed in this session.

## Done and pending

| Client requirement | Completed | Pending / detailed reason | Responsible party and closure evidence |
|---|---|---|---|
| 2. Preserve unpublished Core Four | Ginza Velvet, Harajuku Heat and Shibuya Sunrise remain Draft in Admin; each public URL returns 404 without an add-to-cart form. | Release remains on hold because exact supplier products, variants, SKUs and synchronization have not been confirmed. | Dripshipper supplies written mappings; owner approves any later publication. |
| 2. Preserve Mint/Honduras | All four original product IDs remain accessible. Variant IDs, SKUs and option arrays exactly match the October 11 baseline. No merge, deletion, relinking or inventory change performed. | Which duplicate the supplier actively synchronizes remains unconfirmed. Similar names are not sufficient evidence. | Dripshipper identifies the canonical product and variant IDs and synchronization behavior in writing. |
| 2. Support-request details | Exact original request, submission method, known date, product IDs and submission screenshot included below. | No ticket ID or subsequent response is available in the supplied project evidence. The registered store mailbox has not been verified in this session; absence of a supplied reply is not proof that support has not replied. | Owner checks the registered store mailbox and spam folder, supplies the reply/thread or ticket reference; developer adds it to the register. |
| 3. Checkout handoff | Required access, safeguards, execution steps, evidence and restoration procedure documented below. No order or payment submitted. | Execution remains pending: payment controls were inaccessible in the October 11 session and supplier isolation is unconfirmed. The client's instruction permits documentation and prohibits unauthorized real payment or supplier fulfillment. | Owner provides access and an approved test window; Dripshipper confirms safe isolation; tester records simulated payment, order and received confirmation. |
| 4. WZ handoff | Current setup inspected: 1 of 2 complete; Gmail Not connected. Manual SMTP host, user and from address are blank. Existing settings preserved. Authorization and delivery-test procedure supplied below. | Permanent sender authorization and actual delivery remain pending. Client reports deployment connectivity limitations; account consent/SMTP credentials must be supplied by the owner through the app. | Owner authorizes sender once connectivity works; developer verifies controlled delivery and records receipt. |
| 5. Theme identity | Live theme ID/name/role independently verified and current live screenshots included. | Backup identifier, backup timestamp and exact pre-publication comparison evidence are not available in this repository. User reports item 1 completed; those details are requested only for the final record. | User attaches the already-created backup reference and publication verification evidence. |
| 5. QA and dependencies | Completed checks, prior evidence, current screenshots, supplier request and remaining owner actions assembled in this handoff and audit report. | Formal acceptance remains the client's decision after review; external tests are not marked passed. | Client reviews the handoff; owner supplies missing backup/support records. |

## Protected supplier records

| Product | Shopify product ID | State / safeguard |
|---|---|---|
| Ginza Velvet | 10979128443153 | Draft; public 404; preserve supplier-linked fields. |
| Harajuku Heat | 10979129360657 | Draft; public 404; preserve supplier-linked fields. |
| Shibuya Sunrise | 10979127787793 | Draft; public 404; preserve supplier-linked fields. |
| Mint / mint | 10952738308369 | Retained; variant IDs, SKUs and options match October 11. |
| Mint / mint-1 | 10952740372753 | Retained; variant IDs, SKUs and options match October 11. |
| Honduras / honduras | 10952739979537 | Retained; variant IDs, SKUs and options match October 11. |
| Honduras / honduras-1 | 10952740012305 | Retained; variant IDs, SKUs and options match October 11. |

No original product records, supplier SKUs, variants, inventory, payment settings, fulfillment settings or integrations were edited in this session. These safeguards describe this session and the checks above; they do not certify the operation of Dripshipper's private synchronization or every historical store field.

## Dripshipper request and response register

- Submitted: 11 October 2026, per the prior closure tracker; exact submission time unavailable.
- Channel: Shopify Admin → Dripshipper → Get support form.
- Submission evidence: [original form result](evidence-2026-10-11/supplier-request-result.png). Prior operator recorded that Send dismissed the form without an error; no ticket ID was displayed.
- Reply destination: registered store email, per the prior tracker. The mailbox address is omitted from the public report.
- Ticket reference: not provided by the form / unavailable in project evidence.
- Subsequent response: not supplied or verified as of this handoff. No new support message was sent in this session.
- Owner follow-up: find the original acknowledgement/reply in the store mailbox (including spam), preserve the date, sender, ticket reference and exact response, and attach it to the project. If no acknowledgement exists, the owner can contact Dripshipper using the request below and ask for a reference.
- Closure gate: exact Mint/Honduras mappings, three Core Four supplier options, supported variants/SKUs, inventory synchronization and a documented no-fulfillment test method must be answered. Keep supplier-dependent changes on hold until verified.

### Exact request previously submitted

Hello Dripshipper Support,

We are completing supplier verification for Tokyo Nights Coffee (0c3u4u-pe.myshopify.com; admin store tokyo-nights-coffee). Please confirm the exact Shopify Product ID you actively synchronize for each duplicate pair recorded in our audit:
Mint: mint — 10952738308369; mint-1 — 10952740372753.
Honduras: honduras — 10952739979537; honduras-1 — 10952740012305.

Please also confirm fulfillment options for Ginza Velvet, Harajuku Heat and Shibuya Sunrise, including the exact corresponding supplier products (if any), supported Whole Bean/Ground variants, supplier SKUs and inventory synchronization requirements. We will not guess mappings from similar descriptions.

For a controlled Shopify checkout test, can a Shopify test order trigger any Dripshipper import, charge or fulfillment? Please confirm the supported method to guarantee no real supplier fulfillment.

This is a verification request only. Please do not modify, delete, merge, relink or fulfill any product/order on our behalf.

Thank you.

## Controlled checkout test — future execution procedure

**Status: procedure complete; transaction not run. No real charge or supplier fulfillment is authorized.** A cart-only check is not payment or confirmation-email verification.

### Permissions and prerequisites

- Owner or authorized staff must be able to access Settings → Payments and manage the configured provider's test mode. Owner-only/provider-account actions must be completed by the owner; do not share passwords in this report.
- Tester needs Orders access to view and cancel the test order, store-setting access for approved order-processing changes, access to Dripshipper's controls, and access to a designated test inbox. Product/inventory permissions are needed only if a separately approved isolated test product is used.
- Record the existing payment provider and mode, automatic fulfillment setting, app import/fulfillment rules, inventory baseline, and any automation that could respond to an order. Do not publish these credentials or private customer information.
- Obtain Dripshipper's written isolation method. Disabling Shopify automatic fulfillment alone is insufficient evidence that an app will not import or bill an order. Do not uninstall the integration, change supplier SKUs, or disconnect product mappings as an improvised workaround.
- Use an isolated test store where possible. If testing the production checkout is required, owner must approve a restricted maintenance window and shopper-access controls, because test mode affects customer checkout. Agree on restoration and who will supervise it.

### Execution, only after all prerequisites are satisfied

1. Confirm the approved test window, authorized tester, test inbox and precise product/variant. Do not use or publish the three protected Core Four products. If the supplier cannot guarantee safe testing of its variants, stop; an isolated test product/store can verify checkout mechanics but cannot certify supplier fulfillment.
2. Snapshot existing settings and inventory. Apply only the owner-approved isolation controls for Shopify automatic fulfillment, Dripshipper imports/fulfillment and other order automations. Verify the isolation before any order exists. A TEST tag alone is not an isolation control.
3. Enable the supported test gateway. If Shopify Payments is configured, use Settings → Payments → Shopify Payments → Manage → Test mode → Enable test mode → Save. If that provider is absent, follow the installed provider's documented sandbox setup; never substitute a real card, manual payment, or a charge-and-refund test.
4. Verify the provider is visibly in test mode. Use only its documented test card values. For Shopify Payments, a successful Visa simulation uses 4242 4242 4242 4242, a future expiry, three-digit security code and a two-word name. These values are not for other gateways.
5. Add one approved item in a clean browser cart, confirm the intended variant/quantity and currency, and open checkout. Use the designated controlled inbox and an approved U.S. test address. Check the displayed shipping quote against the configured rules, including the $4.95 standard rate and $35 free-shipping threshold where applicable. Record tax/address-dependent results; do not promise a universal tax value.
6. Submit one simulated transaction only. Verify a test-marked order, correct item/variant, totals and transaction result in Admin. Verify no real payment capture, supplier import/billing, fulfillment request or shipping label. If any safeguard is uncertain, stop and escalate to the owner.
7. Verify the confirmation page and actual order-confirmation receipt in the controlled inbox (including spam). Record order reference, test gateway/mode, UTC timestamp, payment result, fulfillment status and redacted receipt screenshot. An email queued/sent status alone is not inbox receipt. A simulated decline can be checked separately only within the same approved controls.
8. Cancel the test order, reverse only its inventory effects as appropriate and confirm it is excluded from any supplier queue before restoring integrations. Archive/delete only the test record if supported and approved; never touch real orders.
9. Disable test mode, restore the recorded payment/automation settings and shopper access, then verify ordinary checkout availability without submitting a live payment. Record restoration evidence and remove test data only from the controlled test scope.

**Pass criteria:** simulated payment and order creation, correct order contents/totals, received confirmation email, no supplier activity/charge, and verified restoration. Until these are recorded, keep payment/order/email testing pending.

References: [Shopify test-order precautions](https://help.shopify.com/en/manual/checkout-settings/test-orders/processing-test-order), [Shopify Payments test-mode instructions](https://help.shopify.com/en/manual/payments/shopify-payments/testing-shopify-payments), [Shopify store permissions](https://help.shopify.com/en/manual/your-account/users/roles/permissions/store-permissions).

## WZ Back In Stock — authorization and delivery procedure

**Status: existing setup preserved; permanent authorization and delivery not completed.** On 12 October, the app reports 1 of 2 setup steps complete and Gmail Not connected. SMTP host, username and from address are unconfigured; default port shown is 587. No credentials were entered and no settings were saved.

1. Owner ensures the WZ deployment and its Gmail authorization callback are reachable. If the owner-reported connectivity issue persists, restore deployment access first and record the exact error privately. Do not claim that the current reachable dashboard proves the OAuth callback works.
2. In Shopify Admin → Apps → WZ Back In Stock → Open sender email, choose the owner's intended permanent method. For Gmail, select Gmail → Connect Gmail; the owner signs in to the approved sending account and grants consent through Google. Confirm Not connected becomes connected and From Address matches that account. Do not disconnect an existing valid sender.
3. For an approved SMTP alternative, select Manual SMTP and enter the provider-issued host, port/TLS-compatible settings, username, credential and authorized From Address. Confirm the app's configuration requirements with the provider. Save through the app; never put passwords or tokens into the audit or support request.
4. Inspect Alert email template and its send method. The current UI states Manual SMTP is used for Custom alert email. Record the current selection before any change and ensure the intended sender/template combination is supported. Preserve the theme embed, template content, waitlist records and existing customer subscriptions.
5. Use an owner-approved isolated, non-supplier test product/variant and controlled inbox. Obtain approval before creating the fixture or changing its stock. Do not modify the Core Four, Mint/Honduras, real supplier inventory or real customer waitlists to manufacture a restock event.
6. If the app provides a test-send function, send only to the controlled inbox and verify actual arrival, From/Reply-To, subject, product link and unsubscribe behavior. This checks sender delivery but does not by itself pass the restock workflow.
7. With a safe isolated fixture, confirm the storefront signup appears at zero stock, subscribe only the controlled inbox, and confirm the app records that signup. Restock only that fixture using the approved trigger. Verify the app's alert record and actual inbox receipt; record timestamps, fixture ID, trigger, sender, receipt and whether duplicate notifications occur. Do not trigger a batch to existing customer waitlists.
8. Remove only the test signup/fixture or return it to its agreed state; preserve real subscriber records and the permanent sender connection. Capture the final connected/setup state and redacted delivered-email evidence.

**Pass criteria:** authorized permanent sender, matching From Address, actual test-email receipt and controlled restock delivery. Template preview or OAuth consent alone is not proof of delivery. The [WZ app listing](https://apps.shopify.com/wz-back-in-stock) identifies Gmail/SMTP support; the exact controls above were inspected in this store's app on 12 October.

## Publication record and rollback handoff

- Published theme: **185649430801 — COFFEE | JCI | WORKING | SEP 2026**. Public Shopify theme metadata reports role **main** on 12 October.
- Publication: completed by the user before this task, as instructed. No new publication performed here.
- Previous live theme in the October 11 record: **182090334481 — coffee**. This is a historical rollback candidate, not evidence that a verified backup was created or is still available.
- Backup name/ID or ZIP, creation time/location and pre-publication version comparison: **awaiting the user's existing publication record**. The local Theme folder and October 11 nine-file match report are not presented as a complete pre-publication backup.
- Rollback procedure for the owner: verify the intended pre-publication backup in Online Store → Themes, inspect its preview and identity, record the current live theme, then publish the confirmed backup only if rollback is authorized. Recheck homepage, products, cart, navigation and app embed. Theme rollback does not undo store-wide menus, Search & Discovery settings, product data, payments or integrations; those require their separate recorded configuration.

## Evidence and QA interpretation

October 12 evidence is current live verification. October 11 assets remain historical implementation evidence and are explicitly dated. Current checks cover public theme identity, shipping/origin homepage copy, three protected URLs and Admin states, Mint/Honduras variant/SKU preservation, live tea presentation, coffee filters and Discovery Boxes, plus the WZ setup state. The report lists exact coverage and evidence links.

No end-to-end supplier fulfillment, live payment, order-confirmation delivery or permanent WZ delivery is counted as passed. No final acceptance message or Fiverr resubmission has been sent by this session.

## Remaining owner actions, in order

1. Attach the already-completed publication backup reference and version-comparison record for the final handoff.
2. Check the store support mailbox; provide Dripshipper's acknowledgement and any reply. Keep supplier-dependent changes on hold.
3. Arrange payment access, written supplier isolation and an approved test window before anyone executes the documented checkout procedure.
4. Resolve WZ connectivity as needed, authorize the permanent sender through the app and approve an isolated delivery test.
5. Review the updated audit and submit it to the client with external dependencies explicitly retained. Formal acceptance belongs to the client.

## Completed QA checklist

| Check | Result | Evidence / scope |
|---|---|---|
| Published theme identity | PASS | [Live metadata](evidence-2026-10-12/live-verification.json): 185649430801, role main. |
| Desktop/mobile homepage | PASS | [Desktop](evidence-2026-10-12/live-home-desktop.png), [mobile](evidence-2026-10-12/live-home-mobile.png); shipping copy and revised Core Four text. |
| Core Four protection | PASS | [Admin records](evidence-2026-10-12/protected-products-admin.png), 404s in live metadata. |
| Mint/Honduras data comparison | PASS | [Four original records and variant/SKU comparisons](evidence-2026-10-12/supplier-record-check.json). |
| Tea presentation | PASS | All 11 original tea URLs returned 200; Format / Loose Leaf labels and Grind / Loose leaf inputs verified in live metadata. [Current mobile capture](evidence-2026-10-12/live-tea-mobile.png). |
| Live cart presentation | PASS | [Ginza Grey cart](evidence-2026-10-12/live-tea-cart.png) displays Format: Loose Leaf. Isolated browser context; test items removed; no checkout submitted. |
| Coffee filter display and application | PASS | [Two choices](evidence-2026-10-12/live-coffee-filter-desktop.png), [Whole Bean 54](evidence-2026-10-12/live-whole-bean.png), [Ground Coffee 60](evidence-2026-10-12/live-ground-coffee.png). Full pagination/variant exclusion checks are October 11 evidence, not re-run exhaustively today. |
| Discovery Boxes collection/navigation | PASS | [Three products](evidence-2026-10-12/live-discovery-mobile.png), [mobile menu](evidence-2026-10-12/live-navigation-mobile.png). |
| Historical implementation validation | PASS — October 11 | [Nine remote-file matches](evidence-2026-10-11/remote-theme-file-check.json); earlier tracker records Liquid/schema validation. No theme code changed today. |
| WZ current status | VERIFIED PENDING | [Setup status](evidence-2026-10-12/wz-setup-status.png), [Gmail not connected](evidence-2026-10-12/wz-gmail-not-connected.png). |
| Controlled payment / order / confirmation email | NOT RUN | Access and supplier isolation prerequisites remain outstanding. |
| Permanent WZ restock-email receipt | NOT RUN | Permanent sender is not authorized. |
| Supplier mapping / synchronization / fulfillment | NOT VERIFIED | Requires Dripshipper's response and approved isolation. |
| Audit report layout and links | PASS | Desktop and mobile rendered; no document overflow at 390px; local linked assets exist. |

## Suggested client resubmission note

Hi Karlton,

The published storefront has been rechecked, and the audit now includes current live screenshots, the completed QA checklist, the original Dripshipper support request, and a detailed dependency register. The three unpublished Core Four products and existing Mint/Honduras records remain preserved; their supplier-linked variant IDs, SKUs and option values were not changed.

The handoff also documents the permissions, safety controls and exact steps for the deferred checkout test and permanent WZ sender authorization/delivery test. No real payment or supplier fulfillment was triggered. Supplier confirmation, controlled checkout execution and permanent WZ delivery remain explicitly open pending the prerequisites listed in the report.

Please review the updated audit at https://tokyocoffeeauditreport.vercel.app/audit-2026-10-08.html. The publication backup reference and any Dripshipper reply should be attached to the handoff before representing those records as complete. The completed development scope is ready for your review with these dependencies disclosed.

Thank you.
