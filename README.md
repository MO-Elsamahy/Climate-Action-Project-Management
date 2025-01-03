# Climate-Action-Project-Management

**A structured SQL Server database designed to manage climate action projects efficiently, ensuring effective tracking of activities, budgets, funders, locations, milestones, risks, stakeholders, and teams.**

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Database Structure](#database-structure)
- [Usage](#usage)
- [License](#license)

## Overview
The **Climate Action Project Management Database** provides a comprehensive solution to organize, monitor, and report on climate-related projects. It facilitates collaboration among stakeholders and ensures transparency and accountability through detailed schemas and tables.

## Features
- **Project Tracking**: Track projects with detailed information on activities, budgets, and milestones.
- **Budget Management**: Manage allocated and spent funds with real-time updates on remaining budgets.
- **Stakeholder Integration**: Maintain detailed records of funders, stakeholders, and task assignments.
- **Geographic Data**: Store and query project locations with latitude and longitude coordinates.
- **Customizable Schemas**: Modular schema design for scalability and flexibility.

## Database Structure

### Schemas
- **ActivitiesSchema**: Manage project activities and task assignments.
- **BudgetsSchema**: Monitor project budgets.
- **FundersSchema**: Track funding sources and amounts.
- **LocationsSchema**: Store project location data.
- **MilestonesSchema**: Record project milestones and their status.
- **ProjectsSchema**: Centralized project information.
- **ReportsSchema**: Generate and store project reports.
- **RisksSchema**: Identify and manage project risks.
- **StakeholdersSchema**: Maintain a list of stakeholders.
- **TeamsSchema**: Manage project teams.

### Key Tables
- `Activities`: Tracks project activities with details like start and end dates, and status.
- `Budgets`: Manages allocated, spent, and remaining funds for projects.
- `Funders`: Stores information on project funders.
- `Locations`: Holds geographic and address details for projects.
- `Milestones`: Tracks key project milestones and deadlines.

For a complete list of tables and schemas, refer to the script provided in this repository.

## Usage

1. Set up the database by executing the script in your SQL Server environment.
2. Populate the tables with project-related data using `INSERT` statements or through your preferred application interface.
3. Query the database for reports, project statuses, and financial insights.

Example query:
```sql
SELECT ProjectName, Budget, Status 
FROM ProjectsSchema.Projects 
WHERE Status = 'In Progress';
```

## License
This project is licensed under the [MIT License](LICENSE).
