# GRN Monitoring

## Overview

The GRN (Goods Receipt Note) Monitoring system tracks incoming goods receipts from suppliers and automatically identifies backorder fulfillment. It links GRNs to sales orders with backorders and notifies relevant staff when backordered items arrive.

## GRN Dashboard

### Accessing GRN Monitor

Navigate to **Operations > GRN Monitoring** (available via Order Board or direct link).

### Dashboard Metrics

The dashboard displays:
- **Total GRNs Today** - Goods receipts entered today
- **GRNs with Backorders** - GRNs containing backordered items
- **Active Backorder Associations** - Items linked to sales orders
- **Total Backorder Value** - Dollar value of backorders fulfilled

### GRN List View

Each GRN shows:
- **GRN Number** - Goods receipt reference
- **Supplier Name** - Supplier who sent goods
- **Status** - Current GRN status
- **Total Amount** - Value of receipt
- **Invoice Reference** - Supplier invoice number
- **Receipt Date** - When goods were received
- **Backorder Indicator** - Shows if contains backorder items
- **Customer Invoices** - Related sales orders

## Automatic Backorder Detection

### How It Works

The system automatically:
1. Monitors new GRNs every 30 minutes
2. Checks GRN line items against active backorders
3. Matches part numbers
4. Creates backorder associations
5. Sends notifications to sales reps

### Matching Criteria

Items are matched when:
- Part number matches exactly
- Sales order has backorder for that part
- GRN quantity can fulfill backorder
- Sales order is still open

### Notification Process

When backorder items arrive:
1. System creates association
2. Email sent to sales representative
3. Notification appears in dashboard
4. Order status updated
5. Customer can be notified

## GRN Details

### Viewing GRN Details

Click on any GRN to see:
- Complete GRN header information
- Supplier details
- Line items with quantities
- Backorder associations
- Related sales orders
- Customer invoice numbers
- Status history

### Line Item Information

For each line item:
- Part number and description
- Quantity received
- Unit price
- Extended price
- Backorder associations (if any)
- Sales order links

### Backorder Associations

View which sales orders are fulfilled:
- Sales order number
- Customer name
- Part number
- Quantity on backorder
- Quantity fulfilled from this GRN
- Sales representative
- Order status

## Managing GRNs

### GRN Status

**Status Types**:
- **Open** - GRN entered, not finalized
- **Finalized** - GRN completed and posted
- **Cancelled** - GRN cancelled

### Manual Backorder Association

If automatic detection missed an item:
1. Open GRN details
2. Click **Add Backorder Association**
3. Select sales order
4. Select part number
5. Enter quantity
6. Save association

### Removing Associations

If association is incorrect:
1. Open GRN details
2. Find association
3. Click **Remove**
4. Confirm removal

### Adding Notes

Document GRN information:
1. Open GRN details
2. Click **Add Note**
3. Enter note text
4. Save

## Filtering and Search

### Filter Options

Filter GRNs by:
- **Status** - Open, Finalized, Cancelled
- **Date Range** - Specific period
- **Supplier** - Specific supplier
- **Has Backorders** - Only GRNs with backorders
- **Today Only** - Today's GRNs

### Search Functionality

Search by:
- GRN number
- Supplier name
- Invoice reference
- Part number
- Sales order number

## Customer Invoice Linking

### Automatic Linking

System automatically:
- Identifies related sales orders
- Retrieves customer invoice numbers
- Links GRN to customer orders
- Shows order status

### Customer Invoice Display

For each GRN, see:
- List of customer invoice numbers
- Order status summary
- Urgent order indicators
- Sales representative

### Benefits

- Quick visibility of which customers are affected
- Prioritize urgent orders
- Coordinate with sales team
- Improve customer communication

## Backorder Notifications

### Email Notifications

Automatic emails sent to:
- Sales representative assigned to order
- BCC to warehouse team
- Customer (if configured)

### Notification Content

Emails include:
- GRN number and date
- Part numbers received
- Quantities available
- Sales order numbers
- Customer names
- Next steps

### Notification History

Track all sent notifications:
- Date and time sent
- Recipients
- GRN and order details
- Delivery status

## Integration

### Sales Order System

- Links to Order Monitoring
- Updates backorder status
- Shows order details
- Tracks order notes

### Order Board

- Updates PO status
- Shows items received
- Links to procurement
- Tracks supplier performance

### Inventory System

- Updates stock levels
- Records receipts
- Tracks locations
- Manages allocations

## Reporting

### Available Reports

**GRN Summary Report**:
- All GRNs by period
- Supplier breakdown
- Value analysis

**Backorder Fulfillment Report**:
- Items received for backorders
- Fulfillment rates
- Time to fulfill
- Customer impact

**Supplier Performance**:
- On-time delivery
- Quality issues
- Backorder resolution
- Lead times

### Exporting Data

Export options:
- **Excel** - Detailed spreadsheet
- **CSV** - Raw data
- **PDF** - Formatted report

## Best Practices

### Daily Monitoring

1. **Check New GRNs** - Review overnight receipts
2. **Verify Associations** - Confirm backorder matches
3. **Notify Customers** - Inform of item availability
4. **Update Orders** - Coordinate with sales team
5. **Document Issues** - Note any problems

### Backorder Management

1. **Prompt Notification** - Alert sales reps immediately
2. **Verify Quantities** - Confirm sufficient stock
3. **Coordinate Shipping** - Arrange customer delivery
4. **Update Status** - Keep order status current
5. **Follow Through** - Ensure customer receives goods

### Data Quality

1. **Verify Part Numbers** - Ensure accurate matching
2. **Check Quantities** - Confirm receipt quantities
3. **Update Associations** - Correct any errors
4. **Document Discrepancies** - Note any issues
5. **Regular Audits** - Review associations periodically

## Troubleshooting

### GRN Not Appearing

If GRN doesn't appear:
1. Check date filter
2. Verify GRN is in MomentumPro
3. Wait for next sync (30 minutes)
4. Check status filter
5. Contact admin if issue persists

### Backorder Not Detected

If backorder item not associated:
1. Verify part number matches exactly
2. Check sales order has backorder
3. Confirm order is still open
4. Manually create association
5. Report to admin for investigation

### Notification Not Sent

If notification wasn't sent:
1. Check sales rep email address
2. Verify association was created
3. Check email logs
4. Manually send if needed
5. Contact admin if persistent

### Incorrect Association

If association is wrong:
1. Remove incorrect association
2. Verify correct sales order
3. Create new association
4. Document reason for change
5. Notify affected parties

## Related Features

- [Order Management](order-management.md) - Sales order tracking
- [Order Board](order-board.md) - Purchase order management
- [Customer Notifications](customer-notifications.md) - Email notifications
- [Admin Settings](administration.md) - Configure GRN monitoring
