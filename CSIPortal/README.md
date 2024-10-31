 
 
# CSI (Customer Statisfaction Index) Portal
## Overview
The user has several Roles like Project Manager and Delivery Manager having full control of application to add, update, delete User, Client and Project. Other users can generate survey and submit it according to their evaluation.

## My Contributions
- **Implemented PDF conversion from Survey HTML Page using html2pdf while survey is submitted.**
- **Used same generated PDF of submitted survey while user is trying to download already submitted survey.** 
- **Handled part of Windows service which is responsible for sending PDF through Email to desired recepient.**

## Technologies Used
- **Frontend**: Angular
- **Backend**: .NET (MVC Repository)
- **Database**: MSSQL Server.
- **Other Libraries**: PrimeNG for better UI development, html2pdf to covert HTML page to PDF.

## Challenges and Solutions
- **Challenge**: There was a primary challenge of processing HTML to PDF that we were not able to get desired output in PDF.
- **Solution**: We have used accordian with other HTML elements to capture data with better readability but the textarea needed to handled using DOM manipulation while generating PDF.

- **Challenge**: The challenge of accordian was also there when were trying to download PDF.
- **Solution**: We needed to add proper flags in functions by debugging the code through the browser's console, to make sure that accordian is Expanded with all its item expanded.

## Results

### 1. Ease access of survey link
   - **Email link is accessed through Email**: Users can access survey link through their emails and submit survey using few taps or clicks.
   - **Impossible Redundent submition of same survey**: If user have submitted the survey already and when he/she tries to access same link again it redirects to already submitted page.

### 2. Enhanced Data Visibility and Transparency
   - **Real-Time Overview**: Users can see on dashboard data regarding clients and projects and their respective surveys, whether they are submitted or not.
   - **Resend survey**: If user is willing to resend the email containing survey link he/she can do so.
