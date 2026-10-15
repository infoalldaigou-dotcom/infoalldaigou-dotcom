# 1688, Taobao and Xianyu: an order-request validation checklist

A practical documentation template for teams collecting China sourcing requests from overseas buyers. Written by the AllDaigou Mall team. This is a proposed workflow, not a description of a live API or a guarantee that a particular item can be purchased or shipped.

![1688, Taobao and Xianyu: item, cost and delivery checks](https://assets.st-note.com/img/1792085469-q46TG1nfQMsbNSzgw3v5KBRp.png)

*AI-generated explanatory illustration; not a product, warehouse or inspection photograph.*

## Start with the buyer's question

“Can I buy a small batch from 1688 for delivery to the US?” and “Can I request a used item from Xianyu for delivery to Japan?” need different follow-up questions. A single product link is not a complete order request. Taobao purchases also require the exact variant and set contents to be clear.

The goal of validation is to identify missing information before a quote or purchase decision. It is not to decide that one marketplace is always cheaper, safer or faster. Check the actual listing and seller conditions.

## Separate input validity from order readiness

Use distinct states in your documentation:

1. **Draft:** the buyer is still gathering links and requirements.
2. **Needs review:** basic fields are present; price, availability, conditions or shipping still need confirmation.
3. **Quote reviewed:** the agreed scope and cost assumptions have been checked at a recorded time.
4. **Purchase authorized:** the buyer has authorized the specific purchase under the confirmed terms.

These are suggested states for a workflow you design. Passing a form check should never silently imply purchase authorization. If the listing, quantity, destination or material condition changes, return the relevant decision to review.

## A validation matrix that reviewers can use

| Field or condition | Basic validation | Human review question |
| --- | --- | --- |
| Listing URL | Non-empty, well-formed URL | Does it point to the intended current listing? |
| Variant and set contents | Record the selected options | Does the seller's option match the buyer's request? |
| Quantity | Positive integer | Is that quantity available under the stated conditions? |
| Destination country | Explicitly recorded | Is the item acceptable for the proposed route? |
| Requested checks | List the requested work | Is that work available and included in the quote? |
| Costs | Currency and quote status recorded | Which costs are confirmed, estimated or still unknown? |
| Buyer decision | Record scope and time | Was this exact purchase authorized? |

Do not use zero as a substitute for an unknown cost. “Not quoted” and “confirmed free” should have different values and different labels. Keep quote assumptions visible, including what is excluded. Currency conversion and rounding rules must be defined before comparing totals.

## Add listing-specific questions

### 1688: quantity and batch assumptions

For a small-batch sourcing request, record any minimum quantity, quantity-based price conditions and whether different variants can be combined. These conditions depend on the listing. Do not assume that every 1688 item has the same wholesale rules.

### Taobao: the exact retail selection

Record color, size or model and what is included in the selected option. A listing image may show a set while the chosen variant contains only one part. Save the buyer's intended selection clearly enough for another reviewer to understand it.

### Xianyu: evidence about this particular item

For a used-item request, record the current photos, disclosed wear, included accessories and unresolved seller questions. Keep a date for the evidence review. A photo review is not a warranty of authenticity, function or remaining life. Not every listing on Xianyu is used; apply the checks to the actual item.

## Suggested acceptance cases

| Input or change | Expected result |
| --- | --- |
| Quantity is 0, negative or fractional | Ask for a valid quantity; do not mark input complete |
| International shipping is unknown | Display “not yet quoted”; do not display free shipping |
| Buyer changes delivery from US to Japan | Recheck route and shipping quote assumptions |
| A Xianyu listing is replaced by another item | Invalidate the old item's condition review |
| Buyer changes the Taobao size | Recheck selection, price and availability |
| 1688 quantity falls below a confirmed minimum | Request a revised quantity or seller clarification |
| All fields are filled but no buyer decision is recorded | Keep purchase authorization pending |

These are review scenarios, not results from a running system. They can become tests once a team implements its own validation rules. Keep personal addresses, phone numbers, payment data and private seller conversations out of public examples and repositories.

## Prepare a quote request

An overseas buyer can prepare five things: the product link, exact specification, quantity, destination country and requested checks. That makes a 1688 versus Taobao versus Xianyu comparison more meaningful than comparing a headline item price alone.

For service information and purchase-agent enquiries, see [AllDaigou Mall](https://mall.alldaigou.com/?lang=en&utm_source=github&utm_medium=article&utm_campaign=marketplace_choice_20261016). Availability, fees, inspection scope and shipping terms must be confirmed for the specific request.
