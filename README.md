# CPS2232-Car_Rental_Management_System

Group final project for **CPS 2232 Data Structures** at Wenzhou-Kean University.

A Java console application for a car rental business, with separate administrator and customer roles, file-based persistence, and email notifications.

## Features
- **Administrators**: add, update, and delete vehicles; view the full rental log; manage customer accounts
- **Customers**: register, log in, browse available vehicles, rent and return them
- **Availability tracking**: vehicle status is updated on every rental and return
- **Notifications**: rental confirmations sent by email through the JavaMail API
- **Persistence**: vehicles, accounts, and transaction logs stored in `Vehicles.txt`, `Accounts.txt`, and `Log.txt`

## Project structure
| File | Role |
|---|---|
| `CarRentalManagementSystem.java` | Entry point and menu loop |
| `RentalManager.java` | Rentals, availability, file I/O, and email |
| `User.java` | User accounts and authentication |
| `Vehicle.java` | Vehicle attributes and status |

## Running
Requires Java 8+ and the JavaMail library on the classpath.
```bash
export SMTP_USER="you@example.com"      # optional, for email notifications
export SMTP_PASSWORD="your-app-password"
javac -cp javax.mail.jar *.java
java -cp .:javax.mail.jar CarRentalManagementSystem
```

## Team
| Member | Contribution |
|---|---|
| Mi Yixuan | UML design, code integration, debugging, report |
| **Yiduo Yu** | `CarRentalManagementSystem` class, report |
| Zhao Yiyi | `RentalManager` class, report |
| Yu Qiyang | `User` class and user data structure, report |
| Jia Taoyin | `Vehicle` class and vehicle data, report |

## License
MIT
