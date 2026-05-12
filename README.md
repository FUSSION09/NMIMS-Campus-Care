# NMIMS-Campus-Care
A specialized Full-Stack Healthcare &amp; Campus Utility Management System designed specifically for the NMIMS university ecosystem. This portal digitizes the process of booking medical/counseling appointments and managing campus logistics.
Key Features
Smart Appointment Booking: Dynamic 30-minute time slot generation for Medical and Counseling services.

Role-Based Access Control: Dedicated dashboards and interfaces for Students, Medical Staff, and Administrators.

Real-Time Validation: SAP ID verification and conflict prevention to ensure no double-bookings.

Medical Dashboard: Comprehensive queue management for doctors, allowing them to track patient history and update visit statuses.

Secure Authentication: Integrated JWT (JSON Web Tokens) for secure session handling and data privacy.

🛠️ Technical Stack
Frontend: HTML5, CSS3 (Custom Glassmorphism Design), JavaScript (ES6).

Backend: Node.js, Express.js.

Database: MySQL (Relational Schema).

Icons/UI: FontAwesome, Poppins Font.

Tools: MySQL Workbench, Postman.

📂 Project Structure
Plaintext
├── Backend
│   ├── routes/             # API Route handlers (Auth, Appointments)
│   ├── middleware/         # JWT and Role-based Auth middleware
│   ├── db.js               # Database connection pool
│   └── index.js            # Server entry point
├── Frontend
│   ├── my-account.html      # Authentication portal
│   ├── services-booking.html # Appointment booking interface
│   ├── doctor-dashboard.html # Practitioner portal
│   └── css/                # Custom styling
└── database.sql            # Schema and initial data setup
⚙️ Setup & Installation
Clone the Repository

Bash
git clone https://github.com/yourusername/nmims-campus-care.git
cd nmims-campus-care
Database Setup

Open MySQL Workbench.

Run the provided database.sql script to create the campus_care schema and tables.

Install Dependencies

Bash
npm install
Configuration

Create a .env file and add your database credentials:

Plaintext
DB_HOST=localhost
DB_USER=root
DB_PASS=yourpassword
DB_NAME=campus_care
JWT_SECRET=yoursecretkey
Run the Server

Bash
node index.js
Open http://localhost:3000 in your browser.

Challenges Overcome
Data Synchronization: Resolved naming mismatches between the users and appointments tables to ensure accurate analytics on the Doctor Dashboard.

Slot Logic: Engineered a dynamic slot generator to manage high-frequency 30-minute appointments.

Security: Implemented protected routes to prevent students from accessing administrative data.

Contribution
Contributions are welcome! Please open an issue or submit a pull request for any enhancements.
