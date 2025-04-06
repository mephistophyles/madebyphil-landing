---
layout: default
title: "Financial and Managerial Account Module 1"
---

<h1>{{ page.title }}</h1>

## Module 1: Types of Accounting Frameworks

**Core Concepts:**
- Financial vs. Managerial Accounting: Fundamental differences in purpose, audience, and reporting requirements
- Generally Accepted Accounting Principles (GAAP): Historical development and conceptual framework
- International Financial Reporting Standards (IFRS): Global standardization and key differences from GAAP
- Framework for the Preparation and Presentation of Financial Statements: Underlying assumptions and qualitative characteristics
- Regulatory bodies: SEC, FASB, IASB roles in standard-setting

**Case Discussion:** "Global Accounting Standards Convergence: The Tesla Case" - Examine how Tesla navigates reporting requirements across multiple jurisdictions and markets.

<ul>
  {% assign current_dir = page.dir %}
  {% for sibling in site.pages %}
    {% if sibling.dir == current_dir and sibling.url != page.url %}
      <li><a href="{{ sibling.url }}">{{ sibling.title }}</a></li>
    {% endif %}
  {% endfor %}
</ul>