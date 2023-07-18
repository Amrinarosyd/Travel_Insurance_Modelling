# Travel_Insurance_Modelling
by Amrina Rosyada

## **`Business Problem Understanding`**

**Dataset**: <br>
data_travel_insurance.csv

**Context**: <br>
This dataset pertains to a travel insurance company that offers insurance services to prospective travelers through a third party. Travel insurance is a type of insurance that provides coverage during domestic or international travel. Some countries even require travelers to have travel insurance, such as in European and American countries. The amount of premium to be paid depends on the desired coverage, travel duration, and travel destination. An insurance company operating in the travel insurance sector wants to identify potential policyholders who are likely to make insurance claims in order to provide them with the necessary coverage. The policyholder data in the insurance company's records includes travel destinations, insurance products, and other relevant information.

**Target**: 'Claim'<br>
- 0: No claim filed   
- 1: Claim filed

**Problem Statement**: <br>
The company aims to improve the efficiency of the travel insurance claim process by leveraging historical policyholder data to identify policyholders who are likely to file claims and require coverage. This will enable the company to optimize its resources. Previously, the company offered insurance to everyone through a third party without any selection criteria, resulting in financial losses for the company, as they were unaware of whether the individuals they were offering insurance to would actually file claims or not.

**Goals**: <br>
Based on this problem, the company aims to have the ability to predict the likelihood of a prospective policyholder filing a claim. This will prevent financial losses for the travel insurance company, as they will be able to determine in advance if the prospective policyholder is likely to file a claim.

**Analytical Segmentation**: <br>
Therefore, my approach will involve analyzing the data to identify patterns that differentiate policyholders who file claims from those who do not (classification). I will then build a classification model that will help the company predict the probability of a policyholder filing a claim or not.

**Metric Evaluation**

![metrics.png](metrics.png)

Type 1 error: False Positive. The model predicts that a customer will file a claim, but in reality, they do not. This results in the company losing potential customers as they are not offered insurance policies.

Type 2 error: False Negative. The model predicts that a customer will not file a claim, but in reality, they do. This requires the company to pay unexpected claim expenses.

Based on the company's request, my main focus is on identifying customers who are truly likely to file a claim. Although both errors are important, I prioritize avoiding False Negatives over False Positives. In this context, the most suitable metric is **Recall**.

Recall is a metric that measures how well the model accurately identifies customers who will file a claim. In this case, False Negatives have a more significant impact because the company incurs losses if it fails to identify customers who will actually file claims.

Therefore, in the evaluation of the model, I will pay attention to and compare the Recall values to ensure that the model's ability to identify customers who will file claims (True Positive) is very high, and the occurrence of False Negatives is minimized.
