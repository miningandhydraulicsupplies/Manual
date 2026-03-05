# Customer Notifications

## Overview

The Customer Notifications system allows you to send automated email notifications to customers about their orders. It can extract customer email addresses from order comments and send professional notifications with order details.

## Sending Notifications

### Accessing Notification Page

Navigate to **Operations > Customer Notifications** from the sidebar.

### Notification Process

1. **Enter Invoice Number**
   - Type or scan pickslip/invoice number
   - Press Enter or click **Lookup**

2. **System Retrieves Email**
   - Automatically extracts email from order comments
   - Displays customer email if found
   - Shows error if no email found

3. **Review and Send**
   - Verify email address is correct
   - Add custom message (optional)
   - Click **Send Notification**

4. **Confirmation**
   - Success message displayed
   - Email sent to customer
   - Notification logged in history

### Email Extraction

The system automatically:
- Scans order comments for email addresses
- Validates email format
- Displays found email
- Allows manual override if needed

### Manual Email Entry

If no email found automatically:
1. Enter customer email manually
2. Verify email is correct
3. Send notification

## Notification Content

### Standard Email Template

Notifications include:
- **Subject**: Order Ready for Collection/Dispatch
- **Order Number**: Invoice/pickslip number
- **Customer Name**: From order details
- **Order Details**: Items and quantities
- **Collection/Delivery Info**: Instructions
- **Contact Information**: Warehouse contact details
- **Company Branding**: MHS logo and styling

### Customization

Customize notifications:
- Add personal message
- Include special instructions
- Attach documents (planned)
- Select template (planned)

## Notification History

### Viewing History

Navigate to **Notification > History** to see:
- All sent notifications
- Date and time sent
- Invoice numbers
- Customer emails
- Delivery status
- User who sent

### History Filters

Filter by:
- **Date Range** - Specific period
- **Customer** - Specific customer email
- **User** - Who sent notification
- **Status** - Delivered, Failed, Pending

### History Details

For each notification:
- Invoice number
- Customer email
- Sent timestamp
- Delivery status
- Email content
- User who sent
- Any errors

## Recent Notifications

### Dashboard Widget

The dashboard shows:
- Last 10 notifications sent
- Quick status overview
- Recent activity
- Failed notifications

### Quick Actions

From recent notifications:
- Resend notification
- View full details
- Copy email address
- View order details

## Automatic Notifications

### Configured Triggers

System can automatically send notifications for:
- Order ready for collection
- Order dispatched
- Backorder items arrived
- Order status changes
- Custom triggers (admin configured)

### Notification Preferences

Configure per customer:
- Enable/disable automatic notifications
- Preferred notification types
- Email addresses
- Notification frequency

## Email Delivery

### Delivery Status

Track email delivery:
- **Sent** - Email sent to mail server
- **Delivered** - Confirmed delivered
- **Failed** - Delivery failed
- **Bounced** - Email address invalid
- **Pending** - Awaiting delivery

### Failed Notifications

If notification fails:
1. Check email address is valid
2. Verify email server is working
3. Retry sending
4. Contact customer by phone
5. Update email address if incorrect

### Bounce Handling

For bounced emails:
- System logs bounce reason
- Marks email as invalid
- Alerts user to update email
- Prevents future sends to invalid address

## Integration

### Order System

- Links to sales orders
- Retrieves order details
- Shows order status
- Tracks order notes

### Email Service

- Uses SMTP2Go for delivery
- Professional email formatting
- Delivery tracking
- Bounce handling

### Customer Database

- Stores customer emails
- Tracks notification preferences
- Updates contact information
- Manages opt-outs

## Best Practices

### Before Sending

1. **Verify Email** - Confirm email is correct
2. **Check Order Status** - Ensure order is ready
3. **Review Content** - Check notification message
4. **Test First** - Send test to yourself first
5. **Document** - Note notification in order

### Email Etiquette

1. **Professional Tone** - Use business language
2. **Clear Subject** - Descriptive subject line
3. **Complete Information** - Include all details
4. **Contact Info** - Provide contact details
5. **Proofread** - Check for errors

### Customer Service

1. **Timely Notifications** - Send promptly
2. **Accurate Information** - Verify details
3. **Follow Up** - Confirm customer received
4. **Be Responsive** - Reply to customer questions
5. **Document Issues** - Note any problems

## Troubleshooting

### Email Not Found

If system can't find email:
1. Check order comments manually
2. Look in customer database
3. Contact customer for email
4. Enter email manually
5. Update order comments for future

### Notification Not Sent

If notification fails to send:
1. Check internet connection
2. Verify email address format
3. Check email service status
4. Try resending
5. Contact admin if persistent

### Customer Didn't Receive

If customer says they didn't receive:
1. Check spam/junk folder
2. Verify email address
3. Check delivery status
4. Resend notification
5. Try alternate email address

### Wrong Email Sent

If wrong email was sent:
1. Send correction immediately
2. Apologize for error
3. Send to correct address
4. Document incident
5. Update email address

## Reporting

### Available Reports

**Notification Summary**:
- Total notifications sent
- Delivery success rate
- Failed notifications
- Customer engagement

**Customer Communication**:
- Notifications per customer
- Response rates
- Preferred contact methods
- Opt-out tracking

### Exporting Data

Export options:
- **Excel** - Detailed spreadsheet
- **CSV** - Raw data
- **PDF** - Formatted report

## Related Features

- [Order Management](order-management.md) - Sales order tracking
- [Counter Collect](counter-collect.md) - Customer pickup management
- [Customer Management](administration.md#customer-management) - Customer database
- [Admin Settings](administration.md) - Configure email settings
