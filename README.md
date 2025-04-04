# Airtable License Portal

A web-based license management system that integrates with Airtable to track and manage software licenses and trials. Built with vanilla JavaScript and Bootstrap, this application provides an intuitive interface for managing user licenses, trial periods, and license analytics.

## Features

### Trial Manager
- Track trial user requests and conversions
- Search functionality for trial users by email
- Visual analytics with charts showing trial conversion rates
- Date range filtering for trial data
- Export capabilities for trial data

### License Manager
- Manage organization licenses and assignments
- Search functionality by organization, assignee, or Stripe email
- Add new organizations and assignees
- Track license expiration dates
- Generate PDF reports for organization license details
- Real-time updates to Airtable
- Change logging for license modifications

### CSV Prep Tool
- Process and validate license CSV files
- Match and verify Stripe email addresses
- Generate properly formatted CSV files for Airtable sync
- Identify and report unmatched or incorrect email addresses

## Setup

1. Clone the repository
2. Update the Airtable configuration in each file:
   ```javascript
   const airtableApiKey = 'your-api-key';
   const airtableBaseId = 'your-base-id';
   ```
3. Deploy the files to a web server or open locally in a browser

## File Structure

- `airtable_trial_manager.html` - Interface for managing trial users
- `airtable_license_manager.html` - Interface for managing licenses
- `prep2.html` - CSV preparation tool for license data

## Dependencies

- Bootstrap 5.3.0
- Axios
- Chart.js
- PapaParse
- FileSaver.js
- jsPDF

## Features in Detail

### Trial Manager
- View all trial requests
- Track trial creation and conversion status
- Filter trials by date range
- Search trials by email
- View analytics through line and pie charts
- Track trial conversion rates

### License Manager
- View all organization licenses
- Add new organizations
- Add/modify assignees
- Update license expiration dates
- Update Stripe email addresses
- Generate PDF reports
- Track license changes
- Search functionality

### CSV Prep Tool
- Process license CSV files
- Validate Stripe email addresses
- Generate formatted output for Airtable sync
- Track unmatched or incorrect emails
- Export results in CSV format

## Usage

1. Navigate between tools using the navigation buttons at the top of each page
2. Use the search functionality to find specific records
3. Make changes directly in the editable fields
4. Add new organizations or assignees using the provided buttons
5. Generate reports or download data as needed

## Change Logging

The system automatically logs the following changes to Airtable:
- New organization creation
- License assignments
- License modifications
- Trial status changes
