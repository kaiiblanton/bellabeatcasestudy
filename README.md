# Bella Beat Data Analytics Case Study

**Ask:**

*Business task:*
Analyze how people are already using their smart devices to gain insights to inform and guide Bellabeat’s marketing strategy

*Stakeholders:*
Urška Sršen & Sando Mur, the executive team and Bellabeat's marketing analytics team

*Product:*
Leaf classic wellness tracker which connects to the app to track activity, sleep, and stress


**Prepare:**

The data used is from the public data set: https://www.kaggle.com/datasets/arashnic/fitbit/code (CC0: Public Domain, dataset made available through Mobius), which contains personal fitness tracker data from 30 FitBit users. These 30 users consented to the submission of their personal data.

ROCCC  Analysis:

*Reliability:* Low because we don’t have any demographic information, and 30 is a small sample size.

*Original:* Low because I’m unable to validate the information, and it comes from a third-party source.

*Comprehensive:* The data isn’t comprehensive because it’s a small sample size, and there’s no demographic information.

*Current:* The data isn’t current because it was collected 7 years ago, and it's from a month time range.

*Cited:* The data is cited from Amazon Mechanical Turk from 7 years ago. It has not been updated.

This data set has some limitations when it comes to credibility and integrity. A larger sample size is preferential to decrease the possibility of margin of error and bias while increasing the confidence level and statistical significance. It would also be beneficial to have demographic information on the participants since Bellabeat’s target market is women. Lastly, this data is old and could be outdated.


**Process:**

I will be using two spreadsheets: the dailyActivity_merged.csv and the sleepDay_merged.csv

*dailyActivity_merged data cleaning:*

<img width="1081" alt="format number - sleep" src="https://github.com/kaiiblanton/bellabeatcasestudy/assets/150749292/1b6aeb89-cd51-4eb0-b294-223a77126eb4">

Step 1: Ensured all the data was in the right format (plain text was converted to numbers and dates)

![Screen Shot 2023-11-14 at 4 43 57 PM](https://github.com/kaiiblanton/bellabeatcasestudy/assets/150749292/d7d3a939-1d2e-45ea-8bc6-7f9e59d299ca)

Step 2: Rounded all the columns that included distance to 2 decimal places, so the data is easier to read

<img width="329" alt="conditional formatting - activity" src="https://github.com/kaiiblanton/bellabeatcasestudy/assets/150749292/4088b7f5-256b-4878-99f4-94a586fe782a">

Step 3: Looked for any duplicates using conditional formatting

<img width="203" alt="unique : count - activity" src="https://github.com/kaiiblanton/bellabeatcasestudy/assets/150749292/b1c34596-653e-46fe-998f-ba05c26087bf">

Step 4: Used the UNIQUE and COUNT functions to identify the total number of IDs

![Screen Shot 2023-11-14 at 4 43 08 PM](https://github.com/kaiiblanton/bellabeatcasestudy/assets/150749292/963a8d8a-c7b1-413f-9451-728d11be0389)

Step 5: Changed date format from MM/DD/YYYY to the day of the week


*sleepDay_merged data cleaning:*


<img width="697" alt="format - sleep" src="https://github.com/kaiiblanton/bellabeatcasestudy/assets/150749292/23075322-d152-4b1e-9b3b-4f804d267228">

Step 1: Ensured all the data was in the right format (plain text was converted to numbers and dates)

<img width="327" alt="conditional formatting - sleep" src="https://github.com/kaiiblanton/bellabeatcasestudy/assets/150749292/69427a2c-2930-4e98-ad09-e646ae457903">

Step 2: Looked for any duplicates using conditional formatting

![Screen Shot 2023-11-14 at 4 57 45 PM](https://github.com/kaiiblanton/bellabeatcasestudy/assets/150749292/b3f1874d-82e5-4ad2-9b06-4c4eba9b1d11)

Step 3: Used the UNIQUE and COUNT functions to identify the total number of IDs

![Screen Shot 2023-11-14 at 4 58 22 PM](https://github.com/kaiiblanton/bellabeatcasestudy/assets/150749292/90595e46-ed1e-4ede-9314-3d366b5e1e32)

Step 4: Changed date format from MM/DD/YYYY to the day of the week


**Analyze:**

<img width="509" alt="Screen Shot 2023-11-13 at 7 13 51 PM" src="https://github.com/kaiiblanton/bellabeatcasestudy/assets/150749292/0421eef4-4910-44c1-b9a4-932dec336c8e">

Image 1 shows the relationship between average time asleep and day of the week. From the chart, we can see that users get the most sleep on Sundays and the least on Thursdays. Users spend on average between 402 minutes to 452 minutes sleeping, which is between 6.7 hours and 7.5 hours. Note: There was also only data for 24 users instead of 30.

<img width="499" alt="Screen Shot 2023-11-13 at 7 02 24 PM" src="https://github.com/kaiiblanton/bellabeatcasestudy/assets/150749292/01d5de04-1e22-4d60-974d-37be2fd03c4f">

Image 2 shows the relationship between average time in bed and day of the week. From the chart, we can see that users spend the most time in bed on Sundays and the least on Thursdays. Users spend on average between 435 minutes to 503 minutes in bed, which is between 7.25 to 8.3 hours. This observation is consistent with users sleeping the most on Sundays and the least on Thursdays. There was also only data for 24 users instead of 30.

<img width="498" alt="Screen Shot 2023-11-13 at 7 02 00 PM" src="https://github.com/kaiiblanton/bellabeatcasestudy/assets/150749292/42d941d2-366a-4961-8d52-cf873396c2f9">

Image 3 shows the relationship between average daily steps and the day of the week. From the chart, we can see that users get the most steps on Saturday with Tuesday being a close runner up, and users getting the least steps on Sunday. Note: There was data from 33 users instead of 30.

<img width="504" alt="Screen Shot 2023-11-13 at 7 01 34 PM" src="https://github.com/kaiiblanton/bellabeatcasestudy/assets/150749292/8aeee94c-4201-4d95-b2f2-3ac3edfd5fd9">
<img width="158" alt="Screen Shot 2023-11-13 at 7 01 46 PM" src="https://github.com/kaiiblanton/bellabeatcasestudy/assets/150749292/2f8fc8a3-84fc-4144-873b-1c07c745fb3d">

Image 4 shows the relationship between the average active minutes (sedentary, lightly active, fairly active, and very active minutes) and the day of the week. From the chart, we can see that users spend most of their time being sedentary daily. Also, users are most active on Mondays and least active on Thursdays. Note: There was data from 33 users instead of 30.

<img width="506" alt="Screen Shot 2023-11-13 at 7 00 40 PM" src="https://github.com/kaiiblanton/bellabeatcasestudy/assets/150749292/d66fab35-9c4f-4e78-97a3-4bb458e7af57">

Image 5 shows the relationship between average calories burned and day of the week. From the chart, we can see that users burn the most calories on Tuesday with Saturday being a close runner up and the least on Thursday. Note: There was data from 33 users instead of 30.

<img width="488" alt="Screen Shot 2023-11-13 at 7 02 09 PM" src="https://github.com/kaiiblanton/bellabeatcasestudy/assets/150749292/5c64cd36-729d-4fea-9da5-591a0a055dd5">

Image 6 shows the relationship between average total daily distance and day of the week. From the chart, we can see that users have the highest total distance on Saturday with Tuesday being a close runner up, and the least distance on Sunday.

**Share:**

Dashboards created in Tableau to support the above analysis

![Screen Shot 2023-11-13 at 6 58 13 PM](https://github.com/kaiiblanton/bellabeatcasestudy/assets/150749292/c7baefc0-6818-4583-bc32-91a4f578cf8e)

![Screen Shot 2023-11-13 at 6 58 32 PM](https://github.com/kaiiblanton/bellabeatcasestudy/assets/150749292/8bda2104-c9e6-4dea-978f-8e73768696db)


**Act:**

Recommendations:

1. Bellabeat knows that users are already using their smart devices to track their sleep. The National Health Organization advises adults to get between 7-9 hours of sleep. Bellabeat could run a marketing campaign about the importance of sleep and how using the Leaf will help users track their sleeping patterns. If possible, users could set a sleep schedule in the app, and the Leaf could notify them when it's time to go to sleep, which would encourage users to get the recommended 7-9 hours of sleep.
2. There's no way to directly track stress levels using the Leaf device. However, Bellabeat could run a marketing campaign about the negative health effects of stress and how exercise could help lower stress levels. Bellabeat could also talk about how using the Leaf will help users manage their stress by encouraging users to get more exercise, get an adequate amount of sleep, and practice daily mindfulness.
3. Bellabeat knows that users are already using their smart device to track their activity. From the data we can see that most users are sedentary throughout the day. Bellabeat could run a marketing campaign about the negative long term effects of living a sedentary lifestyle. They could also talk about how using the Leaf will help users live a more active lifestyle by encouraging more daily movement.
4. Bellabeat could also run in app challenges to encourage users to move more throughout the day. Bellabeat could add a function that allows users to invite their friends to join their challenge and track each other's progress.
