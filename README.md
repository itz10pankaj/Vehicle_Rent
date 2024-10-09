# Vehicle Rental System

## Overview

This project is a **Vehicle Rental System** that allows users to book, return, and view different types of vehicles such as Cars, Bikes, and Trucks. It is designed with Object-Oriented Programming (OOP) concepts and provides two primary interfaces for **Admin** and **User** interactions.

Admins can manage the vehicle inventory by adding, updating, and deleting vehicles. Users can book and return vehicles, as well as view the vehicles they have booked. 

## Features

### Admin Features:
1. **Login**: Admin can log in using their credentials.
2. **Vehicle Management**:
   - Add a vehicle (Car, Bike, Truck) to the inventory.
   - Delete a vehicle from the inventory.
   - Update the details of a vehicle (model, license plate, rate per day).
   - View the current inventory of vehicles.

### User Features:
1. **User Registration/Login**:
   - New users can register with their name, email, contact number, and password.
   - Registered users can log in using their credentials.
   
2. **Vehicle Booking**:
   - View available vehicles and book them for a specified number of days.
   - Users can book multiple vehicles.

3. **Return Vehicle**:
   - Users can return the vehicles they have booked.
   
4. **View Booked Vehicles**:
   - Users can view the list of vehicles they have booked.

### Vehicle Types:
- **Car**: Represents a car available for booking.
- **Bike**: Represents a bike available for booking.
- **Truck**: Represents a truck available for booking.

## Classes and Structure

### `Vehicle` (Base Class):
- Stores details about a vehicle such as model, license plate, rate per day, and availability.
- Provides methods to update vehicle details and check availability.

### Derived Classes:
1. **`Car`**: Inherits from `Vehicle`.
2. **`Bike`**: Inherits from `Vehicle`.
3. **`Truck`**: Inherits from `Vehicle`.

### `User` (Base Class):
- Stores user information (name, email, contact, password).
- Users can book, return, and view their booked vehicles.

### `Admin` (Inherits from `User`):
- Manages the vehicle inventory (add, update, delete vehicles).
- Authenticates the admin using email and password.

### `Rental`:
- Handles the booking and returning of vehicles.
- Allows users to book available vehicles and calculates the total cost based on the number of days.

## Project Structure

```cpp
#include <iostream>
#include <vector>
#include <string>
#include <unordered_map>
#include <algorithm>

// Classes: Vehicle, Car, Bike, Truck, User, Admin, Rental
```

## How to Run

1. **Clone the Repository**: Clone this repository to your local machine.
   ```bash
   git clone <repo_link>
   ```
   
2. **Compile and Run**: Use any C++ compiler (like g++, clang++) to compile the project.
   ```bash
   g++ vehicle_rental_system.cpp -o rental
   ./rental
   ```

3. **Admin Login**:
   - Email: `admin@gmail.com`
   - Password: `12345678`

4. **User Registration/Login**:
   - New users can register by providing their name, email, contact, and password.

## Example Workflow

### Admin Side:
1. Log in as an admin.
2. Add a vehicle to the inventory (e.g., Car, Bike, Truck).
3. View the inventory to see the list of available vehicles.
4. Delete or update vehicle details as needed.

### User Side:
1. Register or log in as a user.
2. View available vehicles and book one or more.
3. Return a booked vehicle after use.
4. View the list of booked vehicles.

## Future Enhancements

- **Payment Integration**: Adding a payment gateway for users to complete transactions.
- **Date/Time Validation**: Implement a real-time date system to handle vehicle availability.
- **Admin Dashboard**: Improve the admin dashboard to include detailed analytics and reporting.

## Contact

If you have any questions or suggestions, feel free to reach out to Pankaj at `pgarg9355@gmail.com`.

## License

This project is open-source and free to use for educational purposes.
