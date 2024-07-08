# Hospital_2018-2021_-Dashboard
It's a project about Data Visualization for user for the hospital past few years for data about inpatients and outpatients for year 2018-2021.

### Steps to be followed before creating the visual dashboard:-
1. Click `Get Data` and improt the folder inpatient and outpatient seperatly and during importing process choose the `combine and load data` instade of `combine and transform` option.
2. Then go to the tranform field and then go the the `Home` tab and `Append` option.
3. After appened process choose the new append file just in case if you needed the previous data form the inpatient and outpatient data files.

Data Analysis Using Power BI
============================

### Formulas used for measure clms:-

1 .Formula to create the Latest month total bills.

  `Latest Month Wait List = CALCULATE(SUM(All_Data[Total]),All_Data[Archive_Date] = MAX(All_Data[Archive_Date]))`
  
2 .Formula to create the PY Latest month total bills.

  `PY Latest Month Wait List = CALCULATE(SUM(All_Data[Total]),All_Data[Archive_Date] = EDATE(MAX(All_Data[Archive_Date]),-12))`

3 .Formula to create the Average of the total bills.

  `Average = AVERAGE(All_Data[Total])`

4 .Formula to create the Medain of the total bills.

  `Median = MEDIAN(All_Data[Total])`

5 .Formula to create the Switch for Average and median button.

  `Avg/Med Wait List = SWITCH(VALUES('Calculation Method'[Cal Methods]),"Average",[Average],"Median",[Median])`



HERE ARE SOME REVIEW PHOTOS FOR THE DASHBOARD:
1. Summary Page for Hospital Deatils<br><br>

![image](https://github.com/mohitrajendramahajan/Sales_insight/assets/103811474/03cb13b7-ceac-49bb-8d4f-6f2198ef6458)

2. Detailed Page for hospital bills according to the doctor's specialty.<br>

![image](https://github.com/mohitrajendramahajan/Sales_insight/assets/103811474/e2e475fe-9bd0-4092-8537-60927b91cff1)

For any other doubts related you may visit my Power BI workspace:
============================
**(https://app.powerbi.com/groups/me/reports/cdafbf25-b6b1-452d-b006-32cc73962a29/70d05e9150106b363010?experience=power-bi)**

If anyone facing difficulty in login the power Bi page just beacuse you are supposed to use your workspace mail-id instade of outlook ,gmail ,yahoo etc and student may also use their student mail-id provide by their respective universities.
