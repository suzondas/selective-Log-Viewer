# Selective-Log-Viewer
This feature adds facility in Koha for viewing the Patrons Log in selective manner. Primarially it is developed for showing Catalog Add (biblio, item) option with date specification or without date range. This helps to find out the log information using name of the patron. This also helps to count the total book entry done by patrons(s) and also to count wages.


## Where the featuer is added?

> In the Log Viewer Page. (Tools > Log Viewer)

## Parts of this feature

> Three parts.
1. SQL Report Creation and remembering the report number.
2. Adding CSS codes in intranetusercss. (Koha Administration > Global System Preferences > Staff Clients > intranetusercss)
3. Adding JQuery codes in intranetuserjs. (Koha Administration > Global System Preferences > Staff Clients > intranetuserjs)


## How to use it

....Installation....

>> 1. First of all you have to create a sql report with the codes provided in SQL Report file. 
To create sql report, go to Reports > Guided Reports > Create from sql. Now enter the report name for new report (anything you want), then paste the SQL code in SQL textbox. Now Save report. After that, the report will be added in Koha. You have to remember the Report ID number of this newly added report. 

>> 2. Adding CSS Codes.
To add the CSS codes you have to go to Koha Administration > Global System Preferences > Staff Clients > intranetusercss. Clicking Intranetusercss will open a box. Paste the CSS codes here.

>> 3. Adding JQuery Codes.
>> To add the jQuery codes you have to go to Koha Administration > Global System Preferences > Staff Clients > intranetuserjs. Clicking Intranetuserjs will open a box. Paste the JQuery codes here.

Then click "Save all staff Client preferences". 


....Application....

1. Load Log Viewer Page. (Tools > Log Viewer). You will see "Selective Logs (Plugin)" button right to the Browse system logs. Click the button. 

2. A prompt window will be poped up. Enter the Report ID number of the saved report here and click OK. Now the system will load the data. Wait till it finishes all task.

3. After successful loading "Selective Logs" section will be added to the page.
 
4. Under the "Patrons Name", all the patrons added biblio or item will be shown with check box. You can select any of them or all. Selecting Patrons Name is mandatory to run the system.

5. Right to the "Patrons Name" you will see "Date Range". You can  enter the date range or you can select no date range. Date range format is Year-Month-Day (e.g. 2015-01-01). Selecting any of them is mandatory to run the system.

6. Right to the "Date Range" you will see the "Add information". Add information will be retrieved based on your slection. Selecting any or both is mandatory to run the system.

7. Right to the "Add Information" you will find "Salary per add". You can enter the Salary quantity per add (biblio/item). It is optional.

8. After specifying the information click the "Search" button to retrieve the information.

..........Best regards.......
