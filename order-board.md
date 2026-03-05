# Order Board

## Overview

The Order Board is a collaborative procurement management tool that allows teams to track parts that need to be ordered across different divisions. It provides real-time updates, automatic part description lookup, pricing information, and purchase order generation capabilities.

## Divisions

The Order Board is organized into four divisions:

- **Hydraulics** - Hydraulic components and parts
- **Seals** - Sealing products and components
- **Filtration** - Filtration equipment and supplies
- **Projects** - Special project-related items

## Adding Items to the Order Board

### Basic Item Entry

1. Navigate to **Order Board** from the sidebar
2. Select the appropriate division tab
3. Click **Add Item** button
4. Fill in the required fields:
   - **Part Number** - The manufacturer or supplier part number
   - **Quantity** - Number of units needed
   - **Freight Type** - Select from dropdown (Standard, Express, etc.)
   - **Notes** - Optional notes about the item

### Advanced Options

- **Description** - Manually enter description (if left blank, system will auto-lookup)
- **Supplier** - Specify preferred supplier
- **Branches** - Check if item is for branch locations
- **ConsAir** - Check if item is for ConsAir division
- **Stock Item** - Check if this is a stock replenishment
- **Required Next Day** - Mark as urgent for next-day delivery
- **Letter of Conformity** - Check if certification is required

### Automatic Features

When you add an item:
- System automatically looks up part description from MomentumPro
- Base pricing is retrieved (where available)
- Product images are fetched for Hydraulics items
- Part weight is calculated for Hydraulics items
- Sales order associations are tracked for Seals items

## Managing Order Board Items

### Viewing Items

Each item displays:
- Part number and description
- Quantity and unit of measure
- Supplier information
- Base price (if available)
- Freight type
- Special flags (Branches, ConsAir, Stock, etc.)
- Added by and date
- Last updated information
- Order status

### Item Actions

**Edit Item**
- Click the edit icon on any item
- Modify quantity, notes, or other fields
- Changes are tracked in history

**Delete Item**
- Click the delete icon
- Confirm deletion
- Item is removed from active board

**Mark as Ordered**
- Click "Mark as Ordered" button
- Item moves to ordered status
- Timestamp and user are recorded

**Split Item**
- For items with multiple quantities
- Split into separate line items
- Useful for partial ordering

### Filtering and Search

- **Search** - Search by part number or description
- **Status Filter** - Show active, ordered, or all items
- **Supplier Filter** - Filter by specific supplier
- **Sort Options** - Sort by date, part number, or supplier

## Purchase Order Generation

### Creating Purchase Orders

1. Select items to order (checkbox selection)
2. Click **Generate PO** button
3. System groups items by supplier
4. Review generated purchase order
5. Export to Excel or XML format

### Export Options

**Excel Export**
- Formatted spreadsheet with all item details
- Includes pricing, quantities, and notes
- Ready for supplier submission

**XML Export**
- Automated format for supplier systems
- Includes all required fields
- Stored in S3 for supplier access

**CSV Download**
- Simple comma-separated format
- Includes all visible columns
- Useful for data analysis

## Supplier Integration

### Automatic Pricing

For supported suppliers, the system automatically:
- Fetches current pricing
- Displays price breaks
- Calculates extended totals
- Shows availability status

### Supported Suppliers

- **HSA** - Hydraulic Supplies Australia
- **Stauff** - Automated PO export to S3
- Additional suppliers configured in admin settings

### RFQ (Request for Quote) Management

For items without pricing:
1. Select items needing quotes
2. Click **Send RFQ** button
3. System generates email to supplier
4. Tracks RFQ history
5. Updates when quotes received

## Purchase Order Status Tracking

### Status Indicators

- **Pending** - Item added, not yet ordered
- **Ordered** - Purchase order sent to supplier
- **Received** - Item received (linked to GRN)
- **Cancelled** - Order cancelled

### PO Status Checking

The system automatically:
- Checks PO status with MomentumPro API
- Updates status in real-time
- Notifies users of status changes
- Links to GRN when items received

## Sales Order Integration (Seals Division)

For Seals division items:
- System checks for related sales orders
- Displays customer order numbers
- Shows urgency status
- Links to Order Monitoring for details

## History and Audit Trail

### Item History

View complete history of each item:
- When added and by whom
- All modifications made
- When ordered and by whom
- Export history
- Status changes

### Export History

Track all purchase order exports:
- Export date and time
- User who exported
- Items included
- File format
- Download link

## Best Practices

### Adding Items

1. **Use correct part numbers** - Verify part numbers before entry
2. **Add notes** - Include relevant information for purchasing
3. **Check for duplicates** - Search before adding new items
4. **Select correct division** - Ensure item is in appropriate division
5. **Mark urgency** - Use "Required Next Day" for urgent items

### Managing the Board

1. **Regular cleanup** - Mark items as ordered promptly
2. **Update quantities** - Adjust quantities as requirements change
3. **Consolidate orders** - Group items by supplier for efficiency
4. **Track status** - Monitor PO status for timely follow-up
5. **Review history** - Check history for recurring items

### Collaboration

1. **Use notes effectively** - Communicate requirements clearly
2. **Check before ordering** - Verify items haven't been ordered
3. **Update status** - Keep board current for team visibility
4. **Coordinate with team** - Discuss large orders before placing

## Troubleshooting

### Description Not Found

If automatic lookup fails:
- Manually enter description
- Verify part number is correct
- Check if part exists in MomentumPro
- Contact admin if persistent issues

### Pricing Not Available

If pricing doesn't display:
- Check supplier configuration
- Verify part number format
- Request manual quote
- Use RFQ feature

### Item Won't Delete

If you cannot delete an item:
- Check if item is already ordered
- Verify you have permissions
- Contact admin for assistance

## Keyboard Shortcuts

- **Ctrl + F** - Focus search box
- **Ctrl + N** - Add new item (when on Order Board)
- **Esc** - Close modal dialogs

## Related Features

- [Order Monitoring](order-management.md) - Track sales orders
- [GRN Monitoring](grn-monitoring.md) - Track goods receipts
- [Procurement](procurement.md) - Decision support tool
- [Admin Settings](administration.md) - Configure suppliers and settings
