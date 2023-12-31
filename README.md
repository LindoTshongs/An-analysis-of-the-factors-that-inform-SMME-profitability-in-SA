# An-analysis-of-the-factors-that-inform-SMME-profitability-in-SA

South Africa faces the persistent issue of unemployment, with around 34.5% of South Africans of working age and who are eligible to work being unemployed. This number is even worse when we consider youth unemployment which stands at around 63.9% for youth between the ages of 15-24 and around 42.1% for those between the ages of 24-35. This poses serious challenges for the government and the nation at large as such high numbers undermine social cohesion. SMMEs have the potential to solve this problem and the government has identified them in its policies as a potential solution to dealing with the issue of unemployment and thus bring about social cohesion and order. However, SMMEs have alarmingly high failure rates, with about 75% of all SMMEs failing within the first two years of being established. These high numbers challenge the government and its policymakers to ensure that its policy initiatives bear fruits. Thus, a comprehensive study and an understanding of the factors that contribute to SMME success is very important, as such insights can help ensure these high failure rates are curbed. This study looks into the factors that contribute to the success of SMMEs using business profitability as the proxy for success.

Technical steps:
* This analysis first selected the appropriate variables, cleaned them and constructed some newer ones to aide in our analysis.
* Studentised residuals and Cooks distances where used to identify outliers, quantify their impact and inform their removal.
* To deal with the multicollinearity, we used the Inflation Variance Factory( VIF).
* Then, log transformations were used to fix the issue of non-linearity and lessen the severity of heteroscedasticity.
* Missing values were replaced with using the Predicitve Mean Matching algorithm contained in the Mice package.
* Tested for misspecification using the resset test, and then attempted to solve it by using random forest trees and the randomForestExplainer package to find the most important interactions.

The logged regression model was used as the benchmark model. And then the lasso regression model was further used as the final model, which is robust to overfitting by applying a penalty term.
Note, both models were cross validated to further solve the issue of overfitting and high variance on unseen data.

The results from our study suggest that several themes are important in determining SMME profitability in the South African context, 
  1. Selling to government and to larger businesses is a robust predictor of profitability.
  2. Having your business located in the formal urban area is very important for profitability.
  3. Furthermore, also related to location, having your business operating in premises dedicated to business is also very important, and if possible avoiding residential premises.
  4. Having strong managerial competence, highlighted by having a manager who at the least is literate, and who have taken important decisions on behalf of the business such as having insurance, accounting and budgeting, having measures against crime etc is also an important combination in having successful enterprises.
  5. Lastly, but not least, this study showed that being a micro-enterprise at the least, which has at least one employee is an important determiner of profitability, as micro-enterprises tend to be motivated by identifying local opportunities and profiteering objectives, in contrast to the Own-account businesses which only have the owner in charge and motivated by survival imperatives.

It should be noted though that is a relatively old dataset and thus some of the variables are outdated and reflect the state of the world relevant to when the data was collected. Thus, new data might have come to the fore with newer set of variables which are more robust and reflective of the contemporary period. Thus, this study should be repeated with much more newer datasets which reflect the status quo, i,e the advent of smart phones, social media, financial technology advancements and many more which are relevant to businesses that operate in the 2020s.
