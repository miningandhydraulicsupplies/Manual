# Order Management

## Overview

The Order Management system provides real-time monitoring of sales orders from MomentumPro ERP. It automatically tracks order status, identifies backorders, flags urgent orders, and provides detailed line-item information.

## Order Monitoring Dashboard

### Accessing Order Monitor

Navigate to **Order Monitor** from the Operations section in the sidebar.

### Dashboard Metrics

The dashboard displays:
- **Total Active Orders** - All open sales orders
- **Urgent Orders** - Orders marked as urgent
- **Orders with Backorders** - Orders containing backordered items
- **New Orders Today** - Orders entered today
- **Average Order Age** - Average days since order entry

### Order List View

Each order shows:
- **Invoice Number** - Sales order number
- **Customer Name** - Customer account name
- **Status** - Current order status
- **Enter Date** - When order was created
- **Required Date** - Customer requested delivery date
- **Urgency Indicator** - Visual flag for urgent orders
- **Backorder Indicator** - Shows if order has backorders
- **Sales Rep** - Assigned sales representative

## Order Details

### Viewing Order Details

1. Click on any order in the list
2. Detailed view opens showing:
   - Complete order header information
   - Customer details and contact information
   - Line items with quantities and pricing
   - Backorder information
   - Order notes and comments
   - Status history

### Line Item Information

For each line item:
- Part number and description
- Quantity ordered
- Quantity shipped
- Quantity backordered
- Unit price
- Extended price
- Expected availability date (if backordered)

### Order Status Indicators

- **Open** - Order is active and being processed
- **Picking** - Order is being picked in warehouse
- **Packed** - Order is packed and ready to ship
- **Shipped** - Order has been dispatched
- **Invoiced** - Order has been invoiced
- **Finalised** - Order is complete

## Backorder Management

### Identifying Backorders

Orders with backorders are:
- Highlighted with a red indicator
- Shown in the "Orders with Backorders" filter
- Listed with backorder quantities per line item

### Backorder Information

For backordered items:
- Quantity on backorder
- Expected availability date
- Supplier information
- Purchase order status
- Alternative part suggestions

### Backorder Alerts

The system automatically:
- Monitors backorder status
- Checks for incoming GRNs
- Notifies when backorder items arrive
- Updates order status in real-time

## Urgent Orders

### Marking Orders as Urgent

Orders are marked urgent when:
- Required date is within 2 days
- Customer has requested expedited delivery
- Sales rep manually flags as urgent
- System detects critical status

### Urgent Order Handling

Urgent orders:
- Display with red "URGENT" badge
- Appear at top of order list
- Trigger notifications to warehouse
- Receive priority processing

## Order Filtering and Search

### Filter Options

- **Status** - Filter by order status
- **Date Range** - Show orders within date range
- **Sales Rep** - Filter by assigned sales rep
- **Customer** - Filter by customer name
- **Backorders Only** - Show only orders with backorders
- **Urgent Only** - Show only urgent orders

### Search Functionality

Search by:
- Invoice number
- Customer name
- Part number
- Purchase order number
- Sales order reference

## My Orders (Sales Users)

### Personal Order Dashboard

Sales users have access to "My Orders" showing:
- Orders assigned to them
- Personal performance metrics
- Order aging analysis
- Backorder summary
- Recent order activity

### My Orders Metrics

- **Total Open Orders** - Your active orders
- **Orders with Backorders** - Your orders with backorders
- **Urgent Orders** - Your urgent orders
- **Critical Orders** - Urgent orders with backorders
- **Total Backorder Quantity** - Sum of all backordered items
- **Most Recent Order** - Latest order details

### Order History

View historical orders:
- Completed orders
- Cancelled orders
- Order trends over time
- Customer order patterns

## Order Alerts

### Alert Configuration

Set up alerts for:
- Orders approaching required date
- New backorders detected
- Backorder items received
- Order status changes
- Customer-specific alerts

### Alert Preferences

Configure:
- Alert threshold (days before required date)
- Notification method (email, in-app)
- Alert frequency
- Snooze duration options
- Escalation rules

### Managing Alerts

- **View Active Alerts** - See all current alerts
- **Snooze Alerts** - Temporarily dismiss alerts
- **Dismiss Alerts** - Permanently dismiss alerts
- **Alert History** - View past alerts

## Order Notes

### Adding Notes

1. Open order details
2. Click **Add Note** button
3. Enter note text
4. Select note type (Internal, Customer, Warehouse)
5. Save note

### Note Types

- **Internal** - Visible to staff only
- **Customer** - Visible to customer
- **Warehouse** - Visible to warehouse staff
- **Purchasing** - Visible to purchasing team

### Note History

- All notes are timestamped
- User who added note is recorded
- Notes can be edited or deleted
- Full audit trail maintained

## Order Watchlist

### Adding to Watchlist

1. Open order details
2. Click **Add to Watchlist** button
3. Order is monitored for changes
4. Receive notifications on updates

### Watchlist Features

- Monitor specific orders closely
- Receive priority notifications
- Quick access from sidebar
- Custom alert settings per order

### Managing Watchlist

- View all watched orders
- Remove orders from watchlist
- Set custom alert thresholds
- Export watchlist data

## TV Display Mode

### Accessing TV Display

Navigate to **TV Displays > Sales Orders TV** from sidebar.

### TV Display Features

- Full-screen order monitoring
- Auto-refresh every 30 seconds
- Color-coded status indicators
- Urgent orders highlighted
- Optimized for large displays

### TV Display Configuration

- Select which orders to display
- Configure refresh interval
- Choose display columns
- Set color scheme

## Integration with Other Modules

### GRN Monitoring

- Links to goods receipt notes
- Shows when backorder items arrive
- Updates order status automatically
- Tracks partial receipts

### Order Board

- Links to procurement items
- Shows parts being ordered
- Tracks supplier status
- Coordinates purchasing

### Counter Collect

- Identifies customer pickup orders
- Tracks collection status
- Sends pickup notifications
- Manages collection reminders

## Reporting

### Available Reports

- **Order Aging Report** - Orders by age
- **Backorder Report** - All backordered items
- **Sales Rep Performance** - Orders by sales rep
- **Customer Order History** - Orders by customer
- **Urgent Orders Report** - All urgent orders

### Exporting Data

Export options:
- Excel spreadsheet
- CSV file
- PDF report
- Email report

## Best Practices

### Daily Monitoring

1. Review urgent orders first
2. Check backorder status
3. Follow up on aging orders
4. Update order notes
5. Communicate with customers

### Backorder Management

1. Monitor backorder alerts
2. Check supplier status
3. Communicate ETAs to customers
4. Consider alternatives
5. Update order priorities

### Customer Communication

1. Proactive status updates
2. Clear ETA communication
3. Document all interactions
4. Set realistic expectations
5. Follow up on commitments

## Troubleshooting

### Order Not Appearing

If an order doesn't appear:
- Check date filters
- Verify order status
- Ensure order is in MomentumPro
- Check user permissions
- Contact admin if issue persists

### Incorrect Status

If order status is incorrect:
- Refresh the page
- Check MomentumPro directly
- Wait for next sync cycle
- Report discrepancy to admin

### Missing Line Items

If line items are missing:
- Verify in MomentumPro
- Check if items were deleted
- Review order history
- Contact admin for investigation

## Related Features

- [Order Board](order-board.md) - Procurement management
- [GRN Monitoring](grn-monitoring.md) - Goods receipt tracking
- [Counter Collect](counter-collect.md) - Customer pickup management
- [My Orders](my-orders.md) - Personal order dashboard
