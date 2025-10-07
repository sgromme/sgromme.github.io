---
title: Constraints
author: scott_gromme
date: 2025-07-11 09:10:00 +0000
categories: [SP Constraints]
tags: [supply planning]
render_with_liquid: false
mermaid: true
---
# Introduction

Constraints in Supply Planning are the business rules and limitiations that control how materials , resources, and production capacity can be used in a supply chain.
These constraints may include supplier lead times, production capacities, storage limits, transportation availability, order minimums, or contractual obligations. They ensure that supply plans are not only cost-effective but also feasible and aligned with real-world limitations.

All constraints have a begin and end date, or a implied never expire date.

Visibility into these constraints is critical for understanding and improving supply planning solutions. Without clear visibility, planners may be unaware of what's driving stockouts, delays, or excess inventory. Transparent constraint visualization allows decision-makers to:

* Identify bottlenecks and trade-offs

* Explain why certain planning decisions were made

* Simulate "what-if" scenarios

* Improve collaboration between operations, procurement, and sales


###        Supply Chain Flow

```mermaid

flowchart LR
  

A(Demand) <--Products/Materials--> B(Supply)

```
