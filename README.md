#   BFB Semester Project - Supply Chain Web Appliaction

This project is a **web-based logistics management system** developed for BFB321. 
It allows for users to manage **drivers, trucks, deliveries, odometer logs, and maintenance records** through asimple HTML/CSS interface with a supporting SQL schema.

---

## Overview
The system provides:
- A dashboard linking all main modules
- HTML pages for drivers, vehicles, delivery history
- A shared CSS file for consistent styling
- An SQL schema and demo database to support backend integration in the future

**Tech Stack**
- Frontend: HTML, CSS
- Data Layer: SQL schema (`TruckDelivery.sql`) + SQLite demo DB (`TruckDelivery.db`)
- Optional future extension: Flask + Bootstrap 

---

## Features
- **Dashboard (`home.html`, `index.html`)**
  Landing page with navigation to different modules.
- **Driver Management (`drivers.html`)**
  List of drivers with contact details and assigned vehicles.
- **Vehicle Management (`vehicle.html`)**
  Truck information including codes and license plates.
- **Delivery History (`history.html`)**
  Records of completed deliveries.
- **Styling (`main.css`)**
  Consistent styles for tables, navigation, and layout.
- **Database Support (`TruckDelivery.sql`, `TruckDelivery.db`)**
  Schema and example database for drivers, trucks, deliveries, odometer logs, and maintenance logs.

---

## System Design

### ER Diagram

<img width="730" height="851" alt="ERD" src="https://github.com/user-attachments/assets/5239181d-5541-482f-a08c-f7be0488ce2a" />

### Tables 
1. **drivers**: Stores driver details (name, phone, assigned truck).
2. **trucks**: Information about each truck (code, license plate).
3. **deliveries**: Records of deliveries with pickup/drop-off info and status. 
4. **maintenance_logs**: History of maintenance done on trucks.
5. **odometer_logs**: Mileage records for trucks over time. 

### Sample Data
The database includes sample entries for testing: 
- Drivers with phone numbers and assigned trucks.
- Trucks with codes and license plates.
- Delivery records with statuses (Pending, In Transit, Delivered).
- Example maintenance logs and odometer readings.

## File Structure
```
├─ index.html           # Main dashboard / entry point.
├─ home.html            # Dashboard with navigation cards.
├─ drivers.html         # Manage and view drivers.
├─ vehicle.html         # Manage and view trucks.
├─ history.html         # Delivery history records. 
├─ main.css             # Styling for tables, layout, and dashboard.
├─ TruckDelivery.sql    # Database schema.
├─ TruckDelivery.db     # SQLite sample database.
└─ README.md            # Documentation
```
## Usage

1. Open the project folder in VS Code.
2. Double-click the `index.html` and the web browser will open up.
3. Navigate the different pages to manage the drivers or trucks.

## Technologies Used

- **HTML5**: Structure and static pages.
- **CSS3**: Styling and responsive layout.
- **Bootstrap Icons**: Icon set for UI elements. 
- **SQLite / SQL Schema**: For data storage and testing. 

## Browser Compatibility

The application works with all modern browsers that support HTML5 and CSS3, including:

- Chrome 90+
- Firefox 88+ 
- Safari 14+ 
- Edge 90+

**Note:** This is a static HTML/CSS application. For production use, backend functionality would be required for database connectivity and form processing. 