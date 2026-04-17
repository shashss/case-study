# case-study


Approach:
I first checked for the quality by exploring the following: 
  - ensuring the Primary keys are unique
  - no null values present in any of the columns (delivered_at column do have nulls as the orders that are in transit or lost will not be null, which is expected)
  - The Created_at date should be earlier than the shipped_at date which should further be earlier than the delivered_at date.

For the limited amount of time that I had at my disposal, these were some of the checks that I did to ensure the data quality.

Findings: 
  - There are several sellers whose percent of orders delayed is more than 50% - more analysis needs to be done to find the causal variance.
  - Delivery done via Inhouse has good record of delivering On-time. Among the external vendor carriers, Bluedart seems to deliver better On-time maginally, relative to the other vendors. If I were to continue the analysis, I'd focus on how different geographically each Geo operates and that is causing this difference. I'd also focus on the factors why In-house delivery is clearly ahead in On-time delivery and if it can be replicated for the Vendor side as well.
  - There is not significant difference in repeat purchase rate based on the Customer's first delivery experience.

