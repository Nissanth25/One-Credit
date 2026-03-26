# 🏥 Hospital Trip Notification System

## Overview

The Hospital Trip Notification System is an automated solution designed to streamline hospital appointment scheduling and patient communication. It sends real-time notifications to patients, staff, and caregivers to ensure timely reminders and reduce no-shows.

---

## Features

✨ **Core Features:**

- **Automated Reminders** — Sends notifications before scheduled hospital trips
- **Real-Time Alerts** — Instant updates for appointment changes and cancellations
- **Multi-User Support** — Separate interfaces for patients, staff, and caregivers
- **Database Integration** — Seamless appointment tracking and history management
- **SMS & Email Notifications** — Multiple communication channels
- **Appointment Management** — Schedule, reschedule, and cancel appointments easily
- **Dashboard Analytics** — Track appointment statistics and no-show rates

---

## Technology Stack

| Component | Technology |
|-----------|-----------|
| Backend   | Python |
| Database  | MySQL / MongoDB |
| Notifications | SMTP (Email), Twilio (SMS) |
| Frontend  | HTML/CSS/JavaScript |
| Scheduling | APScheduler |

---

## Project Structure

```
hospital-notification-system/
├── src/
│   ├── main.py                 # Entry point
│   ├── database.py             # Database connections
│   ├── notification_service.py # Notification handler
│   ├── appointment_manager.py  # Appointment logic
│   └── config.py               # Configuration settings
├── templates/
│   ├── patient_dashboard.html
│   ├── staff_portal.html
│   └── appointment_form.html
├── database/
│   └── schema.sql              # Database schema
├── tests/
│   └── test_notifications.py
├── requirements.txt
└── README.md
```

---

## Installation & Setup

### Prerequisites
- Python 3.8+
- MySQL or MongoDB
- Git

### Steps

1. **Clone the Repository**
   ```bash
   git clone https://github.com/nissanth/hospital-notification-system.git
   cd hospital-notification-system
   ```

2. **Create Virtual Environment**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install Dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Configure Database**
   - Update `config.py` with your database credentials
   - Run database schema:
   ```bash
   mysql -u root -p < database/schema.sql
   ```

5. **Set Environment Variables**
   ```bash
   # Create .env file
   SMTP_SERVER=your_email@gmail.com
   SMTP_PASSWORD=your_password
   TWILIO_SID=your_twilio_sid
   TWILIO_TOKEN=your_twilio_token
   ```

6. **Run the Application**
   ```bash
   python src/main.py
   ```

---

## Usage

### For Patients
1. Log in to the patient dashboard
2. View upcoming appointments
3. Receive automatic reminders via SMS/Email
4. Reschedule or cancel appointments if needed

### For Hospital Staff
1. Access the staff portal
2. Manage patient appointments
3. Send custom notifications
4. View appointment statistics

### For Caregivers
1. Get notified about patient appointments
2. Receive updates on appointment changes
3. Help patients reschedule if needed

---

## Key Components

### Notification Service
Handles sending notifications through multiple channels:
- Email notifications via SMTP
- SMS alerts using Twilio API
- In-app push notifications

### Appointment Manager
Manages all appointment operations:
- Schedule new appointments
- Reschedule existing appointments
- Cancel appointments
- Track appointment history

### Database Module
Handles all database operations:
- User authentication
- Appointment storage
- Notification logs
- Analytics data

---

## API Endpoints (if applicable)

```
POST   /api/appointments        - Create new appointment
GET    /api/appointments/:id    - Get appointment details
PUT    /api/appointments/:id    - Update appointment
DELETE /api/appointments/:id    - Cancel appointment
POST   /api/notify             - Send notification
GET    /api/dashboard          - Get dashboard data
```

---

## Database Schema

### Users Table
```sql
CREATE TABLE users (
  id INT PRIMARY KEY AUTO_INCREMENT,
  name VARCHAR(100),
  email VARCHAR(100),
  phone VARCHAR(15),
  role ENUM('patient', 'staff', 'caregiver'),
  created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);
```

### Appointments Table
```sql
CREATE TABLE appointments (
  id INT PRIMARY KEY AUTO_INCREMENT,
  patient_id INT,
  appointment_date DATETIME,
  department VARCHAR(50),
  doctor_name VARCHAR(100),
  status ENUM('scheduled', 'completed', 'cancelled'),
  created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP,
  FOREIGN KEY (patient_id) REFERENCES users(id)
);
```

### Notifications Table
```sql
CREATE TABLE notifications (
  id INT PRIMARY KEY AUTO_INCREMENT,
  appointment_id INT,
  message TEXT,
  channel ENUM('email', 'sms', 'in-app'),
  status ENUM('sent', 'pending', 'failed'),
  sent_at TIMESTAMP,
  FOREIGN KEY (appointment_id) REFERENCES appointments(id)
);
```

---

## Configuration

Edit `config.py` to customize:

```python
# Database Configuration
DB_HOST = 'localhost'
DB_USER = 'root'
DB_PASSWORD = 'password'
DB_NAME = 'hospital_system'

# Notification Settings
REMINDER_DAYS_BEFORE = 1
REMINDER_HOURS_BEFORE = 2

# Email Configuration
SMTP_SERVER = 'smtp.gmail.com'
SMTP_PORT = 587

# Twilio Configuration
TWILIO_SID = 'your_account_sid'
TWILIO_AUTH_TOKEN = 'your_auth_token'
```

---

## Testing

Run the test suite:

```bash
python -m pytest tests/
```

Test coverage:
- Appointment creation and updates
- Notification delivery
- Database operations
- User authentication

---

## Troubleshooting

| Issue | Solution |
|-------|----------|
| Database connection fails | Check credentials in config.py |
| Emails not sending | Verify SMTP settings and enable less secure apps |
| SMS not received | Check Twilio SID and auth token |
| Scheduler not running | Ensure APScheduler is installed correctly |

---

## Performance Optimization

- Database indexing on frequently queried columns
- Caching appointment data with Redis (optional)
- Batch notification processing for efficiency
- Scheduled job optimization for large datasets

---

## Security Considerations

- ✅ Hash sensitive data (passwords, tokens)
- ✅ Use environment variables for credentials
- ✅ Implement role-based access control (RBAC)
- ✅ Validate all user inputs
- ✅ Use HTTPS for API communication
- ✅ Regular security audits

---

## Future Enhancements

- 🎯 Mobile app for iOS & Android
- 🎯 Multi-language support
- 🎯 Integration with hospital ERP systems
- 🎯 Voice call notifications
- 🎯 WhatsApp integration
- 🎯 AI-based appointment predictions
- 🎯 Patient feedback system

---

## Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/new-feature`)
3. Commit changes (`git commit -m 'Add new feature'`)
4. Push to branch (`git push origin feature/new-feature`)
5. Open a Pull Request

---

## License

This project is licensed under the MIT License. See LICENSE file for details.

---

## Contact & Support

**Author:** Nissanth S P  
**Email:** nissanth2k6@gmail.com  
**LinkedIn:** [Nissanth S P](https://www.linkedin.com/in/nissanth-s-p-041b94289/)  
**Codolio:** [Nissanth Profile](https://codolio.com/profile/Nissanth)

For issues, questions, or suggestions, please open an issue on GitHub or contact via email.

---

## Acknowledgments

- Built with Python, Flask/FastAPI
- Database design inspired by healthcare management systems
- Notification service powered by Twilio & SMTP
- Grateful to all contributors and testers

---

**Last Updated:** March 26, 2026  
**Version:** 1.0.0
