# Campus Course & Records Manager (CCRM) - Java Project

## Overview

A comprehensive console-based Java SE application that manages students, courses, enrollments, and academic records for educational institutions. The project demonstrates advanced Java programming concepts including OOP principles, design patterns, NIO.2 file operations, Stream API, and modern Java features.

## User Preferences

Preferred communication style: Simple, everyday language.

## System Architecture

### Package Structure
```
src/edu/ccrm/
├── cli/          - Console interface and user interaction
├── domain/       - Core business entities with OOP design
├── service/      - Business logic with interface/implementation pattern
├── io/           - File operations using NIO.2 APIs
├── util/         - Utility classes and validation helpers
└── config/       - Application configuration (Singleton pattern)
```

### Core Features Implemented
- **Student Management**: Create, update, search, and manage student records
- **Course Management**: Course creation with Builder pattern, filtering capabilities
- **Enrollment System**: Handle student-course enrollments with business rules
- **Grade Management**: Record marks, calculate GPAs, generate transcripts
- **File Operations**: CSV import/export using NIO.2, backup functionality
- **Console Interface**: Interactive menu-driven CLI with graceful error handling

### Technical Highlights
- **OOP Principles**: Abstract classes (Person), inheritance, encapsulation, polymorphism
- **Design Patterns**: Singleton (AppConfig), Builder (Course), Interface segregation
- **Java 8+ Features**: Stream API, Lambda expressions, Optional, LocalDate/Time
- **Exception Handling**: Custom exceptions, try-catch-finally, multi-catch
- **File I/O**: NIO.2 Path/Files APIs, defensive programming practices
- **Code Quality**: Input validation, defensive copying, proper toString() implementations

## Technical Requirements Fulfilled

### Language Features
✅ Primitive variables, operators, operator precedence  
✅ Decision structures (if/else, switch with enhanced syntax)  
✅ Loops (while, do-while, for, enhanced-for) with break/continue  
✅ Arrays and Array utilities  
✅ String operations and methods  

### OOP Implementation
✅ **Encapsulation**: Private fields with getters/setters  
✅ **Inheritance**: Person → Student/Instructor hierarchy  
✅ **Abstraction**: Abstract Person class with abstract methods  
✅ **Polymorphism**: Interface-based service implementations  

### Advanced Concepts
✅ **Interfaces**: Service contracts with default methods  
✅ **Enums**: Grade and Semester with fields and constructors  
✅ **Nested Classes**: Course.Builder (static nested)  
✅ **Design Patterns**: Singleton (AppConfig), Builder (Course)  
✅ **Custom Exceptions**: DuplicateEnrollmentException, MaxCreditLimitExceededException  
✅ **Stream API**: Filtering, mapping, collecting operations  
✅ **NIO.2**: Path, Files APIs for modern I/O operations  
✅ **Date/Time API**: LocalDate, LocalDateTime for timestamps  

## Running the Application

### Prerequisites
- Java 19+ (GraalVM CE 22.3.1 recommended)
- Command line access

### Execution
```bash
cd src
javac -cp . edu/ccrm/CCRMApplication.java
java -cp . edu.ccrm.CCRMApplication
```

### Modes
- **Interactive Mode**: Full menu-driven interface for manual testing
- **Demo Mode**: Automatic demonstration when no input is available
- **Sample Data**: Pre-loaded students, courses, and enrollments for testing

## Recent Changes

**2025-09-25**: Complete CCRM application implementation
- Implemented all core domain classes with proper OOP design
- Created service layer with interface/implementation pattern
- Added comprehensive file I/O operations using NIO.2
- Implemented CLI interface with menu system and error handling
- Added design patterns (Singleton, Builder) and custom exceptions
- Created test data files and working application workflow

## External Dependencies

**Java Standard Library Only**
- java.time.* - Date/Time API for modern temporal handling
- java.nio.file.* - NIO.2 APIs for file operations
- java.util.stream.* - Stream API for functional programming
- java.util.* - Collections framework and utilities

**Development Tools**
- GraalVM CE 22.3.1 - Java development environment
- Standard javac compiler - Source compilation
- Console-based execution - No external frameworks required