# Calibration Tracking

## Overview

The Calibration Tracking system manages equipment calibration schedules, certificates, and reminders for customer-owned equipment. It ensures compliance with calibration requirements and provides automated notifications for upcoming calibrations.

## Dashboard

### Accessing Calibration Dashboard

Navigate to **Calibration Tracking** from the Operations section.

### Dashboard Metrics

The dashboard displays:
- **Total Equipment** - All tracked equipment
- **Active Equipment** - Currently in service
- **Due Soon** - Calibrations due within 30 days
- **Overdue** - Equipment past calibration date
- **Calibrations This Month** - Scheduled for current month
- **Upcoming Reminders** - Pending reminder notifications

### Quick Views

- **Equipment Due Soon** - Top 10 items needing calibration
- **Overdue Equipment** - All overdue items
- **Recent Calibrations** - Last 10 calibrations performed
- **Upcoming Calibrations** - Next 30 days schedule

## Equipment Management

### Adding New Equipment

1. Navigate to **Calibration > Equipment**
2. Click **Add Equipment** button
3. Fill in equipment details:

**Required Fields**:
- **Customer** - Select from customer list
- **Equipment Type** - Type of equipment (Flowmeter, Gauge, etc.)
- **Serial Number** - Unique equipment identifier
- **Calibration Interval** - Months between calibrations

**Optional Fields**:
- **Manufacturer** - Equipment manufacturer
- **Model** - Model number
- **Description** - Additional details
- **Purchase Date** - When equipment was purchased
- **Invoice Number** - Purchase invoice reference
- **Sales Order Number** - Original sales order
- **Location** - Where equipment is installed
- **Status** - Active, Inactive, Retired
- **Notes** - Additional information

4. Click **Save**

### Equipment Details

View complete equipment information:
- Equipment specifications
- Customer information
- Calibration history
- Uploaded certificates
- Reminder settings
- Status and location

### Editing Equipment

1. Navigate to equipment list
2. Click **Edit** on desired equipment
3. Modify fields as needed
4. Click **Save Changes**

### Equipment Status

**Active** - Equipment in service, calibrations tracked
**Inactive** - Equipment not in use, no reminders sent
**Retired** - Equipment decommissioned, archived

## Calibration Records

### Recording a Calibration

1. Open equipment details
2. Click **Record Calibration** button
3. Enter calibration details:
   - **Calibration Date** - When calibration was performed
   - **Certificate Number** - Calibration certificate reference
   - **Performed By** - Technician or company
   - **Next Due Date** - Calculated automatically or manual entry
   - **Results** - Pass/Fail/Conditional
   - **Notes** - Calibration notes
   - **Certificate File** - Upload PDF certificate

4. Click **Save Calibration**

### Calibration History

View complete calibration history:
- All past calibrations
- Dates and certificate numbers
- Who performed calibration
- Results and notes
- Uploaded certificates
- Next due dates

### Certificate Management

**Uploading Certificates**:
1. Record calibration or edit existing
2. Click **Upload Certificate**
3. Select PDF file
4. File is stored securely
5. Accessible from equipment details

**Downloading Certificates**:
1. Open equipment details
2. View calibration history
3. Click certificate link
4. PDF downloads automatically

**Certificate Storage**:
- Stored in secure file system
- Organized by equipment and date
- Backed up regularly
- Accessible to authorized users

## Reminder System

### Configuring Reminders

For each equipment item:
1. Edit equipment details
2. Enable reminders checkbox
3. Set reminder days before due date
4. Save settings

**Default Reminder Schedule**:
- 30 days before due
- 14 days before due
- 7 days before due
- On due date
- 7 days after due (overdue)
- 14 days after due (overdue)

### Reminder Notifications

Reminders are sent via email to:
- Customer contact (if configured)
- Internal calibration coordinator
- BCC to warehouse email

**Reminder Content**:
- Equipment details
- Current calibration status
- Due date
- Customer information
- Contact information for scheduling

### Reminder History

Track all sent reminders:
- Date and time sent
- Recipients
- Reminder type (upcoming/overdue)
- Email delivery status

## Customer Management

### Customer Information

For each customer:
- Company name
- Contact person
- Email address
- Phone number
- Address
- Equipment list

### Customer Equipment List

View all equipment for a customer:
- Filter by customer
- See all calibration statuses
- Bulk operations available
- Export customer equipment list

### Customer Notifications

Configure per customer:
- Enable/disable notifications
- Custom reminder schedule
- Multiple contact emails
- Notification preferences

## Searching and Filtering

### Search Equipment

Search by:
- Serial number
- Equipment type
- Customer name
- Manufacturer
- Model number
- Certificate number

### Filter Options

Filter equipment by:
- **Customer** - Specific customer
- **Equipment Type** - Type of equipment
- **Status** - Active, Inactive, Retired
- **Calibration Status** - Current, Due Soon, Overdue
- **Location** - Equipment location

### Sorting

Sort equipment list by:
- Next due date
- Last calibration date
- Customer name
- Equipment type
- Serial number

## Reporting

### Available Reports

**Equipment Status Report**:
- All equipment with current status
- Due dates and overdue items
- Export to Excel

**Calibration Schedule Report**:
- Upcoming calibrations by month
- Resource planning
- Customer breakdown

**Overdue Equipment Report**:
- All overdue equipment
- Days overdue
- Customer contact information

**Customer Equipment Report**:
- Equipment by customer
- Calibration history
- Certificate status

### Exporting Data

Export options:
- **Excel** - Formatted spreadsheet
- **CSV** - Raw data export
- **PDF** - Formatted report

## Automated Processes

### Background Services

The system automatically:
- Calculates next due dates
- Sends reminder emails
- Updates equipment status
- Tracks overdue equipment
- Generates daily reports

### Daily Reminder Processing

Every day at 8:00 AM (Perth time):
- System checks all equipment
- Identifies items needing reminders
- Sends email notifications
- Logs reminder activity
- Updates reminder history

### Status Updates

Equipment status automatically updates:
- **Current** - Within calibration period
- **Due Soon** - Within 30 days of due date
- **Overdue** - Past due date
- **Critical** - More than 30 days overdue

## Best Practices

### Equipment Setup

1. **Complete all fields** - Provide comprehensive information
2. **Verify serial numbers** - Ensure accuracy
3. **Set correct intervals** - Match customer requirements
4. **Enable reminders** - Don't miss calibrations
5. **Add notes** - Document special requirements

### Calibration Recording

1. **Record promptly** - Enter calibrations immediately
2. **Upload certificates** - Attach PDF certificates
3. **Verify dates** - Check next due date calculation
4. **Add notes** - Document any issues or findings
5. **Update status** - Ensure equipment status is current

### Customer Communication

1. **Proactive reminders** - Send reminders early
2. **Clear communication** - Provide all necessary details
3. **Follow up** - Track response to reminders
4. **Document interactions** - Note all communications
5. **Coordinate scheduling** - Help arrange calibrations

### Maintenance

1. **Regular reviews** - Check equipment list monthly
2. **Update customer info** - Keep contacts current
3. **Archive retired equipment** - Clean up inactive items
4. **Verify certificates** - Ensure all certificates uploaded
5. **Monitor overdue items** - Follow up on overdue calibrations

## Troubleshooting

### Reminder Not Sent

If reminder wasn't sent:
1. Check reminder is enabled for equipment
2. Verify customer email address
3. Check reminder history
4. Ensure equipment is active
5. Contact admin if issue persists

### Certificate Upload Failed

If certificate won't upload:
1. Check file is PDF format
2. Verify file size (max 10MB)
3. Ensure stable internet connection
4. Try different browser
5. Contact admin if problem continues

### Incorrect Due Date

If due date is wrong:
1. Check calibration interval setting
2. Verify last calibration date
3. Manually adjust if needed
4. Recalculate from last calibration
5. Document reason for adjustment

## Integration

### Customer Database

- Links to customer management system
- Syncs customer information
- Updates contact details
- Tracks customer equipment

### Email System

- Integrates with SMTP2Go
- Sends automated reminders
- Tracks delivery status
- Handles bounced emails

## Related Features

- [Customer Management](customer-management.md) - Customer database
- [Notifications](notifications.md) - Email notification system
- [Admin Settings](administration.md) - System configuration
