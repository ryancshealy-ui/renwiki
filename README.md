# RenWiki — Renaissance Theatre Staff Portal

A local staff dashboard with integrated modules for staff directory, vendor management, HR handbook, and show scheduling.

## Files

- **ren-dashboard.html** — Main entry point. Shows current date/time, next upcoming show, and links to all modules
- **ren-staff-directory.html** — Staff directory with search, filtering, org chart view, and data management
- **ren-vendors-directory.html** — Vendor contacts organized by category (Concessions, Facilities, Cleaning, etc.)
- **ren-hr-handbook.html** — HR policies, procedures, and employee handbook content
- **shows-data.json** — Show schedule data (auto-loaded by dashboard). Update this with new shows.

## How to Use

### Local Access
1. Download or open these files from Google Drive
2. Open **ren-dashboard.html** in your web browser
3. Click links to navigate between modules
4. All data persists in browser storage (localStorage)

### Updating Show Data
Edit `shows-data.json` or use the "Manage Shows" button in the dashboard to add/edit/delete shows.

### Adding/Editing Staff
Click "+ Add person" in the Staff Directory to add staff members. Use the view toggles to switch between Cards, Hierarchy, and Org Chart views.

### Adding/Editing Vendors
Click "+ Add Vendor" in the Vendors Directory to add new vendor contacts.

## Data Storage

- **Staff Directory** — Stored in browser localStorage (key: `ren-staff-v1`)
- **Vendors Directory** — Stored in browser localStorage (key: `renVendors`)
- **Show Schedule** — Loaded from `shows-data.json`, can be managed via dashboard
- **HR Handbook** — Embedded in the HTML file

### Export/Import
Each module supports JSON export/import for backup and data sharing:
- Click "Export JSON" or "↓ Export" button to download data
- Click "Import JSON" or "↑ Import" button to restore data

## Customization

### Brand Colors
All modules use Renaissance Theatre brand colors:
- Primary: `#252d44` (Ren Blue)
- Accent: `#89c6e8` (Ren Accent Blue)
- White: `#FFFFFF`

Edit the CSS variables in any HTML file to customize colors.

### Adding New Modules
1. Create a new HTML file following the same template
2. Add a link in the dashboard's Quick Links section
3. Add a "← Dashboard" link in the new module's header

## Browser Compatibility

Works in any modern browser (Chrome, Firefox, Safari, Edge). No installation required.

## Updates

To update show data:
- Manually edit `shows-data.json` or
- Use the "Manage Shows" button in the dashboard

To update staff/vendors/handbook:
- Edit directly in the modules or
- Use import/export for bulk updates

---

Last Updated: May 8, 2026
