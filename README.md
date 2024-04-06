
  <div align="center">
  <h1 align="center">Budget Buddy</h1>
  <h3>Codebase for the Budget Buddy platform</h3>
  <h3>◦ Developed with the software and tools below.</h3>
  <p align="center"><img src="https://img.shields.io/badge/-React%20Native-004E89?logo=React%20Native&style=social" alt='React Native\' />
<img src="https://via.placeholder.com/1/0000/00000000" alt="spacer" /><img src="https://img.shields.io/badge/-Expo-004E89?logo=Expo&style=social" alt='Expo\' />
<img src="https://via.placeholder.com/1/0000/00000000" alt="spacer" /><img src="https://img.shields.io/badge/-Firebase-004E89?logo=Firebase&style=social" alt='Firebase\' />
<img src="https://via.placeholder.com/1/0000/00000000" alt="spacer" /><img src="https://img.shields.io/badge/-TypeScript-004E89?logo=TypeScript&style=social" alt='TypeScript\' />
<img src="https://via.placeholder.com/1/0000/00000000" alt="spacer" /><img src="https://img.shields.io/badge/-Mantine%20UI%20library-004E89?logo=Mantine%20UI%20library&style=social" alt='Mantine UI library\' />
<img src="https://via.placeholder.com/1/0000/00000000" alt="spacer" /><img src="https://img.shields.io/badge/-React%20Native%20Chart%20Kit-004E89?logo=React%20Native%20Chart%20Kit&style=social" alt='React-Native-Chart-Kit"' />
<img src="https://via.placeholder.com/1/0000/00000000" alt="spacer" />
  </p>
  </div>
  
  ---
  ## 📚 Table of Contents
  - [📚 Table of Contents](#-table-of-contents)
  - [🔍 Overview](#-overview)
  - [🌟 Features](#-features)
  - [📁 Repository Structure](#-repository-structure)
  - [💻 Code Summary](#-code-summary)
  - [🚀 Getting Started](#-getting-started)
  
  ---
  
  
  ## 🔍 Overview

 This is a React Native project with a TypeScript configuration. The project structure includes a root directory with various files and subdirectories, including the main entry point for the application (App.tsx), configuration files (eas.json, firebase.config.ts, metro.config.js), and a TypeScript configuration file (tsconfig.json).The src directory contains the source code for the application, which is organized into several subdirectories:* components: Contains reusable UI components, such as buttons, inputs, and charts.* constants: Contains constants used throughout the application, such as colors and fonts.* db: Contains the Firebase database configuration and utilities.* hooks: Contains custom React hooks for handling asynchronous storage and session management.* layout: Contains the page container component, which manages the overall layout of the application.* navigation: Contains the root navigation component, which manages the navigation between screens.* screens: Contains the individual screen components for each screen in the application.* services: Contains the API and utilities for interacting with the Firebase database.* state: Contains the context providers for managing global state, such as available categories and history data.Overall, this project appears to be a well-structured and modular React Native application with a TypeScript configuration.

---

## 🌟 Features

 Here is a list of features for the project:<br>
* React Native application with TypeScript configuration
* Modular structure with separate directories for components, constants, database, hooks, layout, navigation, screens, services, and state
* Reusable UI components, such as buttons, inputs, and charts
* Custom React hooks for handling asynchronous storage and session management
* Firebase database integration
* Global state management using context providers
* Individual screen components for each screen in the application
* Overall layout managed by the page container component
* Navigation managed by the root navigation component

---

## 📁 Repository Structure

```sh
├── .gitignore
├── app.json
├── App.tsx
├── babel.config.js
├── eas.json
├── firebase.config.ts
├── google-services.json
├── metro.config.js
├── package-lock.json
├── package.json
├── README.md
├── src
│   ├── components
│   │   ├── common
│   │   │   ├── Button
│   │   │   │   └── Button.tsx
│   │   │   ├── DisplayCard
│   │   │   │   └── DisplayCard.tsx
│   │   │   ├── Input
│   │   │   │   └── TextField.tsx
│   │   │   ├── Tab
│   │   │   │   └── Tab.tsx
│   │   │   └── Text
│   │   │       └── Text.tsx
│   │   └── specific
│   │       ├── AddToBudget.tsx
│   │       ├── AddToExpenses.tsx
│   │       ├── DisplayCard.tsx
│   │       ├── DisplayCategories.tsx
│   │       ├── HistoryItem.tsx
│   │       ├── HistoryModal.tsx
│   │       ├── HistoryStack.tsx
│   │       ├── LineChartComponent.tsx
│   │       ├── PieChartComponent.tsx
│   │       ├── SetBudget.tsx
│   │       └── TopSpendingCategory.tsx
│   ├── constants
│   │   └── colors.ts
│   ├── db
│   │   └── firebaseDB.ts
│   ├── hooks
│   │   ├── useAsyncStorage.ts
│   │   └── useSession.ts
│   ├── layout
│   │   └── PageContainer.tsx
│   ├── navigation
│   │   └── RootNavigation.tsx
│   ├── screens
│   │   ├── AddBudget
│   │   │   └── AddBudget.tsx
│   │   ├── AddExpense
│   │   │   └── AddExpense.tsx
│   │   ├── Auth
│   │   │   ├── LoginScreen.tsx
│   │   │   ├── MainScreen.tsx
│   │   │   ├── ResetPassword.tsx
│   │   │   └── SignUpScreen.tsx
│   │   ├── Category
│   │   │   └── DisplayCategoriesPage.tsx
│   │   ├── History
│   │   │   └── History.tsx
│   │   ├── Home
│   │   │   └── HomeScreen.tsx
│   │   ├── Profile
│   │   │   └── ProfileScreen.tsx
│   │   ├── Settings
│   │   │   └── SettingsScreen.tsx
│   │   ├── Stats
│   │   │   └── Stats.tsx
│   │   └── Suggestions
│   │       └── Suggestions.tsx
│   ├── services
│   │   ├── api
│   │   └── utils
│   └── state
│       └── context
│           ├── AvailableCategoriesContextProvider.tsx
│           ├── CategoriesContextProvider.tsx
│           └── HistoryContextProvider.tsx
└── tsconfig.json

```

---

## 💻 Code Summary

<details><summary>Root</summary>

| File | Summary |
| ---- | ------- |
| App.tsx |  The code defines a React Native app with a navigation container, status bar, and context providers for state management. |
| babel.config.js |  The code defines a Babel configuration file for Expo, which enables the use of ES6 syntax and specifies the root directory for module resolution. |
| firebase.config.ts |  The code initializes a Firebase app and exports its database and authentication services for use in other parts of the application. |
| metro.config.js |  The code defines a configuration object for the Metro bundler, specifically setting the resolver's main fields to react-native browser and main in order to support React Native development. |

</details>

---

<details><summary>\src\components\common\Button</summary>

| File | Summary |
| ---- | ------- |
| Button.tsx |  The code defines a React component called Button that renders a button with a title, icon, and click handler. The button can be primary or secondary, and it has a loading indicator while the click handler is being executed. |

</details>

---

<details><summary>\src\components\common\DisplayCard</summary>

| File | Summary |
| ---- | ------- |
| DisplayCard.tsx |  The code defines a React component called DisplayCard that renders a card with a label, amount, and color. |

</details>

---

<details><summary>\src\components\common\Input</summary>

| File | Summary |
| ---- | ------- |
| TextField.tsx |  The code defines a React component called TextField that renders an input field with a placeholder, a secure text entry toggle, and an optional icon. The component uses the `useState` hook to manage the secure text entry state and toggles it when the user presses the eye icon. The component also styles the input field using the `StyleSheet.create` method and passes any additional props to the underlying `TextInput` component. |

</details>

---

<details><summary>\src\components\common\Tab</summary>

| File | Summary |
| ---- | ------- |
| Tab.tsx |  The code defines a functional component called Tab that renders a pressable button with an icon and label, using React Native's Pressable component and custom styles. |

</details>

---

<details><summary>\src\components\common\Text</summary>

| File | Summary |
| ---- | ------- |
| Text.tsx |  The code defines two React components, H1 and P1, which render text elements with custom styles defined in the StyleSheet.create() method. |

</details>

---

<details><summary>\src\components\specific</summary>

| File | Summary |
| ---- | ------- |
| AddToBudget.tsx |  The code defines a React component called AddToBudget that allows the user to add a new income category and amount to a budgeting app. It uses the `useContext` hook to access the `CategoriesContext` and `HistoryContext` providers, and it defines a state variable for the label and value of the new category. The component also includes a button that triggers the `handleAddToBudget` function when pressed, which validates the input and adds the new category to the contexts if valid. |
| AddToExpenses.tsx |  The code defines a functional component named `AddToExpenses` that renders a form for adding an expense to the user's budget. The form includes a dropdown menu for selecting a category, a text input for entering a description, and a numeric input for entering the amount. The component also includes a button for submitting the form. |
| DisplayCard.tsx |  The code defines a React component called DisplayCard that renders a card with a label, amount, and icon. It uses the Feather icon library and takes in props for the label, amount, color, and icon. The component styles the card using React Native's StyleSheet API and exports it as a default export. |
| DisplayCategories.tsx |  The code defines a React Native component called DisplayCategories that displays a list of categories using a FlatList component. It uses the CategoriesContext to retrieve the list of categories and sorts them by ID in descending order. The component also defines styles for the container, scroll area, title, divider, and grid. |
| HistoryItem.tsx |  The code defines a functional component called `HistoryItem` that renders a card with information about a transaction, including the label, amount, type, date, and category. The component also includes a modal that is opened when the card is pressed, displaying more detailed information about the transaction. |
| HistoryModal.tsx |  The code defines a React component called HistoryModal that displays a modal window with information about a transaction, including the date, time, label, category, and other details. The component uses the react-native library to create a modal view with a customizable layout and styling, and it also imports several other libraries and contexts to manage state and data. |
| HistoryStack.tsx |  The code defines a React Native component called HistoryStack that displays a list of transactions from the history context, sorted by date and displayed in a scrollable area. |
| LineChartComponent.tsx |  The code defines a React component that renders a line chart using the `react-native-chart-kit` library. The chart displays two lines representing the budget and expenses for the last 30 days, with the x-axis representing the dates and the y-axis representing the amounts. The component uses the `useContext` hook to access the `CategoriesContext` and `HistoryContext` from the state, and it calculates the data for the chart based on the history data. The chart is styled using the `styles` object, which includes a container style for the chart and a title style for the chart's title. |
| PieChartComponent.tsx |  The code defines a React component called MyPieChart that renders a pie chart using the react-native-chart-kit library. The chart displays two slices, one representing Income and the other representing Expenses with the total amount of each category displayed in the center of the chart. The component uses the CategoriesContext to retrieve the total amount of each category and passes it as props to the chart. |
| SetBudget.tsx |  The code defines a React component called SetBudget that allows the user to input a budget amount and adds it to the CategoriesContext state. It also adds a history element to the HistoryContext state with the entered amount and navigates to the Home screen upon pressing the Set Budget button. |
| TopSpendingCategory.tsx |  The code defines a React component called TopSpendingCategories, which displays a list of categories with the highest spending amounts. It uses the CategoriesContext to access the list of categories and aggregates their spendings by category. The component then sorts the categories by total spendings in descending order and renders them using a FlatList. |

</details>

---

<details><summary>\src\constants</summary>

| File | Summary |
| ---- | ------- |
| colors.ts |  The code defines a constant object named colors with six properties: primary, secondary, gray, black, white, and their corresponding hexadecimal values. |

</details>

---

<details><summary>\src\db</summary>

| File | Summary |
| ---- | ------- |
| firebaseDB.ts |  The code defines a function called `firebaseDB` that returns an object with a single method, `addData`, which adds data to a Firebase Realtime Database using the `push` method and handles errors by displaying an alert. |

</details>

---

<details><summary>\src\hooks</summary>

| File | Summary |
| ---- | ------- |
| useAsyncStorage.ts |  The `useAsyncStorage` hook in React Native provides a way to store and retrieve data asynchronously using the `@react-native-async-storage/async-storage` library. It allows for the storage of a value with a given key, and provides a setter function that can be used to update the stored value. |
| useSession.ts |  The code defines a custom React hook called `useSession` that manages user authentication and session persistence using Firebase Authentication. It provides functions for signing up, signing in, signing out, and resetting passwords, as well as a `user` state variable to track the current user. |

</details>

---

<details><summary>\src\layout</summary>

| File | Summary |
| ---- | ------- |
| PageContainer.tsx |  The code defines a React component called `PageContainer` that renders a container with a margin of 50px and passes its children as a prop. |

</details>

---

<details><summary>\src\navigation</summary>

| File | Summary |
| ---- | ------- |
| RootNavigation.tsx |  The code defines a React Native app with a bottom tab navigator that displays four tabs: Home, Transactions, Suggestions, and Settings. The Home tab is the main screen of the app, while the other tabs display related information. The app also has a stack navigator for each tab, which allows users to navigate between screens within each tab. Additionally, there is an auth stack for handling user authentication and a root navigator that manages the overall navigation flow of the app. |

</details>

---

<details><summary>\src\screens\AddBudget</summary>

| File | Summary |
| ---- | ------- |
| AddBudget.tsx |  The code defines a React Native component named AddBudgetPage that displays a page with two input fields for setting an income and adding an income source to the current budget amount. |

</details>

---

<details><summary>\src\screens\AddExpense</summary>

| File | Summary |
| ---- | ------- |
| AddExpense.tsx |  The code defines a React Native component called AddExpensePage that displays a form for adding an expense to the user's total amount. It uses the CategoriesContext to retrieve the current expense amount and passes it as a prop to the AddToExpenses component. The component also defines styles for the page layout using the StyleSheet API. |

</details>

---

<details><summary>\src\screens\Auth</summary>

| File | Summary |
| ---- | ------- |
| LoginScreen.tsx |  The code defines a React Native component called LoginScreen that renders a login form with email and password fields, a Forget Password? link, and a Log In button. The component uses the useSession hook to handle user authentication and navigation. |
| MainScreen.tsx |  The code defines a React Native component called MainScreen that renders a container view with an image, two buttons, and a logo. The buttons navigate to the Login and Signup screens when pressed. |
| ResetPassword.tsx |  The code defines a React Native component called SignUpScreen that renders a form for resetting a user's password. The form includes an email input field, a button to submit the form, and a logo image. When the button is pressed, it calls the resetPassword function from the useSession hook, passing in the email address entered in the input field. If successful, it displays an alert with a success message, otherwise it displays an error message. |
| SignUpScreen.tsx |  The code defines a React Native component called `SignUpScreen` that renders a form for creating a new account, with email and password fields, a submit button, and an image logo. The component uses the `useSession` hook to handle the sign-up process and the `StyleSheet` module to style the components. |

</details>

---

<details><summary>\src\screens\Category</summary>

| File | Summary |
| ---- | ------- |
| DisplayCategoriesPage.tsx |  The code defines a React Native component called DisplayCategoriesPage, which renders a View with a container style and a DisplayCategories component. |

</details>

---

<details><summary>\src\screens\History</summary>

| File | Summary |
| ---- | ------- |
| History.tsx |  The code defines a React Native component called History that displays a segmented control with two tabs: Category Wise History and Logs When the user selects a tab, the component renders different content based on the selected index. |

</details>

---

<details><summary>\src\screens\Home</summary>

| File | Summary |
| ---- | ------- |
| HomeScreen.tsx |  The code is a React Native component that renders a homepage for a budgeting app, displaying the user's balance, income, and expenses. It also includes a button to navigate to the Statistics page and a chart to display the user's spending habits. |

</details>

---

<details><summary>\src\screens\Profile</summary>

| File | Summary |
| ---- | ------- |
| ProfileScreen.tsx |  The code defines a React Native component called `ProfileScreen` that renders a `View` with a `Text` element and a `TopSpendingCategories` component. |

</details>

---

<details><summary>\src\screens\Settings</summary>

| File | Summary |
| ---- | ------- |
| SettingsScreen.tsx |  The code defines a React Native component called `SettingsScreen` that renders a list of settings options, including Reset Default Signout and Create New Account The component also includes a `FlatList` to render the settings options, and a `Button` component to render the Reset Default and Signout buttons. |

</details>

---

<details><summary>\src\screens\Stats</summary>

| File | Summary |
| ---- | ------- |
| Stats.tsx |  The code defines a React Native component called StatsPage that displays a segmented control with two tabs: Top Spending Categories and View Insights When the user selects a tab, the component renders different content based on the selected index. The Top Spending Categories tab displays a list of top spending categories, while the View Insights tab displays a pie chart and line chart. |

</details>

---

<details><summary>\src\screens\Suggestions</summary>

| File | Summary |
| ---- | ------- |
| Suggestions.tsx |  The code defines a React Native component called Suggestions that renders a view with a text label and a background color, using the StyleSheet.create method to define the styles for the container view. |

</details>

---

<details><summary>\src\state\context</summary>

| File | Summary |
| ---- | ------- |
| AvailableCategoriesContextProvider.tsx |  The code defines a React context provider for managing a list of available categories, fetching them from Firebase Realtime Database and storing them in local state. |
| CategoriesContextProvider.tsx |  The code defines a React context for managing categories and their associated amounts, as well as functions for adding, deleting, and resetting categories. The context also includes a function to reset all category amounts and remove them from Firebase. |
| HistoryContextProvider.tsx |  The code defines a React context provider for managing a user's history data in Firebase Realtime Database. It provides a `HistoryContext` object that includes a `history` array, `addHistoryElement` function, `deleteHistoryElement` function, and `resetAllHistory` function. The context is used to manage the user's history data in Firebase and provide it to child components. |

</details>

---

## 🚀 Getting Started

 To get started with this React Native project, follow these steps:<br>
1. Install the dependencies by running `npm install` or `yarn install` in your terminal.
2. Start the development server by running `expo start` in your terminal.
3. Open the Expo app on your mobile device and scan the QR code displayed in the terminal to run the app on your device.
4. You can now use the app by navigating through the different screens and interacting with the UI components.

Note: This guide assumes that you have Node.js and npm (or yarn) installed on your system. If you don't have them installed, you can download and install them from the official websites.

---

