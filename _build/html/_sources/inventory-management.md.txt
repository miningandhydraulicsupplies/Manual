# Inventory Management

## Overview

The Inventory Management system provides tools for conducting stocktakes, managing inventory counts, and tracking inventory discrepancies. It integrates with MomentumPro ERP for real-time inventory verification.

## Stocktakes

### Creating a Stocktake

1. Navigate to **Stocktakes** from the Operations section
2. Click **Create Stocktake** button
3. Enter stocktake details:
   - **Description** - Purpose or location of stocktake
   - **Type** - Full, Partial, Cycle Count
4. Click **Create**
5. Stocktake is created with unique number (e.g., ST-20260305-A1B2C3D4)

### Stocktake Types

**Full Stocktake**:
- Complete inventory count
- All items in warehouse
- Typically annual or semi-annual

**Partial Stocktake**:
- Specific area or category
- Targeted inventory verification
- More frequent

**Cycle Count**:
- Rotating inventory counts
- High-value or fast-moving items
- Continuous process

### Stocktake Status

- **Planned** - Stocktake scheduled, items pre-loaded
- **In Progress** - Actively counting
- **Complete** - Counting finished
- **Finalized** - Approved and posted to ERP

## Adding Items to Stocktake

### Manual Item Entry

1. Open stocktake details
2. Click **Add Item** button
3. Enter part number
4. System looks up part details from MomentumPro
5. Enter counted quantity
6. Add notes if needed
7. Click **Save**

### Barcode Scanning

1. Open stocktake details
2. Focus on part number field
3. Scan barcode with scanner
4. System auto-populates part details
5. Enter counted quantity
6. Press Enter to save and continue

### Bulk Import

Import items from file:
1. Prepare CSV or Excel file with:
   - Part number
   - Counted quantity
   - Bin location (optional)
2. Click **Import Items**
3. Select file
4. Review import preview
5. Click **Confirm Import**

## Planned Stocktakes

### Creating Planned Stocktake

1. Navigate to **Stocktakes**
2. Click **Upload Planned Stocktake**
3. Upload PDF or Excel file with expected items
4. System extracts part numbers
5. Creates stocktake with pre-loaded items
6. Status set to "Planned"

### Benefits of Planned Stocktakes

- Pre-loaded expected items
- Compare expected vs actual
- Identify missing items
- Faster counting process
- Better accuracy

### Converting to In Progress

1. Open planned stocktake
2. Review pre-loaded items
3. Click **Start Counting**
4. Status changes to "In Progress"
5. Begin entering counted quantities

## Counting Process

### Best Practices

1. **Organize counting area** - Clear and accessible
2. **Use barcode scanners** - Faster and more accurate
3. **Count systematically** - Follow logical sequence
4. **Double-check high-value items** - Verify expensive items
5. **Document discrepancies** - Note any issues
6. **Take photos** - Document problem areas

### Recording Counts

For each item:
1. Locate physical item
2. Count quantity accurately
3. Scan or enter part number
4. Enter counted quantity
5. Note bin location
6. Add comments if needed
7. Save and move to next item

### Handling Discrepancies

If count doesn't match system:
1. Recount the item
2. Check for multiple locations
3. Verify part number is correct
4. Document reason for discrepancy
5. Flag for management review
6. Add detailed notes

## Stocktake Details View

### Item List

View all items in stocktake:
- Part number and description
- Expected quantity (if planned)
- Counted quantity
- Variance (difference)
- Bin location
- Notes
- Counted by and timestamp

### Summary Statistics

- **Total Items** - Number of items counted
- **Items with Variance** - Items with discrepancies
- **Total Variance Value** - Dollar value of variances
- **Completion Percentage** - Progress indicator

### Filtering and Sorting

Filter items by:
- Counted vs not counted
- Items with variance
- Specific bin location
- Part number range

Sort by:
- Part number
- Variance amount
- Counted date
- Bin location

## Variance Analysis

### Variance Types

**Positive Variance**:
- More stock than expected
- Potential data entry errors
- Unreported receipts
- Misplaced items found

**Negative Variance**:
- Less stock than expected
- Potential shrinkage
- Unreported usage
- Misplaced items

### Variance Reporting

Generate variance reports:
1. Open completed stocktake
2. Click **Variance Report**
3. Review all discrepancies
4. Export to Excel
5. Investigate significant variances

### Variance Approval

For items with variance:
1. Review variance reason
2. Verify count is accurate
3. Approve or reject variance
4. Add approval notes
5. Mark as reviewed

## Completing Stocktakes

### Finalizing Count

1. Ensure all items counted
2. Review variance report
3. Resolve any issues
4. Click **Complete Stocktake**
5. Status changes to "Complete"

### Posting to ERP

After completion:
1. Review final counts
2. Get management approval
3. Click **Post to MomentumPro**
4. System updates inventory levels
5. Status changes to "Finalized"
6. Audit trail created

### Stocktake Archive

Finalized stocktakes:
- Archived for reference
- Cannot be modified
- Available for reporting
- Retained per policy

## Real-Time Collaboration

### Multi-User Counting

Multiple users can count simultaneously:
- Real-time updates via SignalR
- See who is counting what
- Avoid duplicate counts
- Coordinate efficiently

### Live Progress Tracking

Monitor stocktake progress:
- Items counted vs remaining
- Users currently active
- Completion percentage
- Estimated time to complete

## Integration with MomentumPro

### Part Lookup

System automatically:
- Retrieves part descriptions
- Gets current stock levels
- Fetches bin locations
- Shows unit of measure
- Displays part images

### Stock Level Comparison

Compare counts to system:
- Expected quantity from ERP
- Counted quantity
- Variance calculation
- Percentage difference

### Inventory Adjustment

After posting:
- Inventory levels updated
- Transactions recorded
- Audit trail maintained
- Reports generated

## Reporting

### Available Reports

**Stocktake Summary**:
- Overview of stocktake
- Total items and values
- Variance summary
- Completion status

**Variance Report**:
- All items with discrepancies
- Variance amounts
- Percentage differences
- Investigation notes

**Bin Location Report**:
- Items by bin location
- Location accuracy
- Misplaced items

**Historical Comparison**:
- Compare multiple stocktakes
- Trend analysis
- Recurring issues

### Exporting Data

Export options:
- **Excel** - Detailed spreadsheet
- **CSV** - Raw data
- **PDF** - Formatted report

## Mobile Counting

### Mobile-Friendly Interface

The stocktake interface is optimized for:
- Tablets
- Mobile phones
- Barcode scanners
- Touch input

### Mobile Features

- Large input fields
- Quick entry mode
- Offline capability (planned)
- Camera for photos

## Best Practices

### Planning

1. **Schedule appropriately** - Avoid busy periods
2. **Communicate clearly** - Inform all stakeholders
3. **Prepare materials** - Scanners, tablets, printouts
4. **Assign areas** - Divide warehouse logically
5. **Set deadlines** - Establish completion timeline

### Execution

1. **Start early** - Allow adequate time
2. **Count systematically** - Follow planned sequence
3. **Use technology** - Scanners and tablets
4. **Double-check** - Verify high-value items
5. **Document issues** - Note problems immediately

### Follow-Up

1. **Review variances** - Investigate discrepancies
2. **Update procedures** - Improve based on findings
3. **Train staff** - Address knowledge gaps
4. **Adjust inventory** - Post corrections promptly
5. **Plan next stocktake** - Schedule regular counts

## Troubleshooting

### Part Not Found

If part number not found:
1. Verify part number is correct
2. Check for typos or extra characters
3. Try alternate part numbers
4. Check if part is obsolete
5. Contact admin to add part

### Cannot Save Count

If unable to save:
1. Check internet connection
2. Verify stocktake is not finalized
3. Ensure quantity is valid number
4. Try refreshing page
5. Contact admin if issue persists

### Variance Too Large

If variance seems incorrect:
1. Recount the item
2. Check for multiple locations
3. Verify unit of measure
4. Check recent transactions
5. Investigate with management

## Related Features

- [Label Printing](label-printing.md) - Print inventory labels
- [Order Board](order-board.md) - Track stock replenishment
- [Admin Settings](administration.md) - Configure stocktake settings
