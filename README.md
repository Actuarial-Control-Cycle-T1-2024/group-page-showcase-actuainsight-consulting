# Actuarial Theory and Practice A @ UNSW

---
# 2024 ACTL4001 SOA Challenge: SuperLife Saving Lives
![](LifeInsurance.gif)

---
The University of New South Wales

Team: ActuaInsight Consulting

Members: Karan Deshwal, Luis Alvarez, Arneet Kalra, Anoushay Khan and Tom Mihaljevic

**Please refer to [initial repository](https://github.com/Tomathy123/ACTL4001) for full commit history and member contributions.**

---

## Executive Summary
Actualnsight, an actuarial consulting firm, has been engaged by SuperLife, a life insurance agency, to enhance its policyholders' expected mortality. In response, our team has devised four incentive programs: a smoking cessation program, annual health screenings, an active aging initiative, and a fitness tracking program. The primary objectives of these programs are to incentivize healthy behaviours, decrease expected mortality, increase sales, improve marketability, and add economic value to SuperLife.

The proposed program design is rooted in data analysis at the policyholder level, ensuring tailored interventions for maximum effectiveness. Short-term and long-term evaluations have been delineated for each incentive to gauge program efficacy, participant engagement, and health outcomes over time.

Mortality rates were calculated for four cohorts: male smokers, male non-smokers, female smokers, and female non-smokers, providing essential insights for premium determination. Premium calculations were executed in R, followed by financial modelling in Excel.

Risk and risk mitigation considerations have been intricately woven into the report to proactively address potential challenges and uncertainties. Given the inherent limitations and uncertainties of the data, various assumptions were made based on internal data and supplementary research, with detailed rationale and analysis provided in the Appendix. These measures ensure a robust and resilient program implementation strategy.

## 1. Objectives
### 1.1 Background
The proposed targeted health incentives in SuperLife’s life insurance policies are designed to ensure that SuperLife’s policyholders have an improved expected mortality after the policyholder has purchased a life insurance policy. The health interventions/incentives aim to increase healthy behaviours through participation, decrease expected mortality and add economic value to SuperLife through improved marketability and competitiveness as that would increase sales of their long-term life insurance products. More details below.
### 1.2 Objectives
A) Incentivise healthy behaviours through the product design.
- Smoking Cessation Program
- Annual Health Screenings (includes Heart Health, Lung Health, and Cancer Prevention Initiatives)
- Active Ageing
- Fitness Tracking Program
- Decrease expected mortality rates.
- Healthy behaviours from incentives should lead to lower mortality rates.
- Increased healthy behaviours leads to reductions in policyholder mortality.
- Enhance product marketability and competitiveness.
- Promotion of health programs improves marketability.
- Decreased expected mortality rates would lead to more competitive premiums.

B) Increase sales of life insurance policies.
- Improvements in marketability and competitiveness should lead to increased sales of life insurance policies.

C) Add economic value to SuperLife's offerings.
- More policies imply more premiums and hence sustained profits in the long term.

### 1.3 Program Metrics
The program’s success will be assessed using the following targets:
| Incentive Participation Rates | Customer Satisfaction Surveys  | Increase in SuperLife's Economic Value |
|-------------------------------|--------------------------------|----------------------------------------|
| **Claims Frequency**          | **Policy Sales**               | **Reduced Mortality Rates**            |

## 2. Product Design
The primary objective of life insurance is to protect policyholders from the risk of premature death. The team at Actualnsight has carefully designed the following programs to ensure that SuperLife is not only covering policyholders from such risks but also to actively mitigate risk. The product design incorporates four primary interventions/incentives, meticulously derived from data-driven insights based on policyholder-level data analysis.

Due to the distinct nature of the two products offered by SuperLife, certain programs may be more applicable for either policy type. However, due to the unknown nature of applicability, the program intervention currently assumes equal effectiveness and participation across both policy types. This assumption is a key consideration in the Short Term and Long-Term monitoring processes.

### 2.1 Smoking Cessation Program
Cigarette smoking can have adverse impacts on the human body in the long term and opens avenues for multiple diseases that can be of great severity. According to the National Library of Medicine (2020), smoking causes a 70% increase in risk for adverse health conditions. This is evident in the data as the death rate for smokers is approximately 8x higher than non-smokers as seen in Figure 2 (appendix).

SuperLife’s Smoking Cessation Program will work with qualified professionals to help their policyholders quit smoking for the better. Research reports have demonstrated that smoking cessation improves well-being, including higher quality of life and improved health status. Smoking cessation reduces mortality as it lowers the risk of smoking-induced health complications (National Library of Medicine, 2020). The most common causes of death for smokers are diseases of the circulatory and respiratory system (86% of smoker deaths) as seen in Appendix Figure 4 while the most common causes of death for non-smokers are Neoplasms and external causes (60% of non-smoker deaths) as seen in Appendix Figure 5. It is evident that through a smoking cessation program, the likelihood of deaths due to diseases in the circulatory/respiratory system can be significantly reduced.

In terms of participation, it is estimated that 81% (Tobacco in Australia, 2020) of smokers in a developed country attempted to quit smoking. Considering behavioural bias and assuming a person who insures themselves from premature death would also take steps to reduce the risk, the 81% can be inflated. By providing an avenue within the policy such that the policyholders have access to free expert services, we believe this would incentivise policyholders to participate in the program. Quitting smoking has been proven to result in improved well-being and health status, allowing policyholders to live happier and longer lives (in expectation).

Policyholders who participate in the program will go through a structured approach, optimising their aim to quit smoking.
- **Counselling from health professionals** : giving further reasons to quit that could be specific to the policyholder and their medical condition.
- Cessation medications (if required) to overcome the addiction.
- Continuous follow-up support to avoid relapse from a care team ensures efficiency and a coordinated care approach.

Finally, from SuperLife’s perspective, currently, all smokers are classified as moderate to high risk in the Underwriting Classifications as seen in Figure 3 Underwriting Class Distribution by Smoking Class. Through the Smoking Cessation Program, SuperLife will be able to reduce their high frequency and high severity risks. This allows the program to be mutually beneficial, assisting both parties.

**Short-Term and Long-Term Program Evaluation:**

- **Short-term Evaluation (1-2 years):** The program can be evaluated based on metrics such as attendance rates and reported smoking cessation rates, which would demonstrate effectiveness. This timeframe allows for assessing initial program effectiveness with data available on a potentially new cohort of policyholders and allows identification of any challenges and requirements based on stakeholder experience.
- **Long-term Evaluation (5-7 years):** Long-term evaluation is essential for measuring sustained behaviour change and its impact on mortality rates as they are assumed to be refreshed every 4 years. Tracking participants over a longer period allows for observing long-term smoking cessation outcomes and determining the program's overall effectiveness in reducing mortality associated with smoking-related illnesses.

### 2.2 Annual Health Screenings
Annual health screenings, particularly focusing on cardiovascular and oncological prevention, are pivotal in mitigating mortality rates. Empirical evidence underscores the efficacy of regular health screenings in reducing mortality. A study conducted on a Korean cohort (pg. 19-25, Preventative Medicine, 2015) observed a marked decrease in all-cause mortality and cardiovascular disease (CVD) rates among participants of regular health screenings. Notably, this study reported an increased detection rate of CVD-related conditions and a subsequent reduction in long-term healthcare utilisation and costs, an objective of SuperLife.

SuperLife’s Annual Health Examination Program aims to collaborate with healthcare facilities to offer comprehensive screenings, assessment, and risk stratification. This initiative focuses on early detection of neoplasms (both benign and malignant), and conditions related to the circulatory and respiratory systems, among other non-lethal health issues. These conditions are among the leading causes of fatality in the data presented in Figure 4 and Figure 5, and approximately 63% of policyholders who died from the above conditions are situated in the moderate to high-risk bracket. By facilitating early-stage intervention, the program aims to prevent the progression of these diseases.

An integral component of the initiative is to offer subsidised medical coverage for early-stage oncological interventions, emphasising the surgical removal of neoplastic growths to halt their progression and thereby significantly enhance patient survival rates, as depicted in the American Journal of Managed Care (2019).

Furthermore, the program enriches patient care with follow-up check-ups and a suite of support services, including disease abstinence programs. This initiative is critical for enhancing treatment plan adherence, fostering healthier lifestyles, and improving the overall quality of life for participants.

Policyholders who participate in this program will have access to the following incentives:
- **Affordable Health Screenings:** The program aims to overcome economic barriers and the impact of the COVID-19 pandemic on medical systems, ensuring widespread access to crucial health services.
- **Comprehensive Screening Facilities:** Offering wide-ranging disease and risk factor screenings, the program supports early health issue detection through a holistic assessment approach, aimed at preventing and managing health conditions effectively.
- **Enhanced Longevity through Early Detection:** Focused on early detection, intervention, and preventive measures, the program aims to improve quality of life, individual health status and extend life expectancy by reducing the risk of disease progression and mortality.

**Short-Term and Long-Term Program Evaluations:**
- **Short-Term Evaluations (1-3 Years):** Within the initial 1 to 3 years, the focus would be on metrics like participation rates, satisfaction surveys and early detection rates that can provide immediate feedback on the program’s operational effectiveness and its early impact on participant health behaviours. This is critical for identifying areas of success and opportunities for improvement in the program’s design and delivery. See Appendix 8.1.2 Annual Health Screenings for further details.
- **Long-Term Evaluations (6-8 Years):** Over a longer horizon of 6 to 8 years, the evaluation shifts towards assessing the program’s overarching goal of reducing mortality and morbidity rates among participants, healthcare utilisation and cost analysis, the broader health behaviour changes at the population level and monitoring prevalence of conditions detected through the program’s screenings. See Appendix 8.1.2 Annual Health Screenings for further details.

### 2.3 Active Ageing
During the later phases of life, it is imperative to remain active as it keeps one physically and mentally fit. Regular exercise has also shown to reduce the probability of a person contracting cardiovascular diseases by 60-70%. Furthermore, regular exercise has also assisted in lowering the risk of cancer due to the regulation of hormones like insulin which implies a reduced exposure to potential carcinogens.

From the explanatory analysis it was found that the top three causes of death for policyholder’s aged 55 and over were: Neoplasms (potentially cancerous) (36%), Diseases of the Circulatory System (32%) and Diseases of the Respiratory System (8%) as seen in Figure 6. These deaths also account for approximately two-thirds of all deaths.

Further analysis has also shown that almost two-thirds of the policies were issued for policyholders between the ages of 35 and 55, as shown in Figure 7. As such, it was realised that the introduction of an Active Ageing Program will be able to transition majority (assuming high participation) of the policyholders into lower risk classes as they age and surpass the age of 55. Resultantly, the mortality is expected to decline by proactively mitigating or averting the predominant causes of mortality among the aging demographic, thereby extending life expectancy significantly.

Active ageing programs not only promote physical activity but also increase social engagement and mental stimulation. Given the demographic of Lumaria where approximately 90% of the population works in the industry or services sector it is assumed that a program like active ageing will have high perceived benefits and thus a high level of participation within both the rural and urban demographic.

The programs key features would include:
- Voluntary participation through registrations for free/subsidised classes with industry partners and government organisations. This allows of rural and urban availability.
- An emphasis on physical activity, active learning and supportive environments facilitating positive attitudes and wellbeing.
- Promotion of health, maintenance, and independence through learning within the classes.

Overall, these program features would allow the ageing policyholders to be physically fit and aware of their bodies. This would tie in with the healthcare program that SuperLife would offer based on our advice creating a holistic system of healthcare.

**Short-Term and Long-Term Program Evaluations:**
- **Short-Term (6 months - 1 year):** In the short-term SuperLife should investigate the participation rates and how actively policyholders are enrolling for the program. Additionally, utilising the annual healthcare program offered simultaneously would allow SuperLife to assess any immediate benefits in policyholder health. Surveys are to be conducted to measure policyholder satisfaction with program features, allowing for adjustments to be made.
- **Long Term (>1 Year):** In the long term it would be important for SuperLife to assess the exact health outcomes by looking at potential improvements in parameters like fitness levels, and chronic disease risks. Additionally, a strong part of the program is to improve policyholder wellbeing and thus it would be important to monitor and measure perceived wellbeing improvements. Finally, risk reduction, cost savings and retention rates are important factors to evaluate program effectiveness.

### 2.4 Fitness Tracking Program
The relative risk of death is approximately 20-35% lower for people who are physically active and fit compared to sedentary people (National Library of Medicine, 2012). As such, the final incentive that is part of the program design is the fitness tracking program which will provide rewards for policyholders using fitness trackers to monitor and improve physical activity. The program primarily aims to reach out to the current/future young demographic of Lumaria and incentivise healthy behaviours using technology. Additionally, the program allows both the urban and rural populations to stay healthy and get rewarded at their own ease.

Key features of the program include:
- Policyholders who participate will have to provide SuperLife access to their health data through their personal devices.
> - Would include metrics like physical activity (through exercise regime), heart rate and sleep cycle.
> - Such data will allow SuperLife to obtain a clear image of policyholder lifestyle and their likelihood of developing any adverse illness.

- Policyholders will be able to choose their goals and will be rewarded accordingly (relative to what their initial health status might be).
> - Currently, the rewarding system is consistent for all policyholders, however, this is planned to change post the initial monitoring phase.

Even though the program is designed for the younger generation, it was also found that approximately two-thirds of the population in each of Lumaria’s regions are classified as living in an urban area (inforce data) as seen in Figure 8. As such, it is expected that the program is more effective in the urban areas where the likelihood of wearing/owning devices to track everyday health is assumed to be higher.

## 3. Pricing/ Costs

### 3.1 Mortality Savings
From our mortality calculations, we observe a decline in the overall mortality rates for both males and females in the presence of incentives within the policy calculations, across all cohorts of smokers and non-smokers. This trend is illustrated in Appendix Table 5 with its methodology, which presents the mortality tables for both genders in both scenarios.

*Table 1: Average Mortality Savings for all ages based on scenarios for SPWL*
|                  | MNS            | MS             | FNS            | FS             |
|------------------|----------------|----------------|----------------|----------------|
|   Low Cost       |   - Č 26,307   |   - Č 96,681   |   - Č 15,455   |   - Č 61,072   |
|   Average Cost   |   - Č 14,780   |   - Č 95,594   |   - Č 12,778   |   - Č 60,712   |
|   High Cost      |   - Č 7,912    |   - Č 94,887   |   - Č 11,185   |   - Č 60,464   |

*Table 2: Average Mortality Savings for all ages based on scenarios for T20*
|                  | MNS              | MS                | FNS              | FS                |
|------------------|------------------|-------------------|------------------|-------------------|
|   Low Cost       |   - Č 2,482.67   |   - Č 12,478.98   |   - Č 1,624.42   |   - Č 10,269.04   |
|   Average Cost   |   - Č 2,494.60   |   - Č 12,277.19   |   - Č 1,642.62   |   - Č 10,029.02   |
|   High Cost      |   - Č 2,498.87   |   - Č 12,052.69   |   - Č 1,652.72   |   - Č 9,771.81    |

Table 1 and Table 2 illustrate the average mortality savings across all ages (1 to 120) based on four cohorts for T20 and WLI policies. For calculation details, see Appendix 8.2.3 Mortality difference (Baseline vs Incentive). Our model examines three distinct cost scenarios and juxtaposes the mortality savings with three corresponding cost profiles associated with the incentives: lower, average, and maximum costs derived from each implemented incentive within our policy framework.

While the values are negative, from the company's standpoint, these signify the savings accrued to policyholders due to program incentives. This is attributable to the following reasons:

1. **Mortality saving through Pure Premiums:** Decreases in mortality rates directly impact the pure premium component of our insurance policies. As policyholders enjoy extended lifespans, the associated mortality risk diminishes, prompting a downward adjustment in pure premium rates to reflect this reduced risk exposure. Lower mortality rates require smaller allocation of funds to cover potential payouts, and lead to more competitive pricing.

2. **Mortality saving through Profit:** Lower mortality rates have the potential to increase the profitability of insurance firms. The anticipation of fewer payouts due to prolonged policyholder lifespans enables the retention of a larger share of premium income as profit. Despite the apparent negativity in both profit figures, the introduction of incentives results in an overall profit increase. The negative profit metric is contingent upon various factors including investment returns, administrative overheads, and prevailing market competition.

### 3.2 Economic Value of Proposed Program
For the economic value of the proposed program into the future, we have looked at how policies will reduce the pure premium of SuperLife’s insurance products and whether costs of the program will be able to be subsidized by the premiums.

We have projected ahead by 20 years, to 2043 and have considered the following factors:

1. Increases in number of policyholders: Analysing historical data on the yearly acquisition of new policyholders allows for the prediction of future growth in the total number of policyholders.
   
2. Changes to participation rates: It is expected that participation rates will increase as policyholders move to take advantage of the benefits that come with their policy and also allows us to stress test whether the programs are economically viable.

3. Different cost scenarios: Three different scenarios have been examined, each with different assumptions regarding costs per policyholder.

On average pure premiums are found to be reduced by Č 9412 for WLI and Č 3186.55 for T20 policies. The expected reduction in premium due to the program intervention enables the adjustment of base premiums to cover program costs, whist still being lower than the original premium. Policyholders will experience a reduction in their premiums while also enjoying the benefits of the program.

*Table 3: T20 and WLI New Premium + Costs Difference*
|                  | WLI           | T20           |
|------------------|---------------|---------------|
|  Low Cost        |   Č 9066.56   |   Č 2842.17   |
|   Average Cost   |   Č 8443.82   |   Č 2220.76   |
|   High Cost      |   Č 7821.08   |   Č 1599.36   |

This analysis indicates that the value of policy benefits with the program surpasses the value of policy benefits without the program, demonstrating the economic viability of the design.

### 3.3 Pricing Changes
The following recommendations aim to optimise sales and policy value by implementing strategic pricing adjustments within the insurance company's financial model.

1. **Profit Margin Assessment:** Examine the current profit margin of our existing policies and pricing structure with the goal to identify where adjustment can be made to boost profitability while still staying competitive and retaining our valued customers. This can be done through the evaluation of the loss ratio of each policy by dividing incurred claims by earned premiums. If the loss ratio is higher than desired or expenses are excessive, then premiums might need to be increased to improve profitability.

2. **Value-Based Pricing:** Implementing value-based pricing methods involves aligning insurance policy premiums with the perceived value to customers, considering factors like coverage scope, service quality, brand reputation, and supplementary benefits. One way to do this is by estimating the price elasticity of demand. We can use econometric models like linear or log-linear regression, which analyse baseline premiums, sales data, and additional variables to project price elasticity of demand. This comprehensive approach enables informed pricing decisions, optimizing market performance by ensuring premiums accurately reflect customer value and drive policy sales.

## 4. Assumptions
The following mortality and model assumptions had the most significant impact on analysis as they directly affect the pricing and profitability of the program design.

### 4.1 Mortality Assumptions
Mortality analysis in Lumaria is essential in understanding policyholder characteristics and behaviours, enabling SuperLife to price products with precision, particularly in relation to sex and smoker status. Due to the inherent limitations of the available data which solely represents the base population of Lumaria, it was necessary to make assumptions that give insight into the diverse risk profiles associated with policyholders. By performing this analysis and recognising the impact of important risk factors, SuperLife can enhance its pricing strategy to adjust insurance products that align closely with policyholder needs whilst maintaining a competitive advantage.

Gender and smoking cohorts: For mortality modelling, policyholders are categorised into 4 cohorts to accurately capture mortality differences that arise due to the universal variables of sex and smoker status: Male Smokers, Male Non-Smokers, Female Smokers, Female Non-Smokers.

Age Bracketing: Individuals under the legal age of 18 are presumed non-smokers. During this period, the influence of sex on mortality is considered minimal, and all cohorts exhibit uniform base mortality rates from ages 0 to 17.

Mortality Loading Factors: From the ages of 18 onwards, each cohort is assigned a mortality loading factor, which when applied to the base population mortality at each age yields a new mortality rate. This factor reflects the differential impact of smoking and gender on mortality:

*Table 4: Mortality Loading Factor Assumptions*
|   Cohort                 |   Male Smokers   |   Female Smokers   |   Male Non-Smokers   |   Female Non-Smokers   |
|--------------------------|------------------|--------------------|----------------------|------------------------|
|   Gender impact          |   1.52           |   0.91             |   1.52               |   0.91                 |
|   Empirical estimation   |   4.08           |   10.12            |   0.697              |   0.74                 |
|   Loading Factor         |   6.91           |   9.16             |   1.06               |   0.67                 |

*Please see Appendix 8.2.2 Loading Factors Methodology for Calculations.*
- **Uniform smoking intensity:** All smokers in Lumaria exhibit a uniform level of smoking intensity, leading to a consistent adverse mortality impact among the smoking cohorts. This assumption allows smoking to be treated as a homogeneous risk factor, irrespective of individual smoking habits.
- **No Cohort Effects:** The mortality of individuals is not affected by factors relating to their circumstances (birth year, socio-economic status, region etc.).

### 4.2 Pricing Model Assumptions
The financial model for the Single Premium Whole Life Insurance (SPWL) and 20-Year Term Insurance products hinges on several pivotal assumptions.
- Lapse Rate: Assumed to be 0% for SPWL insurance as none of the SPWL policyholders in the in-force dataset lived through the duration of the policy. However, for the 20-year term policy, the lapse rate was computed based on each issue age and issue year. See Appendix 8.3.1 Pricing Model Assumptions for the formula utilised.
- Death Benefit Amount: The death benefit was calculated through a weighted average of the percentage of policyholders with the face value for both the 20-year term and SPWL policies. This was fixated to provide a conservative approach for the calculation of the profit.
- Expense Loading: The amount added to the premium to cover the insurer's expenses, calculated using the highest and lowest averages from the economy sheet.
- Surrender Value: For the SPWL insurance policy, we assumed there would be a surrender rate as some policyholders may want to withdraw from the insurance before the end of the policy and it was assumed to be the highest average percentage from the economy sheet. See Appendix 8.3.1 Pricing Model Assumptions for the formula utilised.
- Reserves:
> - For the SPWL policy, the reserves were based on the probabilities of survival and death directly to ensure the reserves were an accurate representation of the scenario at hand. See Appendix 8.3.1 Pricing Model Assumptions for the formula utilised.
> - In the 20-year term policy, the reserves were calculated using the APRA and BASEL III frameworks. A loss ratio was fixated using multiple resources and reports available online, see Appendix 8.3.1 Pricing Model Assumptions for a snapshot of the calculation methodology and the formula utilised. It was decided to keep the reserves fixed for a conservative approach, across the model, despite the introductions of the incentives.

*See Appendix 8.3.1 Pricing Model Assumptions for the remaining assumptions made.*

## 5. Risk and Risk Mitigation Considerations
The most significant risks to the program are displayed through a risk matrix and are summarised in the table below. These risks arise from data limitations, uncertainty faced during mortality and program analysis, and projection of future claims cost.

*Insert Matrix*
|   Risk                  |   Explanation                                                                                                                                                                                                                                                                                        |   Risk Mitigation                                                                                                                                                                                                                                                                                                                                            |
|-------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|   Assumption Risk       |   Foundational for modelling and ideally help simplify complex procedures. If they are incorrect, the model can produce inaccurate results, leading to poor decision making.                                                                                                                         |   Follow the challenge, validate, review procedure regularly. Apply appropriate modelling techniques like:    - Bayesian: update based on experience. This would assist in reducing uncertainty and improve accuracy of results.    - Ensemble: allow for the usage of multiple models and combining them. Allows us to not rely on one single assumption.   |
|   Product Design Risk   |   SuperLife is looking to introduce new elements to their already existing long term life insurance products. There is a risk that the product might not be perceived beneficial, issues in management and potential obsolescence by going backwards rather than forwards.                           |   SuperLife should look at testing the proposed changes through pilot testing and look at marketing and distribution channels to analyse market properly. Should also ensure the changes are drafted as desired in legal documents. Finally, have an implementation plan is in place to ensure product launch is well managed.                               |
|   Pricing Risk          |   Pricing risk may occur when the expected claims, lapse rates, expenses and investments are inaccurately estimated. Could result in heavy financial losses.                                                                                                                                         |   Scenario Testing to identify impacts of each variable considered in pricing. Practicing this regularly would allow for monitoring and updating based on any deviations.                                                                                                                                                                                    |
|   Underwriting Risk     |   Keeping required data to ensure that that SuperLife is only taking on risks they are capable of can be challenging and may lead to adverse selection.                                                                                                                                              |   Being a developed country, Government of Lumaria should allow SuperLife to access relevant health data through their universal healthcare system. This would allow a proper assessment for everyone.                                                                                                                                                       |
|   Liquidity Risk        |   During a Black Swan event, such as a pandemic, SuperLife faces the risk of simultaneous claims surpassing reserves and capital, potentially destabilizing the company. Moreover, sudden withdrawals or surrenders by customers may occur if they perceive the insurer as financially vulnerable.   |   SuperLife should aim to maintain strong capital positions and ensure that they are conducting stress testing and cash flow projections on an ongoing basis. Furthermore, it would also be viable to ensure close management and optimal asset allocation to mitigate liquidity risk.                                                                       |
|   Interest rate risk    |   There is always a risk of discounting our future premiums and payouts whilst pricing, as the future interest rate is not certain.                                                                                                                                                                  |   This is mitigated using historical data to project future interest rates. It would also be viable to use financial instruments like futures and forwards to hedge against the interest rate risk.                                                                                                                                                          |
|   Moral Hazard          |   Participants inappropriately filing claims and misuse of program features will inflate costs associated with the program.                                                                                                                                                                          |   Assumptions of program participation and effectiveness to be monitored during implementation stages and adjusted accordingly.                                                                                                                                                                                                                              |


## 6. Data and Data Limitations
|   Data Limitation                                                                                     |   Assumption                                                                                                                                                                                      |   Justification                                                                                                                                                                                                 |
|-------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|   Lack of complete data availability for mortality tables (35 to 65 for SPWL and 26 to 55 for T20).   |   Assumed policyholders for both policies have similar mortalities when finding loading factors from policyholder data. Usage of external data from developed countries like USA and Australia.   |   Maximise data availability for more accurate loading factors.    Developed countries like USA and Australia are similar to Lumaria’s in terms of operations and have been considered as ideal replacements.   |
|   Lumaria's pricing regulations are unspecified, with no available guidelines.                        |   It is assumed that policies can be priced based on sex and smoking status.                                                                                                                      |   Legal in countries like Australia (base location of Actualnsight), however, is a limitation since it is illegal in Europe (pricing based on gender).                                                          |
|   No information on competitors in the life insurance market.                                         |   Assumed that the program will make significant impact on existing policyholders and incentivise prospective clients to purchase products.                                                       |   Program impact and its incentives cannot be valued against competitors in the existing life insurance market. This puts SuperLife at a strategic disadvantage.                                                |
|   No data relating to company expenses or existing capital.                                           |   Assumptions related to the pricing model, including expenses, reserves.                                                                                                                         |   This data limitation reduces the accuracy of pricing modelling.                                                                                                                                               |

## 7. Final Recommendations and Conclusion
Actualnsight has found that through the implementation of our 4 incentive programs, a significant decrease in expected mortality can be achieved by encouraging healthier lifestyles. The reductions in mortality lead to lower pure premiums and allow SuperLife to cover the costs of the programs while still reducing the overall premiums for customers. This provides a competitive advantage for SuperLife and mutual benefits to them and their customers. Considerations with regards to potential risks and data limitations have also been addressed with potential methods to mitigate and deal with these issues. Additionally, Actualnsight has provided metrics for monitoring the effectiveness of these incentive programs into the future.

## 8. Appendix - Please Refer to Section 8 of the [Final Report](https://github.com/Actuarial-Control-Cycle-T1-2024/group-page-showcase-actuainsight-consulting/blob/df984685ef9cd79912909576affd3bf1c0579743/Actualnsight%20Consulting%20Report.pdf)
