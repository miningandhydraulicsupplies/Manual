# System Administration

## Overview

The Administration section provides system configuration, user management, and monitoring tools for administrators. Access is restricted to users with the Admin role.

## Admin Dashboard

### Accessing Admin Dashboard

Navigate to **Admin > Admin Dashboard** from the sidebar.

### Dashboard Overview

The admin dashboard displays:
- **System Health** - Status of all services
- **User Statistics** - Active users and sessions
- **Background Jobs** - Job status and performance
- **Database Status** - Connection and performance
- **Cache Status** - Redis connection and usage
- **API Status** - External API connectivity
- **Recent Activity** - Latest admin actions

## User Management

### Managing Users

Navigate to **Admin > Manage Users** to:
- View all system users
- Create new users
- Edit user details
- Reset passwords
- Assign roles
- Deactivate users

### Creating New Users

1. Navigate to **Admin > New User**
2. Fill in user details:
   - **Email** - User's email address (username)
   - **Full Name** - User's full name
   - **Password** - Initial password (must meet requirements)
   - **Confirm Password** - Password confirmation
3. Assign roles (can select multiple):
   - Admin
   - Sales
   - Warehouse
   - Production
   - Viewer
4. Click **Create User**

### Password Requirements

Passwords must:
- Be at least 6 characters long
- Contain at least one uppercase letter
- Contain at least one lowercase letter
- Contain at least one digit
- Contain at least one special character

### Editing Users

1. Navigate to **Admin > Manage Users**
2. Click **Edit** on desired user
3. Modify user details:
   - Email address
   - Full name
   - Roles
   - Active status
4. Click **Save Changes**

### Resetting Passwords

1. Navigate to **Admin > Manage Users**
2. Click **Reset Password** on user
3. Enter new password
4. Confirm password
5. Click **Reset**
6. User will be notified of password change

### User Mapping

Link WMS users to MomentumPro users:

1. Navigate to **Admin > User Mapping**
2. Select WMS user
3. Select corresponding MomentumPro user
4. Click **Map User**

**Benefits of User Mapping**:
- Personal order dashboards
- Performance tracking
- KPI attribution
- Sales rep assignment

## Permission Management

### Permission System

The system uses granular permissions for access control.

### Viewing Permissions

Navigate to **Admin > Permissions** to see:
- All defined permissions
- Permission descriptions
- Assigned roles
- Usage statistics

### Creating Permissions

1. Navigate to **Admin > Permissions**
2. Click **Create Permission**
3. Enter permission details:
   - **Name** - Permission identifier
   - **Display Name** - Human-readable name
   - **Description** - What permission allows
   - **Category** - Permission grouping
4. Click **Create**

### Managing Role Permissions

1. Navigate to **Admin > Manage Role Permissions**
2. Select role to configure
3. Check/uncheck permissions
4. Click **Save Changes**

### Default Permissions

**Admin Role**:
- Full system access
- User management
- System configuration
- All feature access

**Sales Role**:
- Order management
- Quote management
- Customer notifications
- Personal dashboards
- Label printing

**Warehouse Role**:
- Inventory management
- Stocktakes
- Label printing
- GRN monitoring
- Counter collect

**Production Role**:
- Production order monitoring
- Production labels
- Material tracking

**Viewer Role**:
- Read-only access
- Dashboard viewing
- Report viewing

## Printer Configuration

### Managing Printers

Navigate to **Admin > Printer Settings** to:
- View configured printers
- Add new printers
- Edit printer settings
- Test printer connectivity
- Set default printers

### Adding a Printer

1. Navigate to **Admin > Printer Settings**
2. Click **Add Printer**
3. Enter printer details:
   - **Printer Name** - Descriptive name
   - **IP Address** - Network IP address
   - **Port** - Printer port (usually 9100)
   - **Printer Type** - Zebra, Complypro, etc.
   - **Label Types** - Supported label types
   - **Default** - Set as default for label type
4. Click **Save**

### Testing Printers

1. Navigate to **Admin > Printer Settings**
2. Click **Test** on printer
3. System sends test print
4. Verify label prints correctly

### Printer Troubleshooting

If printer issues occur:
1. Check IP address is correct
2. Verify printer is on network
3. Test connectivity with ping
4. Check printer supplies
5. Restart printer if necessary
6. Update printer configuration

## Background Jobs

### Job Monitoring

Navigate to **Admin > Background Jobs** to:
- View all background jobs
- Check job status
- View job history
- Configure job settings
- Manually trigger jobs

### Background Job Types

**Order Monitoring**:
- Syncs sales orders from MomentumPro
- Runs every 10 minutes
- Checks for new and updated orders

**Production Order Monitoring**:
- Syncs production orders
- Runs every 30 minutes
- Updates order status

**GRN Monitoring**:
- Tracks goods receipt notes
- Runs every 30 minutes
- Checks for backorder fulfillment

**Quote Monitoring**:
- Syncs quotes from MomentumPro
- Runs every 15 minutes
- Tracks quote conversions

**Calibration Reminders**:
- Sends calibration due reminders
- Runs daily at 8:00 AM
- Emails customers and staff

**KPI Capture**:
- Captures KPI snapshots
- Runs every 30 minutes
- Stores historical data

**Counter Collect Monitoring**:
- Scans for customer pickup orders
- Runs every 15 minutes
- Sends reminder notifications

### Configuring Jobs

1. Navigate to **Admin > Background Jobs**
2. Click **Edit** on job
3. Modify settings:
   - **Enabled** - Enable/disable job
   - **Interval** - How often job runs
   - **Timeout** - Maximum execution time
   - **Retry Attempts** - Number of retries on failure
4. Click **Save**

### Job History

View job execution history:
- Execution timestamp
- Duration
- Success/failure status
- Error messages
- Records processed

### Manual Job Execution

Trigger jobs manually:
1. Navigate to **Admin > Background Jobs**
2. Click **Run Now** on job
3. Job executes immediately
4. View results in history

## System Logs

### Viewing Logs

Navigate to **Admin > System Logs** to:
- View application logs
- Filter by severity
- Search log messages
- Export logs
- Monitor errors

### Log Levels

- **Information** - General information
- **Warning** - Potential issues
- **Error** - Errors that occurred
- **Critical** - Critical failures

### Filtering Logs

Filter by:
- **Date Range** - Specific time period
- **Log Level** - Severity level
- **Category** - Log category
- **User** - Specific user actions
- **Event Type** - Type of event

### Searching Logs

Search capabilities:
- Full-text search
- Regex patterns
- Multiple keywords
- Case-sensitive/insensitive

### Exporting Logs

Export options:
- **Download** - Download log file
- **Email** - Email logs to admin
- **Archive** - Archive old logs

## Customer Management

### Managing Customers

Navigate to **Admin > Customers** to:
- View all customers
- Add new customers
- Edit customer details
- Manage customer contacts
- Configure notification preferences

### Customer Information

For each customer:
- Company name
- Contact person
- Email address
- Phone number
- Physical address
- Billing address
- Customer code (from MomentumPro)
- Active status

### Customer Contacts

Manage multiple contacts per customer:
- Primary contact
- Billing contact
- Technical contact
- Additional contacts

### Notification Preferences

Configure per customer:
- Email notifications enabled
- Notification types
- Contact preferences
- Reminder settings

## API Keys

### Managing API Keys

Navigate to **Admin > API Keys** to:
- View active API keys
- Create new API keys
- Revoke API keys
- Monitor API usage

### Creating API Keys

1. Navigate to **Admin > API Keys**
2. Click **Create API Key**
3. Enter details:
   - **Client Name** - Application name
   - **Description** - Purpose of key
   - **Permissions** - API access level
   - **Expiration** - Optional expiry date
4. Click **Generate**
5. Copy API key (shown once only)

### API Key Security

- Keys are hashed in database
- Cannot be retrieved after creation
- Revoke compromised keys immediately
- Rotate keys regularly
- Monitor usage for anomalies

## Queue Monitoring

### Viewing Queue Status

Navigate to **Admin > Queue Monitoring** to:
- View API queue status
- Monitor queue backlog
- Check stuck queries
- View queue health metrics

### Queue Metrics

- **Queue Length** - Items in queue
- **Processing Rate** - Items per second
- **Average Wait Time** - Time in queue
- **Stuck Queries** - Queries over threshold
- **Failed Queries** - Recent failures

### Queue Management

Actions available:
- **Clear Queue** - Remove all items
- **Retry Failed** - Retry failed items
- **Pause Queue** - Temporarily stop processing
- **Resume Queue** - Resume processing

## Weekly Reports

### Report Configuration

Navigate to **Admin > Weekly Reports** to:
- Configure report schedule
- Set recipients
- Customize report content
- View report history

### Report Settings

- **Day of Week** - When to send (default: Thursday)
- **Time of Day** - Send time (default: 9:00 AM)
- **Recipients** - Email addresses
- **Test Mode** - Send to test address only
- **Enabled** - Enable/disable automated sending

### Report Content

Weekly reports include:
- Order statistics
- Production summary
- Backorder status
- Performance metrics
- User activity

### Manual Report Generation

1. Navigate to **Admin > Weekly Reports**
2. Click **Generate Report**
3. Select date range
4. Choose recipients
5. Click **Send Report**

## System Configuration

### Application Settings

Configure system-wide settings:
- **Application Name** - Display name
- **Company Information** - Company details
- **Time Zone** - System timezone (Australia/Perth)
- **Date Format** - Display format
- **Currency** - Default currency

### Email Configuration

Configure email settings:
- **SMTP Provider** - Email service (SMTP2Go)
- **Sender Email** - From address
- **Sender Name** - From name
- **Reply-To Email** - Reply address
- **BCC Email** - Always BCC address

### Integration Settings

Configure external integrations:
- **MomentumPro API** - ERP integration
- **SimpleInOut** - Attendance tracking
- **AWS S3** - Document storage
- **OpenAI** - AI features
- **Hiverr** - Email monitoring

## Database Maintenance

### Database Health

Monitor database:
- Connection status
- Query performance
- Table sizes
- Index usage
- Slow queries

### Maintenance Tasks

Regular maintenance:
- **Vacuum** - Reclaim storage
- **Reindex** - Rebuild indexes
- **Analyze** - Update statistics
- **Backup** - Database backup

### Backup and Restore

- Automated daily backups
- Manual backup on demand
- Point-in-time recovery
- Backup verification

## Security

### Security Best Practices

1. **Strong Passwords** - Enforce password policy
2. **Regular Updates** - Keep system updated
3. **Access Control** - Limit admin access
4. **Audit Logs** - Monitor admin actions
5. **API Security** - Protect API keys
6. **Network Security** - Use HTTPS
7. **Data Encryption** - Encrypt sensitive data

### Security Monitoring

Monitor for:
- Failed login attempts
- Unusual activity patterns
- API abuse
- Unauthorized access attempts
- Data export activities

## Related Features

- [User Management](user-management.md) - Detailed user guide
- [Permissions](permissions.md) - Permission system details
- [Background Jobs](background-jobs.md) - Job configuration
- [System Logs](system-logs.md) - Log analysis
