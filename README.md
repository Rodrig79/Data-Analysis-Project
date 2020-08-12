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


<h3>Attributes with their Central Tendencies and Dispersion:</h3>
Type 1: The first type of the Pokemon. Types are used to determine which Pokemon have an advantage over other types. For example, Water type Pokemone do increased damage to Fire type pokemon.

Type 2: The second type of the Pokemon. Not all Pokemon have a secondary type.

Total: The sum of all of the other stats. HP + ATK + DEF + Sp.ATK + SP. Def + Speed = Total<br>
(Mean: 869 Mode: 600 Min: 180 Max:780)
Standard Deviation: 119.89

HP: The Pokemon's base Hitpoints. This is what the Pokemon's initial HP will be, it can increase as it levels up.<br>
(Mean:62.26 Mode:60 Min:1 Max:255)
Standard Deviation: 25.52

Attack: The Pokemon's base Attack stat.<br>
(Mean:79, Mode:100, Min:5, Max:190)<br>
Standard Deviation: 32.4

Defense: The Pokemon's base Defense stat.<br>
(Mean:73.8425 Mode:70 Min:5 Max:230)<br>
Standard Deviation:31.16

Sp.Atk: The Pokemon's base Sp. Attack stat.<br>
(Mean:72.82 Mode:60 Min:10 Max:194)<br>
Standard Deviation:32.7

Sp.Def: The Pokemon's base Sp. Defense stat.<br>
(Mean:71.9 Mode:80 Min: 20 Max:230)<br>
Standard Deviation:27.81

Speed: The Pokemon's base Speed stat.<br>
(Mean:68.2 Mode:50 Min:5 Max:180)<br>
Standard Deviation: 29.04

Legendary: True or False, whether the Pokemon is legendary or not.

