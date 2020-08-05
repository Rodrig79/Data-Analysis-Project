<h2>CPSC-4310 Machine Learning Data Analysis Project</h2><br>
Team Members:<br>
Marco Rodriguez, 
Shaun Lee 
<br>
<h1> Pokemon Dataset </h1><br>
Description: This dataset has all Pokemon up to Generation 6. The dataset includes each Pokemon along with their stats used to calculate damage taken and given in battle. <br>
<br>
Size of dataset: <br>
Instances (Rows): 801<br>
Attributes (Columns): 10<br>
<br>
<h3>Data Samples:</h3><br>
First five datasamples:<br>


|Type 1   |Type 2   |Total   |HP   | Attack |Defense |Sp. Atk |Sp. Def |Speed |Legendary 
|:-:|:-:|:-:|:-:|:-:|:-:|:-:|:-:|:-:|:-:|
|Grass | Poison| 318| 45| 49|49|65|65|45|FALSE
|Grass | Poison| 405| 60| 62|63|80|80|60|FALSE
|Grass | Poison| 525| 80| 82|83|100|100|80|FALSE
|Grass | Poison| 625| 80| 100|123|122|120|80|FALSE
|Fire | None| 309| 39| 52|43|60|50|65|FALSE


Last five datasamples: <br>

|Type 1   |Type 2   |Total   |HP   | Attack |Defense |Sp. Atk |Sp. Def |Speed |Legendary 
|:-:|:-:|:-:|:-:|:-:|:-:|:-:|:-:|:-:|:-:|
|Rock | Fairy| 600| 50| 100|150|100|150|50|TRUE
|Rock	|Fairy|	700|	50|	160|	110|	160|	110|	110|	TRUE
|Psychic	|Ghost	|600	|80	|110	|60	|150	|130	|70	|TRUE
|Psychic	|Dark	|680	|80	|160	|60	|170	|130	|80	|TRUE
|Fire	|Water	|600	|80	|110	|120	|130	|90	|70	|TRUE




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


