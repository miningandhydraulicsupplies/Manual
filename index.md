# MHS Warehouse Management System (WMS)

## Overview

The MHS Warehouse Management System is a comprehensive web-based application designed to streamline warehouse operations, order management, production tracking, and inventory control for MHS (Momentum Hydraulics & Seals). Built with ASP.NET Core 8.0 and PostgreSQL, the system provides real-time monitoring, automated workflows, and integrated label printing capabilities.

## Quick Links

- **[Quick Start Guide](quick-start.md)** - Get started in minutes
- **[Table of Contents](TABLE_OF_CONTENTS.md)** - Complete navigation guide
- **[Complete Documentation Index](COMPLETE_DOCUMENTATION_INDEX.md)** - All documentation files

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
- **GRN Monitoring** - Goods receipt tracking with automatic backorder detection

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

**New User?** Start with the [Quick Start Guide](quick-start.md)

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

## Feature Documentation

### Operations

#### [Order Board](order-board.md)
Collaborative procurement management for multiple divisions (Hydraulics, Seals, Filtration, Projects). Add items, generate purchase orders, track supplier status, and manage procurement workflow.

#### [Order Management](order-management.md)
Real-time sales order monitoring with backorder tracking, urgent order flagging, and personal dashboards for sales representatives. Includes order alerts and watchlist features.

#### [Production Monitoring](production-monitoring.md)
Track production orders across categories (SEA, FIL, HYD, PRO). Monitor status, print production labels, and view TV display mode for production floor visibility.

#### [GRN Monitoring](grn-monitoring.md)
Goods receipt tracking with automatic backorder detection. Links GRNs to sales orders and notifies sales reps when backordered items arrive.

#### [Counter Collect](counter-collect.md)
Customer pickup order management with automatic detection, collection scanner, and reminder system. Tracks aging orders and escalates overdue collections.

#### [Customer Notifications](customer-notifications.md)
Send automated email notifications to customers about order status. Automatic email extraction from order comments and delivery tracking.

#### [Inventory Management](inventory-management.md)
Digital stocktake creation and management with barcode scanning, variance analysis, and mobile-friendly counting interface.

#### [Calibration Tracking](calibration-tracking.md)
Equipment calibration management with automated reminder system, certificate storage, and customer notification integration.

### Labels and Printing

#### [Label Printing](label-printing.md)
Comprehensive label printing system supporting:
- **Pickslip Labels** - Order picking labels
- **Inventory Labels** - Stock identification labels
- **Delivery Labels** - Shipping labels
- **Production Labels** - Production order labels with bag split feature

Includes printer configuration, print history, batch printing, and barcode generation.

### Analytics and Reporting

#### [KPI Tracking](kpi-tracking.md)
Performance tracking and analytics for invoices and purchase orders. Includes user performance trends, goal tracking, comparative analytics, and team rankings.

### Administration

#### [System Administration](administration.md)
Complete system administration guide covering:
- User management and permissions
- Printer configuration
- Background job monitoring
- System logs and diagnostics
- Customer database management
- API key management
- Queue monitoring
- Weekly report configuration

## Navigation

The sidebar navigation is organized into sections:

### Operations
- [Order Board](order-board.md)
- [Order Monitor](order-management.md)
- [Production](production-monitoring.md)
- [Counter Collect](counter-collect.md)
- [Customer Notifications](customer-notifications.md)
- Sales Order Check *(documentation pending)*
- [Stocktakes](inventory-management.md)
- Procurement *(documentation pending)*
- Letter of Conformity *(documentation pending)*
- [Calibration Tracking](calibration-tracking.md)
- Pickslip Lookup *(documentation pending)*
- Tube Fabrication *(documentation pending)*

### TV Displays
- Sales Orders TV - See [Order Management](order-management.md#tv-display-mode)
- Production Orders TV - See [Production Monitoring](production-monitoring.md#tv-display-mode)

### Labels
- [Pickslip Labels](label-printing.md#pickslip-labels)
- [Inventory Labels](label-printing.md#inventory-labels)
- [Delivery Labels](label-printing.md#delivery-labels)
- [Production Labels](label-printing.md#production-order-labels)

### My Work (Sales/Admin only)
- My Orders - See [Order Management](order-management.md#my-orders-sales-users)
- My Quotes *(documentation pending)*
- My Performance - See [KPI Tracking](kpi-tracking.md#user-trends)
- Watchlist - See [Order Management](order-management.md#order-watchlist)

### Analytics
- [KPI Tracking](kpi-tracking.md)
- Hiverr Monitor *(documentation pending)*
- Build Cost *(documentation pending)*

### Admin (Admin only)
- [Admin Dashboard](administration.md#admin-dashboard)
- [Manage Users](administration.md#user-management)
- [Permissions](administration.md#permission-management)
- [User Mapping](administration.md#user-mapping)
- [Printer Settings](administration.md#printer-configuration)
- [Background Jobs](administration.md#background-jobs)
- [System Logs](administration.md#system-logs)
- Email Monitoring - See [Administration](administration.md)
- Weekly Reports - See [Administration](administration.md#weekly-reports)
- [Customers](administration.md#customer-management)

## Additional Resources

### Documentation Files

- **[Quick Start Guide](quick-start.md)** - Get up and running quickly
- **[Table of Contents](TABLE_OF_CONTENTS.md)** - Complete navigation
- **[Screenshot Guide](screenshot-guide.md)** - Guide for adding screenshots
- **[Documentation Summary](DOCUMENTATION_SUMMARY.md)** - Documentation overview
- **[Complete Index](COMPLETE_DOCUMENTATION_INDEX.md)** - All files listed

### Technical Documentation

- **[README](../README.md)** - Installation and setup
- **API Documentation** - Available at `/swagger` when running
- **Configuration** - See [README](../README.md#configuration)

## Support

For technical support or questions:
- **Email**: warehouse@mhs.com.au
- **Internal IT Support**: Contact your system administrator
- **Documentation Issues**: Report via email with subject "WMS Documentation - [Topic]"

## Documentation Status

**Version**: 1.0.0
**Last Updated**: 2026-03-05
**Coverage**: ~70% of features documented
**Status**: Core features complete, additional features in progress

### Documented Features ✅
- Dashboard and navigation
- Order Board (all divisions)
- Order monitoring and management
- Production order tracking
- GRN monitoring
- Counter collect system
- Customer notifications
- Inventory/stocktake management
- Calibration tracking
- Label printing (all types)
- KPI tracking
- System administration

### Pending Documentation 📝
- Sales Order Check
- Procurement Decision Support
- Letter of Conformity
- Pickslip Lookup
- Tube Fabrication
- My Quotes
- Hiverr Email Monitor
- Build Cost Analysis

---

**Welcome to the MHS WMS Documentation!** Use the links above to navigate to specific features, or start with the [Quick Start Guide](quick-start.md) if you're new to the system.
