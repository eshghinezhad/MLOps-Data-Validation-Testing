 MAI201 MLOps - Assignment 2 Report – Data Validation & Testing
**Name:** Monireh Eshghinezhad  **06/26/2026** 
-----------------------------------------------------------------
**1. Great Expectations Validation Results:**

<img width="1827" height="162" alt="Screenshot 2026-06-26 180154" src="https://github.com/user-attachments/assets/7c3008e2-5893-4f91-82fc-9a2fa5372ebf" />
<img width="1744" height="1284" alt="Screenshot 2026-06-26 180422" src="https://github.com/user-attachments/assets/e8653654-1ccc-4a4c-ae69-77646900bd64" />
<img width="1636" height="1006" alt="Screenshot 2026-06-26 180458" src="https://github.com/user-attachments/assets/c71c6b66-45af-4c15-908e-29415d36b927" />


----------------------------------------------------------------------------------------------------------
**2. Data Quality Issues Found:**

After running the validation, there was following issues in the dataset:

<img width="1753" height="1505" alt="image" src="https://github.com/user-attachments/assets/c0ccbff2-0ddf-4927-b233-e7bef0efde8e" />
<img width="1674" height="1186" alt="image" src="https://github.com/user-attachments/assets/da1479e0-8a9e-468f-80ee-625e9cc905ac" />


------------------------------------------------------------------------------------------------------------
**3. pytest Test Results:**

<img width="1746" height="740" alt="image" src="https://github.com/user-attachments/assets/f2302f9a-b1c5-4870-b654-f9f408d78ffb" />

-------------------------------------------------------------------------------------------------------------
**4. Reflection Which Data Quality Issue Would Most Impact ML Model Performance?**

In my opponion **missing data** (null/NaN values) is the data quality issue with the most impact on ML model performance, becuase:

Most ML algorithms cannot handle NaN values at all and the functionality of the system will be broke.
When we fill missing values with mean, median, mode, or even imputation, we are making assumptions about the data which leading to biased predictions.
Missing data corrupts feature distributions, and can affects all other steps.
In addition I think bad numeric values that are out of range are also dangerous in ML because they can mess up feature scaling, affect model weights, and make the overall predictions less accurate without any obvious error showing up.
