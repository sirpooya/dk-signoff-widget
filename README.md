# DK Sign-Off Widget

A Figma widget for managing design sign-off processes with approval tracking, date management, and checklist functionality.

## Features

### 1. **Title Section**
- Displays "Design Sign-Off" title
- Status badge with color-coded labels:
  - **Review** (Orange) - Design is under review
  - **Ready for Dev** (Green) - Design is ready for development
  - **Live** (Blue) - Design is live in production
  - **Archived** (Red) - Design is archived
- Status can be changed via property menu dropdown

### 2. **Date Section**
- **Finalization Date**: Tracks when the design was finalized
- **Last Revision**: Tracks the most recent revision date
- Both dates display in format: `YYYY Month DD - HH:MM` (e.g., "2025 December 06 - 11:20")
- Refresh button (🔄) next to each date to update to current datetime
- Dates are automatically initialized to current datetime on first load

### 3. **Approval Section**
- Three approval roles:
  - **PM** (Product Manager)
  - **Design Lead**
  - **DSM** (Design System Manager)
- Each role has a toggle button with two states:
  - **🟠 In-Review** (Light orange background) - Pending approval
  - **✅ Approved** (Light green background) - Approved
- When toggled to "Approved":
  - Automatically captures the current user's name
  - Displays user's avatar (24x24, rounded) next to the name
  - Shows placeholder avatar if user has no profile photo
- Assignee information persists across widget instances

### 4. **Property Menu Controls**
- **Status Dropdown**: Change the design status (Review, Ready for Dev, Live, Archived)

## Installation

### Prerequisites
- Node.js (comes with NPM) - [Download here](https://nodejs.org/en/download/)
- Figma Desktop App

### Setup

1. Clone or download this repository
2. Install dependencies:
   ```bash
   npm install
   ```
3. Build the widget:
   ```bash
   npm run build
   ```

## Usage

### Setting Status
1. Select the widget on the canvas
2. In the property menu (top of widget), use the dropdown to select status
3. The status badge will update with the corresponding color

### Managing Dates
- Click the refresh button (🔄) next to any date to update it to the current datetime
- Dates are automatically initialized when the widget is first created

### Approving Items
1. Click the toggle button for any role (PM, Design Lead, or DSM)
2. When switched to "Approved", your username and avatar will be automatically captured
3. The assignee information will be displayed below the role name
4. Click again to toggle back to "In-Review"

## License

MIT

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.
