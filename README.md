# investigating-data-set

## Dataset Description 

> In this project, a dataset containing information from 100 thousand medical appointments in Brazil focused on the question of whether or not patients show up for their appointment is the be analyzed. The columns in the dataset are;
1. ScheduledDay which tells us on what day the patient set up their appointment. 
2. Neighborhood which indicates the location of the hospital. 
3. Scholarship which indicates whether or not the patient is enrolled in Brasilian welfare program Bolsa Família.
4. PatientId gives information about the Patient while AppointmentID assigns unique code to each appointment.
5. The Age column specifies the age of the patient while the Sex column states the sex of the patient. Here M stands for Male and F for Female
6. The dataset also contains the columns Hypertesion, Diabeties, Alcoholism and Handicap which states if the patient is Hypertesive, Diabetic, an alcoholic or Handicap. A 0 on this columns shows that the patient is not.
7. The Sms_received column states whether the patient received sms or not. 
8. And lastly the No-show column which says whether the patient showed up for the appointment or not it says ‘No’ if the patient showed up to their appointment, and ‘Yes’ if they did not show up.


## Questions for Analysis: 
> I would like to investigate the following question:
> 1. Is the SMS effective?
> 2. Does Age determine if a patient shows up or not
> 3. Does Neighbourhood have any impact on a patient showing up or not?

## Data Wrangling

 In this section of the report, We will check for cleanliness and tidiness of the dataset, and then trim and clean our dataset for analysis.


### General Properties
> The dataset consists of 110527 appointments scheduled over 103549 day. The number of days for the appointment is 27 in 81 different health centers/hospitals. It involves 104 different ages, both male and female. 

> There are two values each for scholaship, hypertension, diabetes, alcoholism, sms_received and no-show, which can be interpreted as YES and NO or TRUE and FALSE. Handicap has five unique values which could represent different types of disabilities.

### Data Cleaning

In this section, I will get rid of thing that are not required for the analysis and re-arrange where neccessary. 
> 1. Drop rows with age -1
> 2. Rename the Handcap and Hipertension columns as Handicap and Hypertension respectively
> 3. Categorise **Handicap** into into *Disable* and *Non-Disable*
> 4. Replace '-' with '_' and uppercase with lowercase labels in column names

## Exploratory Data Analysis
 In this section, We shall be using some visuals to view the dataset and make few point of it:
 > 1. The larger percentage of patients are below 70 years of age and only about 35 percent received sms
 > 2. The percentage of those who received sms and did not show up is very small compared to those who did not receive
 > 3. Older folks tends to miss appointments than younger ones. Also teenagers, patients in early 20's and early 40's seems to top the chat
 > 4. Most patients at Ilhas Oceanicas de Trindade did not show up
