## Call for Code

https://developer.ibm.com/callforcode/
https://callforcode.org/global-challenge/

## Register to IBM Cloud

https://ibm.biz/BdfMqA

## Tutorial link

https://developer.ibm.com/tutorials/crisis-communication-chatbot-watson-assistant-webhook-integration-discovery-covid-data/

## Add Intents & Entities
*Example 1:*
```
Intent 1: #IsThereVaccineCOVID
examples:
Did anyone found vaccines yet?
Do we have vaccines?
Is there a vaccine for COVID-19?
What type of vaccines are there?
What vaccines we have for COVID?

Dialog 1: 
If recognizes - #IsThereVaccineCOVID
Response - Yes there are now several vaccines that are in use. The first mass vaccination programme started in early December 2020 and the number of vaccination doses administered is updated on a daily basis. At least 13 different vaccines (across 4 platforms) have been administered.
```

*Example 2:*
```
Intent 2: #BenefitsofGettingVaccinated
examples:
What are the benefits of getting vaccinated?
What are the profit of vaccines?
What are the pros of vaccines?
What I get if I get vaccinated?
Why should I get vaccinated?

Dialog 2: 
If recognizes - #IsThereVaccineCOVID
Response - The COVID-19 vaccines produce protection against the disease, as a result of developing an immune response to the SARS-Cov-2 virus.  Developing immunity through vaccination means there is a reduced risk of developing the  illness and its consequences. This immunity helps you fight the virus if exposed. Getting vaccinated may also protect people around you, because if you are protected from getting infected and from disease, you are less likely to infect someone else. This is particularly important to protect people at increased risk for severe illness from COVID-19, such as healthcare providers, older or elderly adults, and people with other medical conditions.
```

*Example 3:*
```
Intent 3: #ScheduleVaccine
examples:
Can I get vaccinated?
Can I schedule vaccine?
Please schedule vaccine
When can I get vaccinated?
Where can I get vaccinated?

Entity: System Entities - @sys-date @sys-time

Dialog 3: 
If recognizes - #ScheduleVaccine
Customize - add slots
Check for:
sys-date - Can you tell me what date you prefer to get vaccinated?
sys-time - Can you tell me what time you prefer?
Respones - Great ! you scheduled your vaccine appointment successfully at $date on $time
```








