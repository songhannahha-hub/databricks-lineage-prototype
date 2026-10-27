# Selective Lineage Expansion — Unity Catalog UX Prototype

A standalone interactive prototype for a Databricks APM product proposal. It demonstrates how engineers could choose which upstream or downstream dependencies to add to a lineage graph.

## Preview
Open [index.html](./index.html) locally in Chrome. No build step, API key, or package installation is required.

## Main demo
1. Click the downstream + on `order_lines`.
2. Search `finance_`; select `finance_01` and `finance_02`, then apply.
3. Notice the original Growth views remain visible.
4. Use downstream + on `finance_01` to explore `margin_metrics`, then continue into `Finance Performance`.
5. Reopen a picker to revise selected dependencies, or try the additional illustrative Growth and Operations branches.

The first 24 synthetic views (`finance_01..08`, `growth_01..08`, `operations_01..08`) recreate the user's trial-workspace demonstration. Additional multi-hop assets are illustrative, not observed production lineage.

## Deployment
This repository contains a static site. Deploy its root folder (including `index.html`) to a static hosting provider such as Netlify or GitHub Pages to share a live URL. GitHub repository access alone is not a public interactive demo.

This is a UX prototype, not an official Databricks product or integration.