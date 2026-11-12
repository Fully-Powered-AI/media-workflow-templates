# Sponsor delivery record

When a sponsored run ends, the partnerships lead gets a register of each placement in the signed scope beside the publication record, metrics and invoices. Gaps, changed dates and incomparable metrics stay visible; billing questions go to finance.

*Workflow template · Media and entertainment · Sales · version 0.1.0 · [Workflows Directory](https://fullypowered.ai/workflow templates/sponsor-delivery-record/)*

## The outcome

A sponsor asks what it got for its money, and the answer is usually spread across a scope document, a publishing log, an analytics export and an accounts system. This workflow template puts them in one register, placement by placement, in the same order every time.

For each placement the lead names, the register shows what was agreed, what the records show, which records fall outside the dates, which use a different asset, what the metrics say and whether they can be compared with the measure the lead named, and what has been invoiced. What the records do not show is written as missing. It is never rounded up to delivered.

The partnerships lead reads the register, confirms fulfilment placement by placement and agrees any make-good with the sponsor. Finance sees the billing questions, each with its facts, and decides on each.

## Who starts the work, and when

The partnerships lead, or the coordinator working for them, starts it when a sponsored run ends and the sponsor needs evidence of delivery. It can also be run part-way through a long run to see what is short while there is still time to fix it.

## What they supply

- **The placements, as the lead names them from the signed scope:** an identifier, a description, the asset, the quantity and its unit, the dates of the window, the measure the sponsor expects and the fee. The lead types these; the workflow template reads no contract.
- **The publication or broadcast log:** one row per record, with dates, channel, asset and, where known, the placement it belongs to.
- **The metrics supplied,** with the period and the source of each figure.
- **The invoice history:** each invoice with its date, amount, status and the placements it covers.
- **The lead's notes:** agreed date changes, approvals, make-goods already agreed.

## What comes out

One register in a fixed order. Each placement has a status (evidence matches, evidence short, or no record found), the records counted, the records left out of the count and why, the metric position, the invoice position and the lead's own note. Below it come records that match no placement, metrics that cannot be compared, billing questions, make-goods already on file, and the decisions for the partnerships lead and for finance. Nothing is sent, posted, paid or changed.

See the worked example with invented data in [EXAMPLE.md](EXAMPLE.md).

## Where it fits

- [Sales](https://fullypowered.ai/functions/sales/), where the partnerships lead owns the sponsor relationship and answers for what was promised.
- [Marketing and content](https://fullypowered.ai/functions/marketing-and-content/), where the publishing and audience records that prove delivery are kept.
- [Finance and accounting](https://fullypowered.ai/functions/finance-and-accounting/), which decides what is invoiced, credited or held.
- [Media and entertainment](https://fullypowered.ai/industries/media-and-entertainment/), where a sponsor buys placements across shows, newsletters, broadcasts and sites.
- [Marketing and advertising](https://fullypowered.ai/industries/marketing-and-advertising/), where an agency or a publisher reports delivery back to the buyer of the media.
- [Growth & scaling](https://fullypowered.ai/situations/growth-and-scaling/), when the number of sponsored runs outgrows what one person can reconcile by hand.
- [Established businesses](https://fullypowered.ai/situations/established-businesses/), where sponsorship income is a standing line and its evidence has to be orderly.

It stays separate from [client billing summary](https://fullypowered.ai/workflows/client-billing-summary/), which prepares a bill for a client's review, and from [wholesale order check](https://fullypowered.ai/workflows/wholesale-order-check/), which checks a buyer's order against a quote. This one checks delivery evidence for a sponsored run and raises billing questions as a by-product. It also stays separate from [creator publication tracking](https://fullypowered.ai/workflows/creator-publication-tracking/), which is the brand-side check of creators' posts; this one is the publisher-side delivery evidence for a sponsor.

## What has to change for your company

Decide how your records name a placement, so the log can point to it, and keep one identifier for each. Settle your units: what counts as an episode, an issue, an airing or a day on your channels. Write down which metric and which source you give sponsors, since the register compares only a metric and a source that match. Choose who confirms fulfilment, who may agree a make-good and who in finance decides billing. The workflow template reads none of your sponsorship terms and never decides what a term means: where an agreement matters, the lead states the placement and a person at your company reads the agreement. It runs in ChatGPT, Claude, Copilot or Gemini from the files you supply, with no access to your publishing, analytics or accounting systems.

## What has been checked

Fully Powered AI wrote this workflow template in its own words. It was editorially reviewed on 10 November 2026. It was tried once on its invented example in Claude on 10 November 2026, and the record is published with it; the template was revised afterwards in response to that run, and again after an independent review, and the revised version has not been run again. It has not yet been tested in a client environment. It has not yet been tested as a packaged version in ChatGPT, Claude, Copilot or Gemini.

Testing in your environment means running it on a sponsored run your team remembers well, with hard cases written in advance: a placement with no record, a record dated after the window, a replacement asset, a metric measured over a different period, an invoice that is larger than the fees it covers. The partnerships lead checks every count against the logs before the register goes anywhere. [Pilot acceptance-test preparation](https://fullypowered.ai/workflows/pilot-acceptance-test-preparation/) builds that test set, and [what we test before we call an AI workflow ready](https://fullypowered.ai/insights/what-we-test-before-a-workflow-is-ready/) describes the record we keep.

- Written by Fully Powered AI.
- Sources and rights reviewed.
- Editorially reviewed on 10 November 2026.
- Package format checked by script on every release.
- Tried once on its invented example in Claude on 10 November 2026. The record is in [TRIAL.md](TRIAL.md).
- Not yet tested in a client environment.

## What is in this folder

- [TEMPLATE.md](TEMPLATE.md): the complete workflow template. Roles, inputs, the procedure, exceptions and stop conditions, the output format, a reviewer checklist, acceptance tests, the instructions for an AI assistant and what to customize.
- [EXAMPLE.md](EXAMPLE.md): a worked example with invented data.
- [TRIAL.md](TRIAL.md): what came out when the template was tried on its example.
- [SKILL.md](SKILL.md): the technical file, for AI products that load packaged instructions from a folder.
- [SOURCES.md](SOURCES.md): what the workflow template drew on, with licences.
- [LICENSE](LICENSE): MIT. Use it, change it, make it yours.

## Start using it

1. Read [EXAMPLE.md](EXAMPLE.md) to see what a good result looks like.
2. Open [TEMPLATE.md](TEMPLATE.md) and set every item under "What to customize" to your own rules, roles and limits.
3. Give your AI assistant the instruction block and the output format from the template, with your own limits in place of the ones the instructions leave open in square brackets. Paste them in as custom instructions in ChatGPT, Claude, Copilot or Gemini, or copy this whole folder into a product that loads `SKILL.md` packages. This folder stands alone; you do not need the rest of the repository.
4. Run it on past work first, using the reviewer checklist and acceptance tests in the template, before anyone relies on it.

## Related workflow templates

- [Client billing summary](https://fullypowered.ai/workflow templates/client-billing-summary/)
- [Creator publication tracking](https://fullypowered.ai/workflow templates/creator-publication-tracking/)
- [Wholesale order check](https://fullypowered.ai/workflow templates/wholesale-order-check/)

## Make it yours

This is the starting version. Fully Powered AI adapts workflow templates to how your company works, proves them on real work and rolls them out to the roles that use them. [Talk with us](https://fullypowered.ai/contact/).
