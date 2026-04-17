# case-study


Approach:
I first checked for the quality by exploring the following: 
  - ensuring the Primary keys are unique
  - no null values present in any of the columns (delivered_at column do have nulls as the orders that are in transit or lost will not be null, which is expected)
  - The Created_at date should be earlier than the shipped_at date which should further be earlier than the delivered_at date.

For the limited amount of time that I had at my disposal, these were some of the checks that I did to ensure the data quality.

