# abol-buna
## Student Information
 - **Name**: naol sisay 
 - **Student ID**: naol
 - **Course**: DSA

 # Abol Buna Cafe

This project is a simple C++ program that simulates a cafe menu system. It allows you to add items to the menu, display the menu, and calculate the total cost of an order.

## Features

- Add items to the menu with a name and price.
- Display the menu with item names and prices.
- Calculate the total cost of an order based on item indices.

## Getting Started

### Prerequisites

- A C++ compiler (e.g., GCC, Clang, MSVC)
- CMake (optional, for building the project)

### Building the Project

1. Clone the repository:
    ```sh
    git clone https://github.com/your-username/abol-buna.git
    cd abol-buna
    ```

2. Compile the project using your preferred method. For example, using `g++`:
    ```sh
    g++ -o cafe abol.cpp
    ```

3. Run the executable:
    ```sh
    ./cafe
    ```

### Using the Program

The program will Display the menu and calculate the total cost of a predefined order. You can modify the `main` function in `abol.cpp` to add more items or change the order.

```cpp
int main() {
    Cafe cafe;
    cafe.addItem("Coffee", 2.50);
    cafe.addItem("Tea", 1.75);
    cafe.addItem("Sandwich", 5.00);

    cafe.displayMenu();

    std::vector<int> order = {0, 2}; // Example order: Coffee and Sandwich
    double total = cafe.calculateTotal(order);

    std::cout << "Total: $" << total << "\n";

    return 0;
}
