 
# Timesheet Portal
## Overview
This is a timesheet management portal designed to log billable and non-billable hours across the week. The tool streamlines the process of time tracking and provides a structured, easy-to-use interface for recording work hours.

## My Contributions
- **Billable and Non-Billable Task Tracking**
- **Dynamic Task Management** (Add/Remove Tasks)
- **Summary Totals**
- **Implemented backend logic using Repository Pattern** (Kept Data access and Business logic separate)

## Technologies Used
- **Frontend**: Angular, HTML, CSS
- **Backend**: .NET (MVC Repository Pattern)
- **Database**: MSSQL Server.
- **Other Libraries**: PrimeNG for better UI development.

## Challenges and Solutions
- **Challenge**: There was a challenge which was kind of part of validation where we wanted to clear the row values when we change any of the drop down of Project and Task.
- **Solution**: We assigned unique ID for each row and passed it on onChange of Project and Task, which helped to clear the required rows values of task and hours.

## Results

### 1. Improved Time Tracking Efficiency
   - **Reduced Time to Log Hours**: Users can log hours for billable and non-billable tasks in less than 2 minutes due to the streamlined layout and easy task addition/removal.
   - **Fewer Errors in Timesheet Submission**: The structured input fields reduce common errors such as incorrect project/task selection and missed entries.

### 2. Enhanced Data Visibility and Transparency
   - **Real-Time Overview**: Users can see an overview of their hours for the week at a glance, including total billable and non-billable hours.
   - **Clear Separation of Task Types**: By displaying billable and non-billable tasks in separate sections, users have better transparency and can easily identify where they are spending their time.

### 3. Personalized Project and Task Display
   - **User-Specific Data Retrieval**: The portal fetches projects and tasks dynamically based on the logged-in user, ensuring that users only see projects and tasks relevant to their roles and assignments.
   - **Efficient Data Loading**: When users log in, the application makes a call to the API, which returns a JSON response with all relevant data, including user-specific project and task lists. This reduces the load on the frontend by avoiding unnecessary data and provides a tailored experience.
   - **Enhanced User Experience**: By filtering projects and tasks according to each user, the portal minimizes the time needed to locate relevant tasks, improving accuracy in timesheet entries and reducing frustration from searching through irrelevant options.

### 4. Potential for Improved Project Planning and Cost Management
   - **Accurate Time Data for Projects**: The portal provides with accurate, real-time data on hours spent on projects, enabling better resource allocation and cost forecasting.
   - **Reduction in Non-Billable Hours**: Managers can analyze non-billable hours more effectively, identifying potential areas for optimization.

### 5. Future Metrics
   - **Expected Impact**: Over time, the portal is expected to reduce timesheet-related administrative tasks by 20%, freeing up time for more productive work.
   - **Scalability**: The tool is designed to be scalable, allowing for additional features such as automated reporting and approval workflows without significant rework.
