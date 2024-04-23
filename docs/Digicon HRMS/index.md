# Digicon HRMS - Technical Documentation

## Overview

Digicon HRMS is a comprehensive Human Resource Management System designed to manage and streamline the HR processes of your organization. It is a powerful and flexible tool that offers support for every aspect of your HR operations.

## Features

- **Recruitment Management**: Streamline your hiring process and get the right talent onboard.
- **Personnel Management**: Keep track of all employee information in one place.
- **Office Transport System**: Manage your office commute efficiently.
- **Role and Permission Management**: Control access to sensitive information and tasks.
- **Multiple Type Attendance Supports**: Track and manage employee attendance in various forms.
- **Payroll Processing**: Simplify your payroll with automated calculations and compliance.

## User and Admin Roles

### User Role

A user in our system has access to the following features:

* Attendance: Users can check their own attendance records.
* Leave Request: Users can request for leaves.
* Expense: Users can submit their expenses for approval.
* Exception Approval: Users can request for exception approvals.
* Resign: Users can submit their resignation.
* Office Transport: Users can request for office transport.
* Announcement: Users can view announcements.

Users can only view and manage their own information. The user role does not depend on any specific roles and permissions.

### Admin Role

An admin user has more privileges and their work procedure depends on roles and permissions. They can perform all the actions a user can, for themselves and for others. This includes:

* Posting requests for themselves.
* Taking action on requests from other users.

The specific actions an admin can perform depends on their assigned roles and permissions.

## Dashboard Overview

The Dashboard provides a quick overview of key metrics and details. It consists of two types of information: counts and details.

For example, the total number of employees is displayed. When you click on the 'Total Employees' card, a popup will open displaying details of these employees.

The Dashboard includes the following metrics:

* Total Employees: Displays the total number of employees. Clicking on this will open a popup with the details of all employees.
* Total Male: Displays the total number of male employees.
* Total Female: Displays the total number of female employees.
* Total Processes: Displays the total number of processes.
* Formal Employees: Displays the number of formal employees.
* Total Present: Displays the total number of employees who are present.
* Total Late: Displays the total number of employees who are late.
* Total On Time: Displays the total number of employees who are on time.
* Total Absent: Displays the total number of employees who are absent.
* Chart Section: This section provides a visual representation of employee attendance metrics. It includes:
  * On Time: Shows the number of employees who arrived on time.
  * Late: Shows the number of employees who were late.
  * Absent: Shows the number of employees who were absent.
  * Leave: Shows the number of employees who were on leave.
  * WFH (Work From Home): Shows the number of employees who were working from home.

The values for Total Employees, Total Male, Total Female, Total Processes, and Formal Employees do not depend on any filters. However, the values for other metrics on the Dashboard will depend on the applied filters.

Only users with the Admin role can access the Dashboard Overview section.

## Attendance

Dive into the attendance details with two submenus:

- **Daily Attendance**: Get a day-to-day breakdown of attendance. Use filters like date, designation, process, branch, or search by name and DG ID. The table showcases attendance status (Device, Biometric, System) and attendance time. For System attendance, only working hours are displayed. Device attendance data also includes check-in and check-out locations.

- **Monthly Attendance**: This view provides a day-by-day breakdown of attendance for the current month. If there are multiple types of attendance data (Device, Biometric, System), they are displayed serially for each day.

## Announcement

The Announcement section serves as a communication hub:

- **For Employees**: Employees can post announcements and view only their own notifications in the table.
- **For Admins**: Admins have the ability to post announcements for all users and can view all users' announcements in the table.

## Employee

### Add Employee
This section allows you to add employees individually or in bulk.

### Current Employee
This section lists all current employees. You can apply filters to this list and even export the entire list with all details. In this section, you can update employee details or remove an employee from the current list. Note that removing an employee here doesn't permanently delete them, but moves them to the 'Formal Employee' list.

### Formal Employee
This section lists all employees who have been removed from the 'Current Employee' list. You can view these employees and even restore them back to the 'Current Employee' list if needed.


Please note, some metrics on the Dashboard may vary based on the filters applied.
