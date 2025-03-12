# IP Address Management in Java
This project was developed as part of a Java programming course to demonstrate object-oriented programming concepts and basic IP address management. It provides a simple Java implementation for managing and analyzing IP addresses, including functionality to:

- **Create IP Addresses**: Instantiate IP addresses using four octets (e.g., `192.168.0.1`).

- **Validate IP Addresses**: Ensure that each octet is within the valid range (0-255).

- **Determine IP Class**: Identify the class of an IP address (A, B, or C).

- **Calculate Network Address**: Compute the network address based on the IP class.

- **Check if IPs are on the Same Network**: Compare two IP addresses to determine if they belong to the same network.

## Key Features
- **IP Address Creation**: Use the `getInstance` method to create an IP address with four octets.

- **IP Class Detection**: The `getClasse` method returns the class of the IP address (A, B, or C).

- **Network Address Calculation**: The `adresseReseau` method calculates the network address based on the IP class.

- **Network Comparison**: The `estMemeReseau` method checks if two IP addresses are on the same network.

## Example Usage
```
IpPackage ip1 = IpPackage.getInstance(192, 168, 0, 7);
System.out.println("Class of ip1: " + ip1.getClasse());
System.out.println("Network Address of ip1: " + ip1.adresseReseau().ToString());

IpPackage ip2 = IpPackage.getInstance(192, 168, 1, 10);
System.out.println("Are ip1 and ip2 on the same network? " + ip1.estMemeReseau(ip2));
```

## Project Structure
- **IpPackage.java**: Contains the `IpPackage` class with methods for IP address management.

- **IpTest.java**: A test class demonstrating the usage of the `IpPackage` class.

## About This Project
This project was assigned as part of a Java programming course to help students learn and practice object-oriented programming concepts, including class design, encapsulation, and basic networking principles. It serves as a practical example of how to work with IP addresses in Java.