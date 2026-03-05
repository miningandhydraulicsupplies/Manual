# Production Order Monitoring

## Overview

The Production Order Monitoring system provides real-time tracking of production orders from MomentumPro ERP. It monitors order status, tracks completion, and provides visibility into the production workflow across different categories.

## Production Dashboard

### Accessing Production Monitor

Navigate to **Production** from the Operations section in the sidebar.

### Dashboard Metrics

The dashboard displays:
- **Total Orders** - All production orders in system
- **Open Orders** - Active production orders (Status: 1)
- **Closed Orders** - Completed production orders (Status: c)
- **Finalised Orders** - Orders marked as finalised
- **Today's Orders** - Orders created today

### Production Order List

Each order shows:
- **Order Number** - Production order identifier
- **Description** - Product or assembly description
- **Category** - Product category (SEA, FIL, HYD, PRO, etc.)
- **Status** - Current order status (Open/Closed)
- **Finalised** - Whether order is finalised
- **Created Date** - When order was created
- **Last Updated** - Most recent update timestamp

## Order Categories

### Category Types

**SEA (Seals)**:
- Seal kits and assemblies
- O-ring products
- Sealing solutions

**FIL (Filtration)**:
- Filter assemblies
- Filter elements
- Filtration systems

**HYD (Hydraulics)**:
- Hydraulic assemblies
- Hose assemblies
- Hydraulic components

**PRO (Projects)**:
- Custom projects
- Special assemblies
- One-off productions

**Other Categories**:
- MAT (Materials)
- CON (Consumables)
- Custom categories as configured

### Category Filtering

Filter production orders by category:
1. Select category from dropdown
2. View orders for that category only
3. Default view shows SEA category
4. Select "All" to view all categories

## Order Status

### Status Types

**Open (Status: 1)**:
- Order is active
- Production in progress
- Not yet completed

**Closed (Status: c)**:
- Production completed
- Order closed in system
- May not be finalised

**Finalised**:
- Order completely finished
- All paperwork complete
- Ready for archival

### Status Indicators

Visual indicators:
- **Green badge** - Open orders
- **Blue badge** - Closed orders
- **Purple badge** - Finalised orders
- **Bold text** - Orders updated today

## Order Details

### Viewing Order Details

1. Click on any order in the list
2. Detailed view opens showing:
   - Complete order information
   - Product specifications
   - Quantity details
   - Material requirements
   - Labor information
   - Cost breakdown
   - Status history
   - Related documents

### Order Information

**Header Information**:
- Order number
- Description
- Category
- Status
- Created date
- Required date
- Priority

**Production Details**:
- Quantity to produce
- Quantity completed
- Unit of measure
- Bill of materials
- Work instructions
- Quality requirements

**Tracking Information**:
- First seen in system
- Last updated timestamp
- Status change history
- User who created order

## Filtering and Search

### Filter Options

**By Status**:
- Open orders only
- Closed orders only
- Finalised orders only
- All orders

**By Category**:
- Select specific category
- View all categories
- Default to SEA

**By Date**:
- Today's orders
- This week
- This month
- Custom date range

**By Finalised Status**:
- Finalised only
- Not finalised only
- All orders

### Search Functionality

Search by:
- Order number
- Description
- Category
- Product code

### Sorting Options

Sort orders by:
- Created date (newest first)
- Order number
- Description
- Status (open first)
- Category

## Production Labels

### Printing Production Labels

1. From order list, click **Print Label** icon
2. Or open order details and click **Print Label**
3. Select printer from dropdown
4. Choose number of copies
5. Optional: Enable bag split for large quantities
6. Click **Print**

### Bag Split Feature

For large production runs:
1. Enable "Split into bags" option
2. Enter quantity per bag
3. System calculates number of bags
4. Each bag gets unique label
5. Labels show "Bag X of Y"

**Example**:
- Production order: 100 units
- Bag size: 25 units
- Result: 4 labels (Bag 1 of 4, Bag 2 of 4, etc.)

### Label Information

Production labels include:
- Production order number
- Product description
- Quantity
- Category
- Due date
- Barcode for scanning
- Bag information (if split)

## Finalising Orders

### Marking Orders as Finalised

1. Open order details
2. Click **Mark as Finalised** button
3. Confirm action
4. Order status updates to finalised
5. Order appears in finalised list

### Finalised Order Behavior

Finalised orders:
- Remain visible for current day
- Archived after midnight
- Can be searched in history
- Included in reports
- Cannot be un-finalised (contact admin)

## TV Display Mode

### Accessing TV Display

Navigate to **TV Displays > Production Orders TV** from sidebar.

### TV Display Features

- **Full-screen view** - Optimized for large displays
- **Auto-refresh** - Updates every 30 seconds
- **Color-coded status** - Easy visual identification
- **Category filtering** - Show specific categories
- **Minimal interface** - Focus on essential information

### TV Display Configuration

Configure display:
- Select categories to show
- Set refresh interval
- Choose sort order
- Enable/disable finalised orders
- Adjust font size

### Use Cases

- **Production floor displays** - Show current orders
- **Management overview** - Monitor production status
- **Team coordination** - Shared visibility
- **Status boards** - Real-time updates

## Production Workflow

### Typical Order Lifecycle

1. **Order Created** - New production order entered
2. **Materials Allocated** - Materials assigned to order
3. **Production Started** - Work begins
4. **In Progress** - Order status remains open
5. **Production Completed** - Order closed
6. **Quality Check** - Verification performed
7. **Order Finalised** - All steps complete

### Status Transitions

- **New → Open** - Order activated
- **Open → Closed** - Production completed
- **Closed → Finalised** - All paperwork complete

## Integration with Other Systems

### MomentumPro ERP

- Syncs production orders automatically
- Updates status in real-time
- Retrieves order details
- Tracks material usage
- Updates inventory

### Label Printing

- Generates production labels
- Prints to configured printers
- Tracks print history
- Supports batch printing

### Inventory System

- Links to material requirements
- Tracks component usage
- Updates stock levels
- Manages work-in-progress

## Reporting

### Available Reports

**Production Summary**:
- Orders by category
- Open vs closed orders
- Production volume
- Completion rates

**Category Performance**:
- Orders per category
- Average completion time
- Efficiency metrics
- Trend analysis

**Daily Production Report**:
- Orders created today
- Orders completed today
- Orders finalised today
- Outstanding orders

### Exporting Data

Export options:
- **Excel** - Formatted spreadsheet
- **CSV** - Raw data
- **PDF** - Formatted report

## Best Practices

### Daily Monitoring

1. **Review open orders** - Check status of active orders
2. **Update completed orders** - Close finished orders promptly
3. **Finalise orders** - Complete paperwork same day
4. **Print labels** - Generate labels as needed
5. **Check priorities** - Focus on urgent orders

### Order Management

1. **Keep status current** - Update status regularly
2. **Document issues** - Note any problems
3. **Communicate delays** - Alert team to delays
4. **Track materials** - Ensure materials available
5. **Quality checks** - Verify before closing

### Label Printing

1. **Print at start** - Generate labels when starting production
2. **Use bag splits** - For large quantities
3. **Verify details** - Check label accuracy
4. **Reprint if needed** - Don't use damaged labels
5. **Track prints** - Monitor label usage

## Troubleshooting

### Order Not Appearing

If order doesn't appear:
1. Check category filter
2. Verify status filter
3. Check date range
4. Ensure order exists in MomentumPro
5. Wait for next sync cycle (30 minutes)
6. Contact admin if issue persists

### Cannot Close Order

If unable to close order:
1. Verify order is open
2. Check user permissions
3. Ensure all requirements met
4. Try refreshing page
5. Contact admin for assistance

### Label Won't Print

If label doesn't print:
1. Check printer status
2. Verify printer selection
3. Check print queue
4. Ensure printer has supplies
5. Try different printer
6. See [Label Printing](label-printing.md) troubleshooting

### Incorrect Order Details

If order details are wrong:
1. Verify in MomentumPro
2. Wait for next sync
3. Refresh page
4. Report discrepancy to admin
5. Do not modify in WMS (read-only)

## Keyboard Shortcuts

- **Ctrl + F** - Focus search box
- **F5** - Refresh order list
- **Esc** - Close order details

## Related Features

- [Label Printing](label-printing.md) - Production label printing
- [Order Monitoring](order-management.md) - Sales order tracking
- [Inventory Management](inventory-management.md) - Material tracking
- [KPI Tracking](kpi-tracking.md) - Production metrics
