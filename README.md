## No-Show Appointment
This dataset collects information from 100k medical appointments in Brazil and is focused on the question of whether or not patients show up for their appointment. A number of characteristics about the patient are included in each row.

● ‘ScheduledDay’ 
tells us onwhat day the patient set up theirappointment.

● ‘Neighborhood’ 
indicates the location of the hospital.

● ‘Scholarship’ 
indicates whether or not the patient is enrolled in Brasilian welfare program Bolsa Família.

● Be careful about the encoding of the last column: 
it says ‘No’ if the patient showed up to their appointment, and ‘Yes’ if they did not show up.

As I was investigating the data I set some factors to guide me,this factors included;

-What is the comparison between the two instances of not showing up for an appointment and showing up for an appointment.Here to get a clear view i will plot a bar graph   against the number of appointments.

-Is there a correlation between the disease categories(Hipertension,Alcoholism,Diabetes,Handcap) and Age

### Necessary packages for the project
`import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns
% matplotlib inline`

### Data Cleaning Issues 

 Grouping the data by patients ID since from the data it appears some patients had severals visitations and assigning the grouped data to a new variable new_df.
 Checked for outliers and dropped the outliers before exploring the dataset.
 
### Conclusion From Findings

From the Graph *Appointment Show Up* there are more than the yes show appointments meaning most appoitments end up being met by the patients.

Proceded to get the correlation among the different diseases and age which apppeared to be positive then went ahead and represented the diffrent correlations on a heat map.

### Data source 
 
 (https://d17h27t6h515a5.cloudfront.net/topher/2017/October/59dd2e9a_noshowappointments-kagglev2-may-2016/noshowappointments-kagglev2-may-2016.csv)

