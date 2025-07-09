# 🏦 Banking Management System

A comprehensive console-based banking system built in C++ using **Functional Programming** paradigm. This system provides complete bank operations including user authentication, client management, and transaction processing.

## 🚀 Features

### 👥 User Management
- **Multi-user authentication** with username/password
- **Role-based permissions** system with granular access control
- **User administration** (add, update, delete users)
- **Session management** with secure login/logout

### 👤 Client Management
- **Complete CRUD operations** for client accounts
- **Account validation** with unique account number enforcement
- **Client search** functionality
- **Detailed client information** display with formatted tables

### 💰 Transaction System
- **Deposit** funds with confirmation
- **Withdraw** funds with balance validation
- **Balance inquiry** for individual accounts
- **Total balance** calculation across all accounts
- **Transaction confirmations** for security

### 🔐 Security Features
- **Permission-based access** control (7 different permission levels)
- **Administrative privileges** with full system access
- **Input validation** and confirmation prompts
- **Secure session handling**

## 🛠️ Technical Architecture

### Programming Paradigm
This system is built using **Functional Programming** principles:
- Functions as first-class citizens
- Modular design with pure functions where possible
- Minimal global state
- Data transformation through function composition

### Data Storage
- **File-based persistence** using custom text format
- **Structured data** with delimiter-based serialization
- **Two-file system**: `clients.txt` and `users.txt`
- **Soft deletion** mechanism for data integrity

### Permission System
Uses **bitwise operations** for efficient permission management:
```
Bit 0: Show Clients List
Bit 1: Add New Clients
Bit 2: Delete Clients
Bit 3: Update Client Information
Bit 4: Find Clients
Bit 5: Transaction Operations
Bit 6: Manage Users
```

## 📁 Project Structure

```
banking-system/
├── src/
│   └── bank.cpp                 # Main application file
├── datafiles/
│   ├── clients.txt              # Client data storage
│   └── users.txt                # User credentials storage
├── exe/
│   └── (compiled executable)
└── README.md
```

## 🔧 Installation & Setup

### Prerequisites
- C++ compiler (GCC, Clang, or MSVC)
- Windows/Linux/MacOS environment

### Compilation

#### Windows (PowerShell)
```powershell
g++ src\bank.cpp -o exe\bank.exe
```

#### Linux/MacOS
```bash
g++ src/bank.cpp -o exe/bank
```

### Running the Application

#### Windows
```powershell
exe\bank.exe
```

#### Linux/MacOS
```bash
./exe/bank
```

## 🎯 Usage Guide

### First Time Setup
1. **Create data directory**: Ensure `datafiles` folder exists
2. **Initialize users**: Create your first admin user
3. **Login**: Use your credentials to access the system

### Default Admin User
```
Username: admin
Password: admin123
Permissions: -1 (Full Access)
```

### Main Menu Options
1. **[1] Show List** - Display all clients
2. **[2] Add New Client** - Register new account
3. **[3] Delete Client** - Remove client account
4. **[4] Update Client** - Modify client information
5. **[5] Find Client** - Search for specific client
6. **[6] Transactions Menu** - Access banking operations
7. **[7] Manage Users Menu** - User administration
8. **[8] Show Current User** - Display logged-in user info
9. **[9] Logout** - Exit to login screen

### Transaction Operations
- **Deposit**: Add funds to any account
- **Withdraw**: Remove funds (with balance validation)
- **Total Balances**: View system-wide balance summary

## 🔒 Security Considerations

### Current Security Features
- Role-based access control
- Transaction confirmations
- Input validation on critical operations
- Session-based authentication

### Security Limitations
- Passwords stored in plain text
- No encryption for sensitive data
- Local file storage without access controls

## 🚧 Known Limitations

- **Performance**: Linear search operations (O(n))
- **Scalability**: File-based storage not suitable for large datasets
- **Concurrency**: No support for multiple simultaneous users
- **Security**: Basic authentication without encryption

## 🔮 Future Development

### Upcoming OOP Version
I'm currently developing an **Object-Oriented Programming** version of this system that will include:

#### 🎨 Enhanced Features
- **Modern C++ Design** with classes and objects
- **Advanced Security** with password hashing and encryption
- **Multi-threading** support for concurrent operations
- **Better CLI Interface** Focus on the CLI and inhance it
- **Advanced Reporting** with transaction history
- **Backup and Recovery** mechanisms
- **Configuration Management** system
- **Logging and Auditing** capabilities
- **More Features** adding More Featurs to the system

## 🤝 Contributing

Contributions are welcome! Please feel free to submit issues, feature requests, or pull requests.

### Development Guidelines
1. Follow existing code style and conventions
2. Add appropriate comments for complex logic
3. Test thoroughly before submitting
4. Update documentation as needed

## 📧 Contact

For questions, suggestions, or collaboration opportunities, please reach out:

- **GitHub Issues**: [Create an issue](../../issues)
- **Email**: yousefalinl0@gmail.com
- **LinkedIn**: https://www.linkedin.com/in/joedev000/

## 🙏 Acknowledgments

- Thanks to the C++ community for excellent documentation
- Inspiration from real-world banking systems
- Educational resources that helped shape this project

---

## 📈 Version History

### v1.0.0 (Current - Functional Programming)
- ✅ Complete banking operations
- ✅ User authentication and authorization
- ✅ File-based data persistence
- ✅ Transaction management
- ✅ Role-based permissions

### v2.0.0 (Coming Soon - Object-Oriented)
- 🔄 Complete OOP redesign
- 🔄 Enhanced security features
- 🔄 better CLI interface
- 🔄 Advanced reporting
- 🔄 More featres

---

# Author

## Joe Ali

- Software Developer & Open Source Programmer
- GitHub: [@JoeDev000](https://github.com/JoeDev000)

Copyright (c) 2025 Joe Ali

**⭐ Star this repository if you find it useful!**