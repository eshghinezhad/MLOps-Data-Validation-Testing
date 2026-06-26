 MAI201 MLOps - Assignment 2 Report – Data Validation & Testing
**Name:** Monireh Eshghinezhad  **06/26/2026** 
-----------------------------------------------------------------
**1. Great Expectations Validation Results:**

<img width="1701" height="607" alt="image" src="https://github.com/user-attachments/assets/329cb9ba-601b-4c67-9f21-a0dfc520136c" />


**2. Data Quality Issues Found:**

After running the validation, I found the following issues in the dataset:

<img width="1352" height="1529" alt="image" src="https://github.com/user-attachments/assets/aaaf9f4b-638f-433a-bc50-ba8fc88fc8e9" />
<img width="1219" height="346" alt="image" src="https://github.com/user-attachments/assets/15483b57-16fa-421d-afc1-74f30ad0470d" />




**3. pytest Test Results:**

<img width="1396" height="757" alt="image" src="https://github.com/user-attachments/assets/1555f886-1925-41ec-bb98-6466ae39e362" />


**4. Reflection**
**Which Data Quality Issue Would Most Impact ML Model Performance?**

In my opponion **missing data** (null/NaN values) is the data quality issue with the most impact on ML model performance, becuase:
- Most ML algorithms cannot handle NaN values at all and the functionality of the system will be broke.
- When we fill missing values  with mean, median, mode, or even imputation, we are making assumptions about the data which leading to biased predictions.
- Missing data corrupts feature distributions, and can affects all other steps.

In addition I think bad numeric values that are out of range are also dangerous in ML because they can mess up feature scaling, affect model weights, and make the overall predictions less accurate without any obvious error showing up.
