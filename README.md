# BD-temperature-prediction
As a result of global warming, there is a significant change in our climate. There are several reasons for global warming and as a result of global warming there are changes in different aspects of nature. In this finding, we considered CO2 emission as a potential reason for global warming, we considered solar radiation and rainfall as potential reasons for climate change and we considered temperature as a candidate of climate change indicator. In this case, the scope can be very large. So, we considered the temperature in Dhaka - which we wanted to predict. For  predicting the temperature (target variable) of Bangladesh from feature variables - Bangladesh CO2 emission, global CO2 emission, solar radiation and rainfall data of Bangladesh.

<h2> Data Source </h2>
For this prediction, we did not collect data by ourselves. Therefore, we relied on secondary data sources. But all secondary sources are not reliable. So we relied on websites of the Bangladesh Government and International data source which is trusted and used by : Harvard, Stanford university; The Guardian, The New York Times, CNN, BBC and other news media.

Temperature and solar radiation dataset:
http://barcapps.gov.bd/climate/

CO2 emission dataset:
https://ourworldindata.org/co2-and-other-greenhouse-gas-emissions

Rainfall Data:
https://oasishub.co/dataset/bangladesh-historical-daily-rainfall-record-1948-2014-bangladesh-meteorological-department

<h2> Outcomes of Data Analysis <h2>

![Capture](https://user-images.githubusercontent.com/46414380/215963672-ab46f977-60c5-456e-8620-e2c6aad79bbe.PNG)

![Capture1](https://user-images.githubusercontent.com/46414380/215963694-60854cd1-b9e4-473e-8339-d31533e865fa.PNG)

![Capture2](https://user-images.githubusercontent.com/46414380/215963710-82dc669c-515d-4b38-a95e-ecb4c557611c.PNG)

![Capture3](https://user-images.githubusercontent.com/46414380/215963719-53534d23-1197-440b-8818-737c077fbd8b.PNG)

![Capture4](https://user-images.githubusercontent.com/46414380/215963728-0b388fc1-75b9-48ff-bf67-440fee3b2cd5.PNG)

![Capture5](https://user-images.githubusercontent.com/46414380/215963763-d5841f3d-8930-42f7-a206-2169228647da.PNG)

![Capture6](https://user-images.githubusercontent.com/46414380/215963780-1c85bf27-5d02-4d4d-9511-877d9f6e750f.PNG)


<h2> Results and Discussion: <h2>
We have finally worked on 3 yearly features : GlobalCO2emission, Solar radiation of
Bangladesh, Rainfall in Bangladesh. Prior to any transformation, our R2 the value was 0.607. We have computed various transformations on these features. Among them, log transformation on the feature “GlobalCO2emission” has increased the R2 value from 0.607 to 0.619. Log transformation, square-root transformation, cube-root transformation, exponential transformation and inverse transformation on the other features did not increase the value, rather decrease it.


![Capture7](https://user-images.githubusercontent.com/46414380/215965100-9ff75c74-746d-4311-bf58-4fc31e35cada.PNG)

<h2> Final Equation<h2>


y(TEMPERATURE) = 𝛃0 + 𝛃1*log(CO2_global) + 𝛃2(Solar_Radiation_BD) + 𝛃3(Rainfall_BD)


<h2>Conclusion and Future Work<h2>	

From this finding, we found that there is a relationship between CO2 emission of the world, rainfall and solar radiation with temperature. After performing linear regression, evaluating the p-value based on residuals less than 0.05 (significance level) rejects the null hypothesis which indicates impasse on the assumptions. We found the best possible R2 value to be 0.619, which is not very high but not too low. The value of R2 could be increased if we considered some other related features which are important factors of temperature change. Future work could also be - collecting more data of the considered features. For example, if we could collect monthly or even daily data of the following features, our results could have improved.

