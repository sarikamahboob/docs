# Digicon HRMS - Technical Documentation


## Overview

Digicon HRMS is a comprehensive Human Resource Management System designed to efficiently manage and streamline your organization's HR processes. It stands as a powerful and flexible tool, offering support for every facet of your HR operations. By automating diverse processes and providing intuitive interfaces, it empowers both administrators and employees to streamline their workflows and concentrate on strategic initiatives.


## Authors

- [rakibulhasan](https://github.com/rakibul-hasan-1)

- [sarikamahboob](https://github.com/sarikamahboob)


**_\*For credentials and inquiries, please contact the authors._**


## Target Audience

HR professionals, administrators, and employees of organizations using Digicon HRMS.


## Technology Stack

The "Digicon HRMS" project utilizes a combination of front-end, back-end, and database technologies to deliver its functionalities effectively. These include:

- <u>**Front-end Technologies:**</u>
  - Next Js
  - Ant Design
  - Redux
  - Typescript
  - Deck.gl
  - Maplibre GL
  - React map GL
  - Husky
  - Eslint

- <u>**Back-end Technologies:**</u>
  - Laravel
  - PHP
  - PostgreSQL
  - PostGIS

- <u>**Additional Technologies:**</u>
  - Git
  - Docker
  - NGINX
  - Sentry


## Key Features

- **Recruitment Management**: Effortlessly streamline your hiring process, attracting and onboarding the best talent.

- **Personnel Management**: Maintain a centralized hub for all employee data, simplifying organization and recordkeeping.

- **Role and Permission Management**: Granular control over access to sensitive information and functionalities, ensuring data security and compliance.

- **Multiple Type Attendance Supports**: Track and analyze employee attendance in various forms (e.g., in-office, remote, flex hours), enabling accurate work-time management.

- **Office Transport System**: Effectively manage employee commutes, optimizing transportation logistics.

- **Automated Payroll Processing**: Simplify payroll calculations and ensure compliance with regulations, saving time and resources.

- **Rostering**: Create and manage work schedules with user assignments, fostering efficient team collaboration.

- **Security and Access Control**: Implement role-based access control (RBAC) to ensure data security and user privileges align with their roles.


## User and Admin Roles

### User Role

As a user, you have limited access compared to admins, primarily focused on submitting requests and accessing specific information relevant to your role within the organization. Here's an overview of the access privileges associated with the user role:

* **Attendance**: Users can check their own attendance records.
* **Announcement**: Users can make announcements, view, and update their own announcements.
* **Leave Request**: Users can request for leaves.
* **Expense Request**: Users can submit their expenses for approval.
* **Exception Approval**: Users can request exceptional approvals.
* **Resign**: Users can submit their resignation
* **Office Transport**: Users can request for office transport.

Users can only view and manage their own information. By default, the user role is not contingent upon any specific roles and permissions. However, if there is a roles permission list for the user, then it will be counted.

### Admin Role

An admin user has more privileges, and their workflow depends on roles and permissions. They can perform all the actions a user can, for themselves and for others. This includes:

* Posting requests for themselves.
* Taking action on requests from other users.

The specific actions an admin can perform depend on their assigned roles and permissions.


## Functionality Breakdown

### Login

- **Login Credentials**: Anyone can access the dashboard with their DG ID or email and a password.

- **Provision by Admin**: DG ID or email and password are provided by an admin when onboarding a new user.

- **Password Reset Request**: Users can request a password reset if they have a valid email address.

- **Password Reset Process**: Upon requesting a password reset, an email containing a reset password link is sent.

- **Reset Procedure**: Clicking the link redirects the user to the reset password page of the Digicon HRMS website, where they can set a new password to replace the old one.

### Dashboard Overview

The Dashboard Overview provides a quick overview of key metrics and details, consisting of two types of information: counts and details.

For instance, it displays the total number of employees. Clicking on the 'Total Employees' card opens a popup displaying details of these employees.

The Dashboard includes the following metrics:

* Total Employees: Displays the total number of employees. Clicking on this opens a popup with the details of all employees.
* Total Males: Displays the total number of male employees.
* Total Females: Displays the total number of female employees.
* Total Processes: Displays the total number of processes.
* Former Employees: Displays the number of former employees.
* Total Present: Displays the total number of employees who are present.
* Total Late: Displays the total number of employees who are late.
* Total On Time: Displays the total number of employees who are on time.
* Total Absent: Displays the total number of employees who are absent.
* Chart Section:  This section provides a visual representation of employee attendance metrics, including:
  * On Time: Shows the percentage of employees who arrived on time.
  * Late: Shows the percentage of employees who were late.
  * Absent: Shows the percentage of employees who were absent.
  * Leave: Shows the percentage of employees who were on leave.
  * WFH (Work From Home): Shows the percentage of employees who were working from home.

The values for Total Employees, Total Male, Total Female, Total Processes, and Former Employees do not depend on any filters. However, the values for other metrics on the Dashboard will depend on the date range, process, and branch filters.

**_Only users with the Admin role and type can access the Dashboard Overview section._**

### Attendance

Dive into the attendance details with two submenus:

- **Daily Attendance**: Get a day-to-day breakdown of attendance. The daily attendance table showcases attendance status (Device, Biometric, System), attendance time, and working hours. For System attendance, only working hours are displayed. Device attendance data also includes check-in and check-out locations. You can use filters like date, designation, process, branch, or search by name and DG ID. Both users and admins can also export the table data.

- **Monthly Attendance**: This view provides a day-by-day breakdown of attendance for the current month. If there are multiple types of attendance data (Device, Biometric, System), they are displayed serially for each day. Same as daily attendance, you can apply the same filters, and only admins can export the table data.

**_Anyone with the user or admin role can view the daily and monthly attendance._**

### Announcement

The Announcement section serves as a communication hub:

- **Employees**: Employees can post announcements and update their own announcements only. They can also view announcements posted by other employees in the table.

- **For Admins**: Admins have the ability to post announcements for all users and can view all users announcements in the table. Admins can update their own announcements only. Additionally, admins can add announcement types, which will be displayed when an employee is creating an announcement.

Date, announcement types, branch, and name filters are also available, which will be applied to the announcement table.

**_Under the same process, everyone will receive notifications for announcements made by employees, which will be shown in the top nav bar._**

## Employee

### Add Employee
This section allows you to add employees individually or in bulk.

### Current Employee
This section lists all current employees. You can apply filters to this list and even export the entire list with all details. In this section, you can update employee details or remove an employee from the current list. Note that removing an employee here doesn't permanently delete them, but moves them to the 'Formal Employee' list.

### Formal Employee
This section lists all employees who have been removed from the 'Current Employee' list. You can view these employees and even restore them back to the 'Current Employee' list if needed.


Please note, some metrics on the Dashboard may vary based on the filters applied.
