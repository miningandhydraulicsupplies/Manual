# Label Printing

## Overview

The Label Printing system provides automated label generation for various warehouse operations including pickslips, inventory, delivery, and production orders. Labels are generated in ZPL (Zebra Programming Language) format and sent directly to network printers.

## Label Types

### Pickslip Labels

**Purpose**: Identify items to be picked for customer orders

**Information Included**:
- Pickslip number
- Customer name
- Part numbers and descriptions
- Quantities to pick
- Bin locations
- Order priority

**How to Print**:
1. Navigate to **Labels > Pickslip**
2. Enter pickslip number
3. Select printer
4. Optional: Print delivery label simultaneously
5. Optional: Print component labels
6. Click **Print**

### Inventory Labels

**Purpose**: Label inventory items for storage and identification

**Information Included**:
- Part number
- Description
- Quantity
- Bin location
- Barcode
- Date printed

**How to Print**:
1. Navigate to **Labels > Inventory**
2. Enter part number
3. Enter quantity
4. Enter bin location (optional)
5. Select printer
6. Click **Print**

### Delivery Labels

**Purpose**: Shipping labels for customer deliveries

**Information Included**:
- Customer name and address
- Delivery instructions
- Order number
- Number of packages
- Barcode

**How to Print**:
1. Navigate to **Labels > Delivery**
2. Enter pickslip or order number
3. System retrieves customer details
4. Select printer
5. Click **Print**

### Production Order Labels

**Purpose**: Identify production orders and work instructions

**Information Included**:
- Production order number
- Product description
- Quantity to produce
- Category (SEA, FIL, HYD, etc.)
- Due date
- Barcode

**How to Print**:
1. Navigate to **Labels > Production**
2. Enter production order number
3. System retrieves order details
4. Select printer
5. Optional: Print multiple copies
6. Optional: Split into bag labels
7. Click **Print**

**Bag Split Feature**:
- For large production runs
- Split into multiple bags
- Each bag gets unique label
- Tracks bag number (e.g., "Bag 1 of 5")

## Printer Configuration

### Available Printers

The system supports multiple printer types:

**Zebra Printers**:
- MHSZT411 (Main warehouse printer)
- Delivery Label Printer
- Network-connected via IP

**Complypro Printers**:
- BP530_FilterShield
- Used for specialized labels
- Template-based printing

### Printer Selection

When printing labels:
1. Select from dropdown of configured printers
2. System remembers last used printer
3. Different label types may have default printers
4. Admin can configure printer assignments

### Printer Status

Check printer status:
- Green indicator: Printer online and ready
- Yellow indicator: Printer busy
- Red indicator: Printer offline or error
- View printer queue in **Print Queue** page

## Print History

### Viewing Print History

Navigate to **Dashboard** to see recent print activity.

**Recently Printed Labels** section shows:
- Label type
- Timestamp
- User who printed
- Printer used
- Item details

### Print History by Type

Each label type maintains separate history:
- **Pickslip History** - Last 50 pickslip labels
- **Inventory History** - Last 50 inventory labels
- **Production History** - Last 50 production labels
- **Material History** - Last 50 material labels

### Searching Print History

Search capabilities:
- Filter by date range
- Filter by user
- Filter by printer
- Filter by label type
- Search by part number or order number

## Batch Printing

### Pickslip Batch Printing

Print multiple pickslips at once:
1. Navigate to **Pickslip > Print Batch**
2. Enter pickslip numbers (comma-separated or line-by-line)
3. Select printer
4. Choose options:
   - Include delivery labels
   - Include component labels
5. Click **Print Batch**
6. System queues all labels
7. View batch progress

### Production Order Batch Printing

Print multiple production orders:
1. Navigate to **Production Order Monitoring**
2. Select orders to print (checkboxes)
3. Click **Print Selected**
4. Choose printer
5. Confirm batch print

## Label Templates

### Standard Templates

The system includes pre-configured templates:
- **Pickslip Template** - Standard pickslip format
- **Inventory Template** - Inventory label with barcode
- **Delivery Template** - Shipping label format
- **Production Template** - Production order format

### Custom Templates

Admin users can:
- Create custom label templates
- Modify existing templates
- Set template defaults
- Assign templates to divisions

### Template Variables

Templates support dynamic variables:
- `{PartNumber}` - Part number
- `{Description}` - Item description
- `{Quantity}` - Quantity
- `{Date}` - Current date
- `{OrderNumber}` - Order number
- `{CustomerName}` - Customer name
- `{Barcode}` - Generated barcode

## Barcode Generation

### Barcode Types Supported

- **Code 128** - Default for most labels
- **Code 39** - Alternative format
- **QR Code** - For complex data
- **EAN-13** - For retail products

### Barcode Content

Barcodes typically encode:
- Part numbers
- Order numbers
- Serial numbers
- Bin locations

### Scanning Barcodes

Barcodes can be scanned for:
- Inventory lookup
- Order verification
- Stocktake counting
- Counter collect pickup

## Print Queue Management

### Viewing Print Queue

Navigate to **Home > Print Queue** to see:
- Queued print jobs
- Currently printing jobs
- Completed jobs
- Failed jobs

### Queue Status

Each job shows:
- Job ID
- Label type
- Printer name
- Status (Pending, Printing, Complete, Failed)
- Timestamp
- User who submitted

### Managing Queue

Actions available:
- **Retry Failed Jobs** - Resubmit failed prints
- **Cancel Pending Jobs** - Remove from queue
- **View Job Details** - See full job information
- **Clear Completed** - Remove completed jobs from view

## Development Labels

### Development Pickslip Labels

For development/testing purposes:
- Separate tracking from production labels
- Used in development environment
- Same format as production labels
- Tracked separately in history

### Development Inventory Labels

Test inventory label printing:
- Validate label format
- Test printer connectivity
- Verify barcode scanning
- Train new users

## Troubleshooting

### Label Not Printing

If label doesn't print:
1. Check printer status (online/offline)
2. Verify printer IP address is reachable
3. Check print queue for errors
4. Ensure printer has paper and ribbon
5. Try different printer
6. Contact IT if issue persists

### Incorrect Label Format

If label format is wrong:
1. Verify correct template is selected
2. Check printer configuration
3. Ensure printer firmware is updated
4. Review template settings
5. Contact admin for template issues

### Barcode Not Scanning

If barcode won't scan:
1. Check barcode print quality
2. Verify scanner is configured correctly
3. Try different scanner
4. Ensure barcode type matches scanner
5. Reprint label if necessary

### Print Queue Stuck

If print queue is stuck:
1. Check printer connectivity
2. Clear completed jobs
3. Retry failed jobs
4. Restart printer if necessary
5. Contact admin if queue remains stuck

## Best Practices

### Label Printing

1. **Verify before printing** - Check details are correct
2. **Use correct printer** - Select appropriate printer for label type
3. **Print test labels** - Test new templates before production use
4. **Monitor print queue** - Check for failed jobs regularly
5. **Report issues promptly** - Alert admin to printer problems

### Label Quality

1. **Check printer supplies** - Ensure adequate paper and ribbon
2. **Clean printer regularly** - Maintain print quality
3. **Verify barcode quality** - Test scannability
4. **Use correct label stock** - Use recommended label materials
5. **Store labels properly** - Protect from moisture and heat

### Batch Printing

1. **Group similar items** - Batch similar label types
2. **Verify quantities** - Check batch size before printing
3. **Monitor progress** - Watch for errors during batch
4. **Handle failures** - Reprint failed labels individually
5. **Document batches** - Note batch details for tracking

## Keyboard Shortcuts

- **Ctrl + P** - Quick print (when on label page)
- **Ctrl + Enter** - Submit print form
- **Esc** - Cancel print dialog

## Related Features

- [Pickslip Lookup](pickslip-lookup.md) - View pickslip details
- [Production Monitoring](production-monitoring.md) - Production order tracking
- [Inventory Management](inventory-management.md) - Inventory operations
- [Admin Settings](administration.md) - Printer configuration
