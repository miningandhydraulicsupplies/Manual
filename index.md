# MHS Warehouse Management System (WMS)

## Overview

The MHS Warehouse Management System is a comprehensive web-based application designed to streamline warehouse operations, order management, production tracking, and inventory control for MHS (Momentum Hydraulics & Seals). Built with ASP.NET Core 8.0 and PostgreSQL, the system provides real-time monitoring, automated workflows, and integrated label printing capabilities.

## Key Features

- **Real-time Order Monitoring** - Track sales orders, production orders, and GRN (Goods Receipt Notes)
- **Order Board Management** - Collaborative procurement board for multiple divisions
- **Label Printing** - Automated label generation for pickslips, inventory, delivery, and production
- **Calibration Tracking** - Equipment calibration management with automated reminders
- **KPI Analytics** - Performance tracking and reporting dashboards
- **Customer Notifications** - Automated email notifications for order status
- **Stocktake Management** - Digital stocktake creation and tracking
- **Production Order Monitoring** - Real-time production order status tracking
- **Counter Collect Management** - Track customer pickup orders with automated reminders
- **Tube Fabrication Calculator** - Quote generation for tube fabrication projects

## System Architecture

### Technology Stack

- **Backend**: ASP.NET Core 8.0 (C#)
- **Database**: PostgreSQL
- **Caching**: Redis
- **Real-time Communication**: SignalR
- **Authentication**: ASP.NET Core Identity
- **API Documentation**: Swagger/OpenAPI
- **Logging**: Serilog

### Integration Points

- **MomentumPro API** - ERP system integration for orders, quotes, and inventory
- **SimpleInOut** - Employee attendance tracking integration
- **Hiverr** - Email monitoring and customer service integration
- **AWS S3** - Document storage for purchase orders and certificates
- **OpenAI** - AI-powered quote analysis and extraction
- **SMTP2Go** - Email delivery service

## User Roles

The system supports role-based access control with the following roles:

- **Admin** - Full system access including user management and configuration
- **Sales** - Access to order management, quotes, and customer-facing features
- **Warehouse** - Access to inventory, stocktakes, and label printing
- **Production** - Access to production order monitoring and labels
- **Viewer** - Read-only access to dashboards and reports

## Getting Started

### Accessing the System

1. Navigate to the application URL (typically `https://warehouse.mhs.com.au`)
2. Log in with your credentials
3. You'll be directed to the Dashboard showing system overview

### Dashboard Overview

The main dashboard provides:

- **Daily Statistics** - Today's label printing activity
- **System Status** - Health check of connected systems
- **Recent Activity** - Latest print jobs and operations
- **Production Overview** - Open and closed production orders
- **Sales Order Summary** - Active orders and backorders
- **Counter Collect Status** - Pending customer pickups
- **GRN Backorders** - Items awaiting receipt

For Sales and Admin users, additional personal statistics are displayed:
- My Orders summary
- My Quotes summary
- Performance trends
- Active goals

## Navigation

The sidebar navigation is organized into sections:

### Operations
- Order Board
- Order Monitor
- Production
- Counter Collect
- Customer Notifications
- Sales Order Check
- Stocktakes
- Procurement
- Letter of Conformity
- Calibration Tracking
- Pickslip Lookup
- Tube Fabrication

### TV Displays
- Sales Orders TV
- Production Orders TV

### Labels
- Pickslip Labels
- Inventory Labels
- Delivery Labels
- Production Labels

### My Work (Sales/Admin only)
- My Orders
- My Quotes
- My Performance
- Watchlist

### Analytics
- KPI Tracking
- Hiverr Monitor
- Build Cost

### Admin (Admin only)
- Admin Dashboard
- Manage Users
- Permissions
- User Mapping
- Printer Settings
- Background Jobs
- System Logs
- Email Monitoring
- Weekly Reports
- Customers

## Next Steps

- [Order Management](order-management.md) - Learn about order monitoring and management
- [Order Board](order-board.md) - Collaborative procurement board usage
- [Label Printing](label-printing.md) - Print labels for various purposes
- [Calibration Tracking](calibration-tracking.md) - Manage equipment calibration
- [Production Monitoring](production-monitoring.md) - Track production orders
- [Inventory Management](inventory-management.md) - Stocktakes and inventory control
- [Administration](administration.md) - System configuration and user management

## Support

For technical support or questions:
- Email: warehouse@mhs.com.au
- Internal IT Support: Contact your system administrator
