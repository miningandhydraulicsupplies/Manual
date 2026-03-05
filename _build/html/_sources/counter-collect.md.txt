# Counter Collect Management

## Overview

The Counter Collect system tracks customer pickup orders and manages the collection process. It automatically identifies orders marked for customer collection, sends reminder notifications, and provides a scanner interface for efficient pickup processing.

## Active Orders

### Viewing Active Orders

Navigate to **Counter Collect > Active Orders** to see:
- All orders awaiting customer collection
- Days waiting for each order
- Customer contact information
- Order status and details

### Order Information

Each order displays:
- **Invoice Number** - Sales order reference
- **Customer Name** - Who will collect
- **Days Waiting** - How long order has been ready
- **Status** - Waiting, Collected, or Cancelled
- **Added Date** - When order was identified
- **Notes** - Special instructions

### Status Indicators

**Color Coding**:
- **Green** - Recently added (0-6 days)
- **Yellow** - Waiting 7-13 days
- **Orange** - Waiting 14-20 days
- **Red** - Waiting 21+ days (urgent follow-up needed)

## Automatic Detection

### How Orders Are Identified

The system automatically scans for orders with carrier keywords:
- "collect"
- "pickup" / "pick up" / "pick-up"
- "counter collect"
- "customer collect"
- "will collect"

### Scanning Process

Background service runs every 15 minutes:
1. Scans all open sales orders
2. Checks carrier/delivery instructions
3. Identifies collection orders
4. Adds to Counter Collect list
5. Sends initial notification

## Collection Scanner

### Accessing Scanner

Navigate to **Counter Collect > Collection Scanner** for quick pickup processing.

### Using the Scanner

1. **Scan or Enter Invoice Number**
   - Use barcode scanner
   - Or manually type invoice number
   - Press Enter

2. **Verify Order Details**
   - Customer name
   - Order contents
   - Special instructions

3. **Confirm Collection**
   - Click **Mark as Collected**
   - Or scan next order

4. **Record Collector** (optional)
   - Enter collector name
   - Add notes if needed

### Scanner Features

- **Fast Entry** - Optimized for speed
- **Barcode Support** - Scan pickslip barcodes
- **Audio Feedback** - Beep on successful scan
- **Error Handling** - Clear error messages
- **History** - View recently collected orders

## Reminder System

### Automatic Reminders

The system sends email reminders at:
- **7 days** - First reminder
- **14 days** - Second reminder
- **21 days** - Third reminder
- **30 days** - Final reminder
- **45 days** - Escalation to management

### Reminder Content

Emails include:
- Order number and date
- Customer name and contact
- Days waiting
- Collection instructions
- Contact information

### Reminder Recipients

Reminders sent to:
- Customer (if email on file)
- Sales representative
- Warehouse team
- Management (for escalations)

### Escalation Process

For orders waiting 45+ days:
1. Email sent to supervisor
2. CC to manager
3. BCC to director
4. Requires management review
5. Decision: collect, cancel, or follow up

## Managing Orders

### Manual Actions

**Mark as Collected**:
1. Open order details
2. Click **Mark as Collected**
3. Enter collector name (optional)
4. Add collection notes
5. Save

**Cancel Order**:
1. Open order details
2. Click **Cancel**
3. Enter cancellation reason
4. Confirm cancellation

**Add Notes**:
1. Open order details
2. Click **Add Note**
3. Enter note text
4. Save

**Update Contact Info**:
1. Open order details
2. Click **Edit**
3. Update customer contact
4. Save changes

### Bulk Operations

Select multiple orders to:
- Send reminder emails
- Export to Excel
- Print collection list
- Update status

## Collection History

### Viewing History

Navigate to **Counter Collect > History** to see:
- All collected orders
- Collection dates and times
- Who collected each order
- Days waited before collection

### History Filters

Filter by:
- **Date Range** - Specific period
- **Customer** - Specific customer
- **Collector** - Who picked up
- **Days Waited** - Wait time range

### History Reports

Generate reports:
- **Collection Performance** - Average wait times
- **Customer Patterns** - Frequent collectors
- **Peak Times** - Busiest collection periods
- **Aging Analysis** - Wait time trends

## Customer Communication

### Notification Preferences

Configure per customer:
- Enable/disable reminders
- Preferred contact method
- Reminder frequency
- Escalation contacts

### Manual Notifications

Send ad-hoc notifications:
1. Select order
2. Click **Send Notification**
3. Choose template
4. Customize message
5. Send

### Notification Templates

Pre-configured templates:
- **Ready for Collection** - Initial notification
- **Reminder** - Follow-up reminder
- **Urgent** - Overdue collection
- **Custom** - Create your own

## Dashboard Widget

### Counter Collect Summary

Dashboard displays:
- **Active Orders** - Total awaiting collection
- **Waiting 7+ Days** - Orders needing follow-up
- **Waiting 14+ Days** - Urgent orders
- **Collected Today** - Today's collections

### Quick Actions

From dashboard:
- View all active orders
- Access collection scanner
- Send bulk reminders
- View collection history

## Integration

### Sales Order System

- Links to Order Monitoring
- Shows order details
- Updates order status
- Tracks order notes

### Email System

- Automated reminder emails
- Escalation notifications
- Collection confirmations
- Customer communications

### Reporting

- Included in KPI tracking
- Performance metrics
- Trend analysis
- Management reports

## Best Practices

### Daily Operations

1. **Morning Review** - Check overnight additions
2. **Follow Up** - Contact customers waiting 7+ days
3. **Process Collections** - Use scanner for pickups
4. **Update Notes** - Document all communications
5. **End of Day** - Review pending orders

### Customer Service

1. **Proactive Communication** - Don't wait for reminders
2. **Clear Instructions** - Provide collection details
3. **Flexible Scheduling** - Accommodate customer needs
4. **Professional Service** - Friendly and efficient
5. **Follow Through** - Ensure successful collection

### Order Management

1. **Regular Reviews** - Check aging orders weekly
2. **Escalate Promptly** - Don't let orders age excessively
3. **Document Issues** - Note any problems
4. **Update Contacts** - Keep customer info current
5. **Clean Up** - Archive old collected orders

## Troubleshooting

### Order Not Detected

If order should be counter collect but isn't showing:
1. Check carrier field in sales order
2. Verify keywords are present
3. Wait for next scan cycle (15 minutes)
4. Manually add if needed
5. Contact admin if persistent

### Reminder Not Sent

If reminder wasn't sent:
1. Check customer email address
2. Verify reminder schedule
3. Check email logs
4. Ensure order is active
5. Manually send if needed

### Scanner Not Working

If scanner won't read barcodes:
1. Check scanner connection
2. Verify barcode format
3. Try manual entry
4. Test with different barcode
5. Contact IT if issue persists

### Wrong Order Status

If order status is incorrect:
1. Verify actual status
2. Check collection date
3. Update manually if needed
4. Document discrepancy
5. Report to admin

## Reporting

### Available Reports

**Active Orders Report**:
- All orders awaiting collection
- Aging analysis
- Customer breakdown

**Collection Performance**:
- Average wait times
- Collection trends
- Peak periods

**Customer Analysis**:
- Frequent collectors
- Average wait by customer
- Communication effectiveness

**Escalation Report**:
- Orders requiring management review
- Aging trends
- Resolution tracking

### Exporting Data

Export options:
- **Excel** - Detailed spreadsheet
- **CSV** - Raw data
- **PDF** - Formatted report
- **Email** - Send to recipients

## Mobile Access

### Mobile-Friendly Scanner

The collection scanner works on:
- Tablets
- Smartphones
- Mobile barcode scanners
- Touch devices

### Mobile Features

- Large buttons for touch
- Camera barcode scanning
- Offline capability (planned)
- Quick entry mode

## Related Features

- [Order Management](order-management.md) - Sales order tracking
- [Customer Notifications](customer-notifications.md) - Email notifications
- [Label Printing](label-printing.md) - Print pickslip labels
- [Admin Settings](administration.md) - Configure reminders
