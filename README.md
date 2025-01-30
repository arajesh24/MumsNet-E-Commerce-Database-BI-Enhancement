# MumsNet E-Commerce Database & BI Enhancement Project

## Overview
This was a group project of 6 members where I specifically focused on Deliverable 2 (D2) - the Business Intelligence platform implementation using Microsoft SQL Server Analysis Services (SSAS/SSDT). The project involved redesigning MumsNet's database system and implementing a new business intelligence platform to analyze their online store data.

## Project Structure
```
Database
  └── Group15-D1.bak
BI_Solution
  ├── Group15-D2/
  │   └── Group15-D2.sln
```

## My Contribution - Business Intelligence Platform (D2)
I developed a comprehensive 'proof of concept' BI solution that successfully met all business requirements for data analysis using SSAS. The solution included creating appropriate Data Source Views (DSV) and designing corresponding Cube measures and dimensions.

### Business Requirements Implemented
The BI platform delivers the following analytics capabilities:

#### Order Analysis
- Number and percentage of cancelled orders
- Sales value of cancelled orders
- Number and percentage of unfulfilled basket orders (due to out-of-stock items)
- Percentage of abandoned basket orders
- Percentage of fulfilled orders
- All percentages calculated against total orders placed

#### Hierarchical Analysis
- Customer hierarchy: Customer → City → Region → Country
- Product hierarchy: Product Variant → Product → Product Group
- Time hierarchy: Day → Month → Quarter → Year

#### Detailed Metrics
- Sales and quantity sold breakdowns by:
  - Product
  - Customer
  - Day
- Ordered stock quantity by:
  - Product
  - Ordered day
- All product calculations at product variant level

## Technologies Used
- Microsoft SQL Server 2018
- SQL Server Analysis Services (SSAS/SSDT)
- Microsoft Visual Studio with SSDT installed

## Setup Instructions

### Database Restoration (Group15-D1.bak)
1. Save the .bak file locally (recommended: C:/Users/Public)
2. Open Microsoft SQL Server Management Studio
3. Right-click on "Databases" in Object Explorer
4. Select "Restore Database"
5. Choose "Device" and click "..."
6. Click "Add" and navigate to the .bak file location
7. Select the file and click "OK"
8. Verify the restore settings and click "OK" to restore the database

### Business Intelligence Solution (Group15-D2.sln)
1. Open Visual Studio with SQL Server Data Tools
2. Go to File → Open → Project/Solution
3. Navigate to the Group15-D2 folder
4. Select the Group15-D2.sln file and click "Open"
5. In Solution Explorer, double-click the .cube file
6. Deploy the solution to your local SSAS instance

## Prerequisites
- Microsoft SQL Server 2018
- SQL Server Management Studio
- Visual Studio with SSDT installed

## Important Notes
- Solution compatible with SQL Server 2018
- Database contains MumsNet data from 2005-2009

## Troubleshooting
1. Database Restore Issues:
   - Save .bak file in C:/Users/Public for proper permissions
   - Verify SQL Server service is running
   - Check database compatibility level

2. BI Solution Issues:
   - Ensure SSAS is properly configured
   - Verify all required features are installed in Visual Studio
   - Check Data Source connection settings

## Project Components
1. D1 - Database Design (.bak file)
2. D2 - Business Intelligence Solution (.sln)

## Version
1.0.0
Note: This project contains real business data and is intended for academic purposes only.
