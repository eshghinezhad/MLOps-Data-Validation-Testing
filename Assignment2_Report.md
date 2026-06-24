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

In my opinion, the **age column** having values like 999 would cause the problems for a machine learning model.
Age is a numeric feature that a model uses directly in calculations. If the model sees an age of 999 during 
training, it will treat that as a real value and learn wrong patterns from it. For example, if we are building 
a model to predict customer behavior, a 999-year-old customer would completely confuse the model and pull predictions
in the wrong direction. This is different from something like a missing salary or a badly formatted email. Those can 
be handled by dropping or filling in missing rows. But an age of 999 does not look like a missing value, it looks 
like a real number,so the model might not even know it is wrong.

Bad numeric values that are out of range are especially dangerous in ML because they can mess up feature scaling, affect model weights, and make the overall predictions less accurate without any obvious error showing up.
