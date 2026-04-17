# case-study

Approach
I began by evaluating data quality through the following checks:

  - Primary Key Integrity: Confirmed that all primary keys are unique.
  - Null Value Analysis: Verified that no unexpected null values exist. (Note: The delivered_at column contains nulls for orders currently in transit or lost, which is expected behavior).
  - Chronological Logic: Validated that created_at precedes shipped_at, which in turn precedes delivered_at.

Due to time constraints, these checks served as the baseline to ensure data reliability before proceeding with the analysis.

Findings

  - High Delay Rates: Several sellers have a delay rate exceeding 50%. Further analysis is required to identify the root causes of this variance.
  - Carrier Performance: In-house delivery maintains a strong record for on-time arrivals. Among external vendors, Bluedart shows a marginal lead in on-time performance. If I were to continue this analysis, I would investigate how geographical differences impact performance and explore whether the successful in-house delivery model can be replicated for external vendors.
  - Customer Retention: There is no significant difference in repeat purchase rates based on a customer's first delivery experience.


Use of AI

  - Environment Setup: Used an LLM to assist with executing SQL code within my local IDE, as I am more accustomed to using SQL within Databricks notebooks.
  - Debugging: Leveraged AI to resolve specific errors encountered while querying [Task/Section B3].
  - Strategy & Review: Used AI to brainstorm and validate my analytical approach, as well as to proofread this documentation.

