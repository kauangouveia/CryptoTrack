# CryptoTrack

CryptoTrack is a modern web application built using **React**, **TypeScript**, and **Clean Architecture** principles. The application provides users with real-time tracking and analysis of cryptocurrency data, leveraging external APIs like CoinGecko. This project is structured for scalability, maintainability, and testability.

## **Features**

- Real-time cryptocurrency price tracking.
- Historical data and chart visualizations.
- Search and filter functionality for different cryptocurrencies.
- Integration with external APIs for reliable data.
- Modular and scalable codebase following Clean Architecture.

---

## **Technologies Used**

### **Core Frameworks and Libraries**

- **React**: Front-end library for building user interfaces.
- **TypeScript**: Strongly-typed language for improved code reliability.
- **Jest & Testing Library**: Testing frameworks for unit and integration tests.

### **Project Structure**

This project follows the principles of **Clean Architecture**, ensuring a clear separation of concerns.

```
src/
├── core/               # Business logic and use cases
│   ├── useCases/       # Application-specific logic
│   └── errors/         # Custom error handling
├── domain/             # Domain entities and contracts
│   ├── entities/       # Core domain objects
│   └── types/          # Type definitions and DTOs
├── infra/              # Infrastructure and external services
│   ├── api/            # API integrations
│   ├── repositories/   # Repository implementations
│   └── monitoring/     # Performance monitoring
├── presentation/       # UI components and pages
│   ├── components/     # Reusable components
│   ├── pages/          # Application pages (e.g., Dashboard, Profile)
│   ├── hooks/          # Custom React hooks
│   └── styles/         # Global and scoped styles
├── tests/              # Automated tests
│   ├── unit/           # Unit tests
│   ├── integration/    # Integration tests
│   └── e2e/            # End-to-end tests
├── assets/             # Static assets (e.g., images, icons)
├── App.tsx             # Root application component
├── index.tsx           # Main entry point of the application
├── setupTests.ts       # Test setup file for Jest
└── reportWebVitals.ts  # Performance reporting (optional)
```

---

## **Folder Breakdown**

### **1. core/**

This folder contains the core business logic of the application:

- `useCases/`: Implements use cases (e.g., FetchCryptoPrices, CalculateMetrics).
- `errors/`: Defines custom error types for better error handling.

### **2. domain/**

Holds domain-specific objects and definitions:

- `entities/`: Core entities like `Crypto`, `User`.
- `types/`: DTOs (Data Transfer Objects) and shared TypeScript types.

### **3. infra/**

Manages external integrations and system-level services:

- `api/`: Handles API calls (e.g., CoinGecko API integration).
- `repositories/`: Implements data access logic.
- `monitoring/`: Contains performance monitoring tools (e.g., `reportWebVitals.ts`).

### **4. presentation/**

Handles user-facing components and views:

- `components/`: Reusable UI components like buttons, modals, etc.
- `pages/`: Represents full pages (e.g., Dashboard, Login).
- `hooks/`: Custom hooks for state management and shared logic.
- `styles/`: Manages global and scoped CSS or CSS-in-JS.

### **5. tests/**

Contains all test files:

- `unit/`: Isolated tests for individual functions or components.
- `integration/`: Tests for multiple modules working together.
- `e2e/`: Full end-to-end tests simulating user interactions.

### **6. assets/**

Stores static assets such as images, SVGs, and icons.

### **Other files**

- **`App.tsx`**: Root component that initializes the application layout and routing.
- **`index.tsx`**: Entry point for ReactDOM to render the application.
- **`setupTests.ts`**: Configures Jest and Testing Library for consistent test environments.
- **`reportWebVitals.ts`**: Optional performance monitoring for the application.

---

## **Getting Started**

### **Prerequisites**

Make sure you have the following installed:

- **Node.js**: v16 or later
- **npm**: v7 or later

### **Installation**

1. Clone the repository:
   ```bash
   git clone https://github.com/your-repo/cryptotrack.git
   ```
2. Navigate to the project folder:
   ```bash
   cd cryptotrack
   ```
3. Install dependencies:
   ```bash
   npm install
   ```

### **Running the Application**

Start the development server:

```bash
npm start
```

The application will be available at `http://localhost:3000/`.

### **Running Tests**

Run unit and integration tests with:

```bash
npm test
```

### **Building for Production**

Build the application for production:

```bash
npm run build
```

---

## **Contributing**

Feel free to submit issues or pull requests to improve the project. Make sure to follow the existing code structure and include tests for new features.

---

## **License**

This project is licensed under the MIT License. See the `LICENSE` file for more details.
