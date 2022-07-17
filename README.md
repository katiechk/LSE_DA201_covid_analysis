# LSE_DA_COVID_analysis


### Week 2 Notes and observations:

The total numbers provide a glimpse of the COVID-19 data to indicate the overview of the data recorded. Yet, it is unable to provide much insight because of the following reasons:
1. Part of the data recorded are cumulative data that the sum does not provide an actual picture of the data
2. There are missing data in the provided dataset that the total number is not the full representation of the period recorded
3. There is no clear indication for the stability of the data that if the data is collected consistently over time.

With the concern listed above, it is important to review the data trends over time to offer additional insights. Based on the identified trend, we can recognize the unjustified part of the data that required further investigation. We can also discover the 2 spike for COVID-19 that is Dec 2020 and Jul 2021. We can distinguish a positive relevance between the Deaths, Cases, Hospitalised and Recovered.

The typical mistakes that are easily made in this phase is to review the data at a high level only and neglect the data detail.

#### Explore the cases dataframe:
- The cases dataframe is the daily entries that contain details of COVID cases in the United Kingdom, including the number of deaths, cases, recovered, and hospitalised cases in each of the provinces.
- Deaths and Cases are cumulative data as we can see the number increase over time. Hence, descriptive statistic does not provide much insight in this case
- The hospitalised data is the number of cases where COVID-19 positive individuals are hospitalised, yet it is worth to further explore and clarify given that the number of hospitalised could be higher than the number of cases that is absurd
- The cases dataframe have 7,584 rows and 12 columns with 2 rows of missing data
- The number of COVID-19 cases differs significantly from province to province due to the difference in population. Others are especially high as we expect it to cover the large number of population in the UK.

#### Explore the vaccinated dataframe:
- The vaccinated dataframe is the daily entries of vaccination in UK and it is not cumulative data
- The vaccinated dataframe have 7,584 rows and 11 columns with 0 rows of missing data
- Although the number of COVID-19 cases in Others differs significantly as it covers the large number of population in the UK, the vaccination number is similar with other province
- Vaccinated number is the same as Second Dose which indicate people who received Second Dose are considered to be fully vaccinated
- The desriptive statistic of vaccinated dataframe does not provide much insight either because the data entries before the vaccination launched were all recorded as 0

#### Explore the tweets dataframe:
- The tweets dataframe is an extract of Twitter data from 15 May 2022 to 23 May 2022 relating to the #coronavirus hashtag
- The tweets dataframe have 3,960 rows and 21 columns with missing value from few columns across all data

#### View the Covid cases and Vaccination in Gibraltar:
- Descriptive statistic of cases_gibraltar dataframe does not provide much insight given part of the data are cumulative data
- Gibraltar reached the maximum number of death on 27 Aug, 2021
- Gibraltar reached the maximum number of recovered and hospitalised on 4 Aug, 2021 and 18 Jan, 2021 respectively. The number dropped back that indicated a potential data record issue if the data was recorded as a cumulative data
- Based on the lineplot of Gibraltar COVID-19 data over time, we can identify that the hospitalised data should be reviewed before further analysis because the data recorded before Aug 2020 are impractical that the hospitalised cases are higher than recorded positive cases.
- The recovered data should also be reviewed because of the sudden drop to 0 in one day on August 5, 2021.



### Week 3 Notes and Observations:

The data for Others province/state is heavily skewed that affect the overview of the dataset. Given that there is no clear indication of what the Others represented and we cannot see much insight provided from this data, we have dropped the Others data to better review the entire dataset.

The overview of the cases_vaccinated shows a similar trend as the cases_gibraltar for the number of cases, deaths, hospitalised and recovered. The hospitalised data is oddly recorded that is not correspond with the number of positive cases. Recovered cases since 5 Aug, 2021 onwards are missing from the dataset. The detailed breakdown by province/state should be examined to further investigate if the data are well collected in each province/ state.

Gibraltar has the highest number of fully vaccinated population across all province/ state. Yet if we reviewed the vaccination % by province, we can see that the fully vaccination % are similar across all province/ state at approx. 95.5%.

To evaluate the vacciation pattern by days, people tend to received vaccination on Thursday to Saturday and less likely to receive vaccination on Sunday and Monday. This may be attributed to the recommended recovery period following vaccination. We can also see the number of total vaccination decreased from July 2021 with majority of the population already vaccinated.

The analysis of the data is limited by the incompetency and inaccuracy of the data. All data should be reviewed to ensure the accuracy. Population by province/state should also be included to better evaluate the data.



### Week 4 Notes and observations:

- Others is taken out to avoid skewing the dataset and better observe the patterns
- The hospitalisations are synchronised across province/states
- The recovered cases increased starting from 2021, we can see the sharp increase specially for Gibraltar and Channel Island from Jan 2021 to Apr 2021
- Bermuda is having a significant increase in the number of death since Oct 2021, further investigation is recommended to understand the root cause
- There is no strong relation identified between the vaccination and number of deaths/ recovered based on the visualised trends
- The trend between cases, hospitalised and recovered are similar to a certain extent with 2 spike in total
- Further research can be conducted for province/state shared similar pattern to explore the other external factors in affecting the data (e.g. weather, location, population density...)
- If more vaccination detail can be provided (e.g. the difference in time between first dose and second dose), we can further explore to see how to maximise the effectiveness of vaccination to reduce the number of casese and deaths.



### Week 5 Notes and Observations:

- The Tweets data are collected in May 2022
- The top hashtags and words in the Tweets data are netural words that reflects how the general public are used to COVID-19 with less negative emotions. Yet, the data size is too small that more data should be scraped from Twitter for a better review
- Vaccine doesn't appear to be a topic that is widely discussed on Twitter
- People are having high interest towards 'Athen', 'China' and 'Greece' that worth to further explore
- The data from Twitter provide a wider picture to review the COVID-19 situation in the word of public. However, it is vital to vet and critically analyse the data carefully to avoid misusing the data.



### Week 6 Notes & Observations:

Answer 1: Quantitative data are information about numeric variables. In contrast, qualitative data are data that cannot be counted, measured or readily expressed using figures. It is the descriptive and conceptual findings usually collected through questionnaires, interviews, or observation.

Both quantitative and qualitative data are used in business predictions. Quantitative forecasting make use of the exact numbers and predict based on the identified patterns. Whereas qualitative forecasting make the prediction based on emotions, ideas and judgements instead of numbers. Qualitative prediction allows more interpretation comparing with quantitative prediction and can communicate concept that numbers don't capture. However, it is easy to include personal bias when it comes to qualitative predictions.

In our example, Twitter data will be considered to be qualitative data while the COVID-19 cases data will be considered to be quantitative data.

Answer 2: Continuous improvement is vital because we can review and make necessary change to adapt and optimise the effectiveness and outcome based on the change in situation. Most of the projects and works would experienced a learning period and testing is essential to achieve the best result. Hence, continuous improvement is needed to ensure we are doing things in the most efficient and effective way.

Answer 3: Data ethics are the guideline that should be followed by every business to ensure that privacy, security, and transparency standards are met because it establish a baseline of trust between the business and users. In our case, only share the data to restricted party is the data ethics and ensure users know how their data is being used are two of the most important data ethics that should be applied.
