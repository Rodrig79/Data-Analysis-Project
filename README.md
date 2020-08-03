<h2>CPSC-4310 Machine Learning Data Analysis Project - Assignment 2</h2><br>
Team Members:<br>
Marco Rodriguez, 
Shaun Lee 
<br>
<h1> New York Times Coronavirus (COVID-19) Data in the United States (Dataset #1) </h1><br>
Description: This dataset has the cumulative counts of coronavirus cases in the United States, at the state and county level, over time. This data is taken from state and local governments and health departments in order to provide a complete record of the outbreak in the United States.<br>
<br>
Size of dataset: <br>
Instances (Rows): 3549<br>
Attributes (Columns): 7<br>
<br>
<h3>Data Samples:</h3><br>
First five datasamples:<br>


|date   |state   |cases   |deaths   | cases_per_capita |deaths_per_capita |state_population
|:-:|:-:|:-:|:-:|:-:|:-:|:-:|
|2020-01-21|	Washington|	1|	0|	0.0| 0.0| 7614893
|2020-01-21|	Washington|	1|	0|	0.0| 0.0| 7614893
|2020-01-21|	Washington|	1|	0|	0.0| 0.0| 7614893
|2020-01-21|	Washington|	1|	0|	0.0| 0.0| 7614893
|2020-01-21|	Washington|	1|	0|	0.0| 0.0| 7614893

Last five datasamples (as of 5/7/20): <br>

|date   |state   |cases   |deaths   | cases_per_capita |deaths_per_capita |state_population
|:-:|:-:|:-:|:-:|:-:|:-:|:-:|
|2020-05-07|	Virginia	|21570	|769	|252.7	|9.0	|8535519
|2020-05-07| 	Washington|	17334|	903|	227.6|	11.9|	7614893
|2020-05-07|	West Virginia|	1297|	51|	72.4|	2.9|	1792147
|2020-05-07|	Wisconsin|	9215|	374|	158.3|	6.4|	5822434
|2020-05-07|	Wyoming|	635|	7	|109.7|	1.2|	578759




<h3>Attributes:</h3>
Date: date of confirmed cases and deaths. We changed the format from the raw data to make data visualization easier.

State: US State of confirmed cases and deaths

Cases: Cumulative cases of COVID-19 to date.

Deaths: Cumulative deaths from COVID-19 to date.

Cases Per Capita: We used an function to take the number of cases divided by the state's population, then multiplied that value by 100,000 to obtain the cases per capita for that row. Cases per capita = (Cases/State Population) * 100,000 

Deaths Per Capita: Used the same function as cases per capita Deaths per capita = (Deaths/State Population) * 100,000 

Population: Estimated state population in 2019. Used to calculate Cases and Deaths per capita.



<h1> State Action on Coronavirus (Dataset #2) </h1><br>
Description: This dataset showcases state legislative action towards containing the COVID-19 outbreak. <br>
<br>
Size of dataset:<br>
Instances (Rows): 579<br>
Attributes (Columns): 3<br>
<br>
<h3>Data Samples:</h3><br>

First five datasamples:<br>
|State|Enacted|Date_Enactment|Economy|Health|Bill_Summary
|:-:|:-:|:-:|:-:|:-:|:-:|
|Alabama	|TRUE	|2020-04-02	|FALSE	|TRUE|SJR 40  Urges individuals to fist bump rather than shake hands. Enacted.| 
|Alabama	|TRUE	|2020-03-12	|TRUE	|TRUE|SR 49  Urges Congress to fund additional rental assistance due to coronavirus. Adopted.|
|Alabama	|TRUE	|2020-05-05	|FALSE	|FALSE|SR 60  Relates to no excuse absentee voting, Legislature urged to adopt. Adopted.|
|Alabama	|FALSE	|NA	|FALSE	|TRUE|HR 107  Urges the promotion, sharing and posting of practices to reduce the spread of infectious diseases. Pending.|
|Alabama	|FALSE	|NA	|TRUE	|TRUE	|HJR 121/HJR 122  Urges the Governor to expand Medicaid coverage for new mothers in response to the current COVID-19 pandemic. Pending.|



Last five datasamples (as of 5/7/20): <br>

|State|Enacted|Date_Enactment|Economy|Health|Bill_Summary
|:-:|:-:|:-:|:-:|:-:|:-:|
|Washington	|TRUE	|2020-03-17	|TRUE	|TRUE	|SB 6189  Clarifies eligibility for School Employees' Benefits Board coverage of substitute teachers; and of school employees during quarantine or school closures due to COVID-19. Enacted.|
|Wisconsin	|FALSE	|NA	|FALSE	|FALSE	|SR 7  Acknowledges that the Communist Party of China deliberately and intentionally misled the world on the Wuhan Coronavirus; stands in solidarity with the Chinese people to condemn the actions of the Communist Party of China. Failed.|
|Wisconsin	|FALSE	|NA	|TRUE	|TRUE	|SB 927  Exempts pharmaceutical, treatment, and other medical supplies used for treating coronavirus from the Unfair Sales Act, also called the minimum markup law, during the public health emergency due to coronavirus. Failed.|
|Wisconsin	|FALSE	|NA	|TRUE	|TRUE	|AB 1035  Exempts pharmaceutical, treatment, and other medical supplies used for treating COVID-19 from the Unfair Sales Act, also called the minimum markup law, during the public health emergency declared on March 12, 2020. Failed.|
|Wisconsin	|TRUE	|2020-04-15	|TRUE	|TRUE	|AB 1038  Relates to the state government response to the coronavirus pandemic; authorizes limited autopsies for the death of an inmate due to COVID-19; establishes a civil liability exemption for persons who manufacture, distribute or sell emergency medical supplies to respond to the public health emergency. Enacted.|

<h3>Attributes:</h3>
State: US State where the bill is proposed.

Enacted: If the proposed bill was signed into law.

Date_Enactment:  Date of when the bill was passed.

Economy: If the bill is related to the economy. Can be True or False. Is determined through a function that scans the bill summary for keywords related to the economy.

Health: If the bill is related to public health. Can be True or False. Is determined through a function that scans the bill summary for keywords related to public health.

Bill Summary: A brief summary of the proposed bill.


