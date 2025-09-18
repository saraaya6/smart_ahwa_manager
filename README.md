# Smart Ahwa Manager ☕

A Flutter application designed for coffee shop owners in Cairo to efficiently manage customer orders, track popular items, and generate sales reports. This project is built with a strong focus on clean architecture using SOLID principles and Object-Oriented Programming concepts.

## 📸 Screenshots

Here are a few screenshots of the app in action.

| Dashboard (Pending Orders) | Add New Order Screen |
| :---: | :---: |

## 🏛️ Architecture and Principles Applied

This application was designed using core OOP concepts and three main SOLID principles to ensure the codebase is modular, scalable, and maintainable.

This implementation of the Smart Ahwa Manager app is architected using core Object-Oriented concepts and SOLID principles to ensure it is modular, scalable, and maintainable. Firstly, the **Single Responsibility Principle (SRP)** is applied by separating concerns into distinct classes: the `Order` class only holds data, the `OrderManager` handles business logic like creating and completing orders, the `OrderRepository` manages data persistence, and the `SalesReporter` is solely focused on generating reports. This separation makes the system easier to understand, test, and modify, aligning with the concept of modularity from *The Object-Oriented Thought Process*.

Secondly, the **Open-Closed Principle (OCP)** is achieved through abstraction in the design of the `Drink` hierarchy. By creating an abstract `Drink` class, we can introduce new types of drinks (e.g., `HibiscusTea`) by simply adding new classes that implement the `Drink` interface without altering any existing code in the `OrderManager`. This promotes extensibility. Finally, the **Dependency Inversion Principle (DIP)** is central to the design, where high-level modules like `OrderManager` depend on the `OrderRepository` abstraction, not on a concrete implementation. This decoupling, achieved via dependency injection, allows us to easily swap the data source in the future with minimal impact on the application's business logic, thus enhancing flexibility and testability.

## 🚀 How to Run

1.  Download the project's `.zip` file from this repository.
2.  Extract the zip file.
3.  Open the project in your code editor (like VS Code).
4.  Run `flutter pub get` in the terminal.
5.  Run the app using `flutter run`.
