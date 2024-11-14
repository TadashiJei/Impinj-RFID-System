# RFID Integration System for HireTrack NX
## Powered by Impinj R700 Series RAIN RFID Readers

![Version](https://img.shields.io/badge/version-1.0.0-blue.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)

## Overview
The RFID Integration System is a cloud-based SaaS solution designed to seamlessly integrate Impinj R700 Series RAIN RFID readers with HireTrack NX software. This system enables efficient asset tracking, inventory management, and automated data collection for entertainment and event equipment rental operations.

## Purpose
To bridge the gap between RFID hardware capabilities and HireTrack NX software, providing real-time asset tracking and automated data collection while maintaining compatibility with existing workflows.

## Scope
- Integration with Impinj R700 Series RAIN RFID Readers
- Cloud-based data processing and storage
- CSV export functionality for HireTrack NX compatibility
- Real-time asset tracking and management
- Multi-location support
- User role management
- Automated data collection and processing

## Goals
1. Streamline asset tracking and inventory management
2. Reduce manual data entry and human error
3. Improve operational efficiency
4. Enable real-time asset visibility
5. Facilitate seamless data integration with HireTrack NX
6. Provide accurate reporting and analytics

## System Architecture

### Backend Stack
- Node.js
- Express.js
- MongoDB
- AWS S3 (file storage)
- Socket.IO (real-time communications)

### Frontend Stack
- React.js
- Material-UI
- Redux
- Chart.js

## Core Modules

### 1. RFID Reader Management
- Reader configuration and setup
- Real-time status monitoring
- Firmware updates
- Performance analytics
- Multi-reader support

### 2. Settings Module
- **FTP Configuration**
  - Server settings
  - Credentials management
  - Connection testing
  - Automated sync scheduling
  
- **File Path Configuration**
  - CSV export locations
  - Backup directories
  - Log file paths
  
- **User Management**
  - Role-based access control
  - Employee profiles
  - Activity logging
  - Permissions management

### 3. Preparation Module
Features:
- New preparation entry
- Bulk item scanning
- Edit existing entries
- Delete entries
- Export to CSV
- Advanced search
- Real-time status updates
- Photo documentation
- Notes and comments

### 4. Dispatch Module
Features:
- Create dispatch orders
- Scan items for dispatch
- Verification checks
- Documentation
- Export capabilities
- Search functionality
- Status tracking
- Chain of custody

### 5. Return Module
Features:
- Process returns
- Condition assessment
- Damage documentation
- Missing item tracking
- Export reports
- Search capabilities
- Integration with billing
- Automated notifications

### 6. Check-In Module
Features:
- Rapid item scanning
- Condition verification
- Location assignment
- Status updates
- Export functionality
- Search capabilities
- Maintenance flagging
- Integration with inventory

### Additional Features

#### Reporting & Analytics
- Custom report generation
- Data visualization
- Performance metrics
- Inventory analytics
- Usage patterns
- Loss prevention statistics

#### Integration Services
- HireTrack NX compatibility layer
- CSV file generation
- Data mapping
- Error handling
- Retry mechanisms
- Validation rules

#### Security Features
- End-to-end encryption
- Role-based access
- Audit logging
- Session management
- API authentication
- Data backup

## Installation & Setup

```bash
# Clone repository
git clone https://github.com/TadashiJei/Impinj-RFID-System.git

# Install dependencies
npm install

# Configure environment
cp .env.example .env

# Start development server
npm run dev

# Build for production
npm run build
```

## Configuration

### Environment Variables
```env
NODE_ENV=production
PORT=3000
MONGODB_URI=mongodb://localhost:27017/rfid_system
AWS_ACCESS_KEY=your_access_key
AWS_SECRET_KEY=your_secret_key
RFID_READER_IP=192.168.1.100
```

### RFID Reader Setup
1. Configure reader IP address
2. Set power levels
3. Configure antenna settings
4. Test connectivity
5. Verify read rates

## Usage

### Basic Operations
1. Start the system
2. Configure RFID readers
3. Set up user roles
4. Configure export settings
5. Begin scanning operations

### Data Export
- Automated CSV generation
- Manual export triggers
- Customizable field mapping
- Error handling
- Backup creation

## Troubleshooting

### Common Issues
1. Reader connectivity problems
2. CSV export errors
3. Data synchronization issues
4. Performance bottlenecks

### Solutions
- Network diagnostics
- Log analysis
- Error tracking
- Performance monitoring

## Support
For technical support, contact:
- Email: support@tadashijei.com
- Hours: 24/7

## License
Copyright © 2024 Tadashi Jei. All rights reserved.
