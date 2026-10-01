# Script-Controlled ACL – Branch-Based Record Access in ServiceNow

## Project Description

This project implements role-based and branch-based access control in ServiceNow using Access Control Lists (ACLs).

A custom Institution Details table stores student information. Users with the designated read role can view only records whose Branch is EEE, while administrators retain access to records from all branches.

Separate roles control permission to create, edit, and delete records.

## Features

- Custom Institution Details table with automatically generated student roll numbers.
- Student and faculty reference fields linked to ServiceNow users.
- Branch choices: EEE, ECE, and CSE.
- Script-controlled read ACL combined with a branch condition.
- Separate ACLs for create, write, and delete operations.
- Administrator access through Admin overrides.
- Access verification using user impersonation.

## Roles and Permissions

| Role | Permission |
|------|------------|
| bb1 | Read records where Branch is EEE |
| bb2 | Create records |
| bb3 | Write permission to edit records |
| bb4 | Delete permission |
| admin | Full access to records from all branches |

## Table Details

**Table:** Institution Details  
**Technical name:** `u_institution_details`

Fields:
- Student Roll Number – Auto-numbered
- Student Name – Reference to User
- Faculty Name – Reference to User
- Branch – Choice
- Email – String
- Phone Number – String
- Description – Multiline text

## Technologies Used

- ServiceNow Personal Developer Instance
- Access Control Lists (ACLs)
- JavaScript
- Custom tables and fields
- User administration and roles
- User impersonation

## Learning Outcome

This project demonstrates how user roles, record conditions, and scripts work together to enforce access control in ServiceNow.

## Project Context

Completed as part of the TN Skills ServiceNow micro-project.

## Project Demo

[Watch or download the demo video](./Demo%20Video.mp4)
