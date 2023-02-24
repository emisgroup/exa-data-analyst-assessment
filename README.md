# Data Analyst - Technical Assesment
Our tech teams are curious, driven, intelligent, pragmatic, collaborative and open-minded and you should be too. 

## Testing Goals
We are testing your ability to design and scalable usable and readable SQL code, this will be underpinned by using best practices are being aboout to take requirements and create outcomes with value.

You will have approximately 1 week to complete this task but can as much or as little time as you deem necessary to **demonstrate your understanding of the problem, your range of skills and approach to problem solving**.

Some successful candidates have spent as little as 3 hours whilst others have used the full week because they've enjoyed exploring different ideas, technologies and approaches. 

## The Tasks

Part 1:Using the patient data provided identify how many patients there are for each given postcode area to check which area would be best to use for the population you are looking for.Patient counts should be reviewed by gender to make sure there's enough distribution across genders.

Part 2:
Using the information you have from part 1 identify the 2 most suitable postcode areas (i.e. largest patient count) and derive a list of patients that fit the following criteria so that you can invite them to take part in a local research study.

Patients should have:
* Current diagnosis of asthma, i.e. have current observation in their medical record with relevant clinical codes from asthma refset (refsetid 999012891000230104), and not resolved
* Have been prescribed medication from the list below, or any medication containing these ingredients (i.e. child clinical codes), in the last 30 years:
 * Formoterol Fumarate (codeid 591221000033116, SNOMED concept id 129490002)
 * Salmeterol Xinafoate (codeid 717321000033118, SNOMED concept id 108606009)
 * Vilanterol (codeid 1215621000033114, SNOMED concept id 702408004)
 * Indacaterol (codeid 972021000033115, SNOMED concept id 702801003)
 * Olodaterol (codeid 1223821000033118, SNOMED concept id 704459002)

AND should be excluded if:
 * Currently a smoker i.e.  have current observation with relevant clinical codes from smoker refset (refsetid 999004211000230104)
 * Currently weight less than 40kg (SNOMED concept id 27113001)
 * Currently have a COPD diagnosis i.e. have current observation in their medical record with relevant clinical codes from COPD refset (refsetid 999011571000230107), and not resolved.

Only patients that have not opted out of taking part in research or sharing their medical record should be invited to participate (type 1 opt out, connected care opt out)

You will need to use a combination of the patient, observation, medication and clinical code information for a complete picture of a medical record. You should aim for your code to return a list of eligible patients with information on their organisation, registration id, patient id, full name, postcode, age, and gender.

## The Solution
You can use any data storge engine you feel fits however solutions should be saved as .SQL files

## Evaluation
We take into account the following critria when evaluating a solution. Each criteria is evaluated from 0 (non-existent) to 5 (excellent) and your final score would be a simple average across all 5 areas. These are:

- **Functionality**: Is the solution correct? Does it run in a decent amount of time? How well thought and architected is the solution?
- **Good Practices**: Does the code follow standard practices for the language and framework used? Take into account reusability, names, function length, structure, etc.
- **Testing**: How did you test the SQL does what it is ment to. 
- **Documentation**: Is the code readable, are there comments, does the query needs explaining.


## Submit your solution	
Create a public Github repository and push your solution including any documentation you feel necessary. Commit often - we would rather see a history of trial and error than a single monolithic push. When you're finished, please send us the URL to the repository. 
