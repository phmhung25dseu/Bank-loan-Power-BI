# Bank Loan 
![image](https://github.com/user-attachments/assets/95c83101-b68c-4fd3-b92f-d848bdbf8884)
## I. Introduction

This project focuses on a comprehensive analysis of loan data to uncover trends, regional variations, and the influence of employment duration on loan outcomes. A key objective is to distinguish between good and bad loans, supporting more accurate risk assessments.

Our primary goal is to support data-driven decision-making in loan approvals by building a robust reporting system and identifying critical performance indicators. Through this analysis, we aim to enhance the efficiency of the loan approval process, reduce risk exposure, and improve overall portfolio quality.
## II. Data Dictionary
| Column Name             | Description                                                                                   | Data Type |
|-------------------------|-----------------------------------------------------------------------------------------------|-----------|
| `Id`                    | Unique identifier for each loan record.                                                       | int       |
| `Address_state`         | Borrower's state of residence.                                                                | varchar   |
| `Application_type`      | Type of applicant: Individual or Business.                                                    | varchar   |
| `Emp_length`            | Duration of borrower's employment (e.g., 10+ years). Reflects job stability.                  | varchar   |
| `Emp_title`             | Borrower's job title or occupation.                                                           | varchar   |
| `Grade`                 | Loan grade classification indicating creditworthiness.                                        | varchar   |
| `Home_ownership`        | Borrower's home ownership status (e.g., Rent, Own, Mortgage).                                 | varchar   |
| `Issue_date`            | Date when the loan was issued.                                                                | date      |
| `Last_credit_pull_date` | Most recent date the borrower's credit report was pulled.                                     | date      |
| `Last_payment_date`     | Most recent loan payment date.                                                                | date      |
| `Loan_status`           | Current status of the loan (e.g., Fully Paid, Current, Default).                              | varchar   |
| `Next_payment_date`     | Scheduled date for the next loan payment.                                                     | date      |
| `Member_id`             | Unique identifier for the borrower.                                                           | int       |
| `Purpose`               | The stated purpose of the loan (e.g., credit card, education).                                | varchar   |
| `Sub_grade`             | Finer classification within the loan grade.                                                   | varchar   |
| `Term`                  | Loan term in months, defining the repayment duration.                                         | varchar   |
| `Verification_status`   | Indicates if the borrower's financial information has been verified.                         | varchar   |
| `Annual_income`         | Borrower's total annual income. Used to evaluate repayment ability.                          | int       |
| `Dti`                   | Debt-to-income ratio. Measures debt load relative to income.                                 | int       |
| `Installment`           | Fixed monthly repayment amount including principal and interest.                             | int       |
| `Int_rate`              | Interest rate on the loan (annual percentage rate).                                           | int       |
| `Loan_amount`           | Total amount of money borrowed (principal).                                                   | int       |
| `Total_acc`             | Total number of credit accounts the borrower holds.                                           | int       |
| `Total_payment`         | Total amount to be repaid over the life of the loan (principal + interest).                   | int       |

## III. Design thinking
![image](https://github.com/user-attachments/assets/4cab5253-a5fa-4287-aac7-10c903c395ed)
![image](https://github.com/user-attachments/assets/617d0721-b3c1-4c28-b06a-52f7469a2372)
![image](https://github.com/user-attachments/assets/5d95e5e0-243f-4c0f-a518-39f003d4cb4b)
![image](https://github.com/user-attachments/assets/abc1c0d2-4fea-4608-8c6c-bd506271e6c4)
![image](https://github.com/user-attachments/assets/0c1eb75f-ef77-4151-8785-106b0862f202)
![image](https://github.com/user-attachments/assets/0023951a-b5d4-4843-81eb-4893ef0ccab7)

## III. Visualization
### 1. Overview Loan
![image](https://github.com/user-attachments/assets/1da50c02-1f7e-4352-8450-fdb4da3d47c4)
### ✅ Insights
#### 1. Loan Volume and Growth
- **Total Funded Loans** reached **$435.76M in 2021**.
- Loan volume increased steadily month over month, with a strong year-end performance at **$53M+ in December**.
- **MoM Growth** in funded loans is **13.04%**, indicating increasing customer demand or successful loan campaigns.

#### 2. Loan Purpose Distribution
- **Debt Consolidation** is the dominant loan purpose, accounting for **$232.5M (~53%)** of total funded loans.
- **Credit Card**, **Home Improvement**, and **Other** also represent significant portions.
- Less demand observed for **Car** and **Wedding** loans.

#### 3. Loan Term Trends
- **60-month loans** are more popular, comprising **62.66%** of the total amount, suggesting a borrower preference for longer repayment periods.

#### 4. Verification Status
- About **45.2%** of loans were **source verified**.
- **32.06%** were **not verified**, raising potential credit risk concerns.
- Only **22.74%** were verified through standard means.

#### 5. Geographic Distribution
- **California (CA)** leads with **$78.5M**, followed by **New York (NY)** and **Texas (TX)**.
- Some states (e.g., **PA**, **VA**) contribute less but may offer **growth opportunities**.

#### 6. Key Financial Metrics
- **Total Amount Received** exceeded total funded, indicating **high repayment performance**.
- **NPL Ratio** (Non-Performing Loan) is at **13.82%**, slightly improved MoM, but still notable.
- **Average DTI** stands at **13.33%**, indicating relatively manageable debt levels among borrowers.

### ✅ Recommendations

#### 1. Risk Mitigation through Verification
- Increase the proportion of **verified** or **source-verified** borrowers to reduce default risks.
- Implement **stricter verification procedures**, especially for high-value or long-term loans.

#### 2. Loan Product Focus
- Strengthen offerings in **debt consolidation** and **credit card refinancing**, which have the highest uptake.
- Evaluate **underperforming categories** (e.g., wedding, car) for potential discontinuation or repositioning.

#### 3. Geographic Expansion
- Explore **market expansion** in states with lower loan volumes but economic growth potential (e.g., **PA**, **VA**, **NJ**).
- Consider **localized marketing campaigns** and **partnerships** in those regions.

#### 4. Optimize Loan Term Strategy
- Monitor the performance of **60-month loans** closely, especially their impact on delinquency rates.
- Consider **incentives** for borrowers to opt for **36-month terms**, which may carry lower risk.

#### 5. Improve NPL Ratio
- Identify **common characteristics of defaulted loans** and refine approval criteria accordingly.
- Introduce **early-warning systems** or **predictive modeling** to flag at-risk accounts.

### 2. Customer Analysis
![image](https://github.com/user-attachments/assets/3d3af49c-78c8-488e-bb1f-2188a78980c6)

### 🔍 Insights

#### 1. Loan Application Volume
- A total of **38.58K loan applications** were submitted in 2021.
- Application volume steadily increased each month, peaking toward year-end (~4K per month in Q4), suggesting growing customer engagement or **seasonal loan demand**.

#### 2. Income and Loan Size
- The **average applicant income** is **$69.64K**, while the **average loan size** is **$11.30K**, reflecting **conservative borrowing behavior** relative to income.

#### 3. Loan Term Preferences
- **73.2%** of applicants chose the **36-month term**, while only **26.8%** opted for the **60-month term**, indicating a **preference for quicker debt resolution**.

#### 4. Home Ownership Breakdown
- The majority of applicants either **own (47.8%)** or have a **mortgage (44.58%)**.
- Only **7.36%** are **renting**, which may reflect higher credit risk or a younger borrower segment.

#### 5. Employee Duration Impact
- Employees with **2–5 years** of tenure account for the **largest loan volumes** (over **$160M**), implying a sweet spot of **employment stability and financial need**.
- Loan volume drops significantly for applicants with longer job tenures (**6+ years**), especially **9 years or more**.

#### 6. Loan Grade Distribution
- The highest total loan amount is concentrated in **Grade B ($131M)**, followed by **Grade C ($87M)** and **Grade A ($84M)**.
- **Grades F and G** contribute minimally, possibly due to **credit risk restrictions**.

### ✅ Recommendations

#### 1. Target Mid-Tenure Employees
- Focus marketing and approval strategies on applicants with **2–5 years** of employment duration.
- They demonstrate both **stability** and **strong borrowing activity**.

#### 2. Strengthen Grade B-C Loan Management
- Since **Grade B** holds the highest exposure, enhance **risk monitoring** and **servicing** for this group.
- Assess **Grade C** loan behavior for potential **promotion to Grade B incentives** or **early repayment strategies**.

#### 3. Loan Term Incentives
- Since most customers prefer **36-month terms**, consider offering **rate discounts** or **faster approval** to encourage this choice.
- For riskier borrowers, **steer toward 36-month terms** to limit long-term exposure.

#### 4. Refine Home Ownership-Based Offers
- Homeowners (own/mortgage) represent over **92%** of applicants.
- Develop specific offers for this segment such as **home improvement loans** or **equity-backed products**.

#### 5. Upsell Opportunity for Low Average Loan Size
- With an average loan amount of only **$11.3K**, there’s room to **cross-sell** or **bundle loan products** to qualified borrowers with higher income or lower DTI.

#### 6. Support for Grade F and G Applicants
- Instead of declining, consider **credit-building micro-loans** or **secured loans** for Grades **F and G** to expand reach while controlling risk.

### 3. Credit Analysis
![image](https://github.com/user-attachments/assets/46884603-121e-41f8-883c-e7c33d20ac1f)
### 🔍 Insights

#### 1. Loan Quality Distribution
- **Good loans** account for **86.18%** of all applications (**33.24K**), while **bad loans** represent **13.82%** (**5,333**).
- This is a **solid overall performance**, but bad loans are still significant in both **volume and value**.

#### 2. Financial Impact
- **Good Loan Funded Amount**: **$370.22M**
- **Bad Loan Funded Amount**: **$65.53M**
- Only **$37.28M** of bad loans have been recovered, implying **$28.25M in potential losses**.

#### 3. Loan Status Overview
- **Fully Paid Loans**: **$351M**
- **Charged Off (Bad Loans)**: **$66M**
- **Current (Active) Loans**: **$19M**
- The high proportion of **fully paid loans is encouraging**, but the **charged-off segment is 15.1%** of total funded value.

#### 4. Bad Loans by Homeownership
- **Renters** account for **50% (2.69K)** of bad loans.
- **Mortgage holders**: **2.23K**
- **Homeowners**: Only **0.4K** bad loans
- Indicates **higher risk among renters and mortgaged applicants**.

#### 5. Average Interest Rate by Loan Status
- **Bad loans (Charged Off)**: **13.88%**
- **Good loans (Fully Paid)**: **11.64%**
- Suggests **higher interest rates correlate with higher default risk**.

### ✅ Recommendations

#### 1. Tighten Criteria for High-Risk Groups
- Strengthen credit evaluation for **renters and mortgaged applicants**, as they form the bulk of **charged-off loans**.
- Require **additional income or DTI documentation** for these segments.

#### 2. Reassess High-Interest Loans
- Loans with **interest >13%** show higher default rates.
- Revisit **pricing models** to better reflect risk.
- Offer **rate discounts** or **incentives** for borrowers with stronger profiles to **lower default exposure**.

#### 3. Enhance Early Warning Systems
- Use **predictive analytics** based on employment duration, loan purpose, and verification status to **flag high-risk accounts early**.
- Implement **automated alerts** for missed or delayed payments.

#### 4. Recovery Strategies
- For the **$28M+ in unpaid charged-off loans**, apply **targeted collection efforts** or **settlement offers** for partial recovery.
- Segment bad loans by **homeownership and employment profile** to tailor outreach.

#### 5. Periodic Policy Adjustments
- Conduct **quarterly reviews** of bad loan data to refine approval thresholds.
- **Retrain risk models** regularly using the **latest loan performance data**.

## IV. Recommendation

### 🔍 Key Insights

#### 1. Loan Performance Overview
- **Total Applications**: 38,576  
- **Good Loans**: 86.18% (33.24K applications)  
- **Bad Loans**: 13.82% (5,333 applications)  
- **Fully Paid Loans**: $351M | **Charged Off**: $66M  
- High repayment performance is seen, but a **13.82% charge-off rate** presents a **non-trivial risk exposure**.

#### 2. Loan Purpose & Demand Trends
- Most borrowed for **Debt Consolidation** ($232.5M), followed by **Credit Card** and **Home Improvement**.
- Loan demand **increases consistently** through the year, with **peak volume in Q4 2021**.
- **Average Loan**: $11.3K | **Average Income**: $69.64K — suggests **conservative borrowing behavior**.

#### 3. Loan Term & Repayment Behavior
- **60-month loans** account for **62.66%** of total funded volume, though **36-month loans** are more popular by count.
- **Bad loans** have **higher interest rates** (avg. 13.88%) compared to **good loans** (11.64%), implying a **correlation between pricing and risk**.

#### 4. Customer Profile & Risk Factors
- Borrowers with **2–5 years employment** contribute the **highest loan volumes**, suggesting this is a **sweet spot for stable lending**.
- **Grade B loans** dominate ($131M), while **Grades F/G** contribute the least (likely representing **higher risk**).
- **Renters** represent **50%+ of bad loans**, followed by **mortgaged borrowers**. **Homeowners** have far fewer defaults.

### ✅ Strategic Recommendations

#### 1. Enhance Risk Control & Mitigation
- **Prioritize verification**: Source-verified loans outperform others. Increase **automation** and enforcement of verification standards.
- Introduce **creditworthiness scoring thresholds** for high-risk groups (e.g., renters, low-tenure employees, unverified applicants).

#### 2. Product & Pricing Optimization
- **Refine interest rate models**: High-interest loans correlate with charge-offs. Implement **dynamic pricing** based on real-time risk assessments.
- Promote **36-month terms** with better rates to encourage **faster repayment** and **lower long-term risk**.

#### 3. Targeted Lending Strategy
- Focus on borrowers with **2–5 years of employment** — they offer a balance of **income stability** and **loan demand**.
- Expand geographically in **mid-tier performing states** (e.g., **NJ**, **VA**) to **balance portfolio exposure** and **capture growth potential**.

#### 4. Reduce Charge-Offs and Improve Recovery
- Develop **early-warning systems** using behavioral and employment data to flag risky accounts.
- Initiate **special collections plans** for high-value defaults and explore **settlement strategies** to recover part of the **$28M+ in losses**.

#### 5. Improve Loan Product Bundling
- Leverage insights on **home improvement**, **credit card**, and **small business loans** to **cross-sell or upsell**.
- Launch **personalized loan offers** based on borrower profile (income, employment, loan purpose) to increase **wallet share**.













