# Olist Fulfilment Pipeline

A dbt pipeline analysing order fulfilment performance for the Olist Brazilian e-commerce dataset.

---

## The Question

<!-- Finish these sentences. Two or three sentences total is enough. -->

Olist's operations team needs a reliable view of their order fulfilment to understand how many orders are getting completed, how long they take, and where delays concentrate.

The pipeline in this repo produces staging tables for the relevant source tables and a fulfilment data mart to answer the questions of the operations team.

---

## Scope

**In scope (v1)**

- Four source tables: `orders`, `order_items`, `customers`, `products`
- A staging layer with one model per source table
- A single fulfilment mart answering the question above
- Data tests covering the assumptions documented below
- CI running the pipeline on every pull request
- Generated dbt documentation

**Out of scope (deferred to v2)**

- Review score analysis — the planned next question is whether delivery lateness predicts poor reviews
- Payments, sellers, and geolocation tables
- Incremental models and orchestration

The boundary is deliberate. v1 exists to establish a trustworthy view of what "delivered" actually means; the more interesting questions depend on getting that right first.

---

## Data source

[Brazilian E-Commerce Public Dataset by Olist](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce) — approximately 100,000 real anonymised orders placed between 2016 and 2018.

The raw CSVs are not committed to this repo. See _How to run this_ below for loading instructions. The dataset carries its own licence terms, listed on the Kaggle page.

---

## Data quality findings

_(not yet written)_

<!-- What the data turned out to be like, once you looked. One short paragraph per finding.
     Write these as you discover them, not at the end — you will forget the details. -->

---

## Decisions and assumptions

_(not yet written)_

<!-- The most important section in this README. For each ambiguity you hit:
     what you decided, why, and what it costs.

     Write in sentences, not bullets. "Cancelled orders are excluded because ...,
     though this means ..." — the reasoning is the point, not the choice. -->

---

## Testing approach

_(not yet written)_

<!-- Each test should trace back to a decision above. The framing to aim for:
     a test is a written assertion that a rule still holds, not a check that
     the pipeline ran. Say what would break if each assumption quietly stopped
     being true. -->

---

## How to run this

_(not yet written)_

<!-- Prerequisites, loading the data, configuring credentials, running the build.
     Credentials live outside this repo — never commit a service account key. -->

---

## Further work

_Automate ingestion via GCS with scheduled loads_

<!-- Everything interesting you found and deliberately did not chase.
     This section is what stops the scope creeping. -->

---

## Licence

MIT — see [LICENSE](LICENSE).
