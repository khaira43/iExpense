# iExpense

A simple SwiftUI expense tracking app that allows users to add, view, and delete expenses, with data persisted locally using UserDefaults.

## Features

- Add new expenses with name, type (Business or Personal), and amount.  
- View a list of all expenses with details.  
- Swipe to delete expenses from the list.  
- Data persists between app launches using JSON encoding and UserDefaults.  
- Clean and intuitive UI built with SwiftUI.

## Tech Stack

- Language: Swift 5+  
- Framework: SwiftUI  
- Data Persistence: UserDefaults with Codable  
- State Management: Custom Observable class using @Observable and @State  
- UI Components: NavigationStack, List, Form, and modal sheets  

## Project Structure

iExpense/
├── ContentView.swift # Main view displaying expenses and managing addition/removal
├── AddView.swift # Form view to add new expenses
├── Expenses.swift # Observable class managing expense data and persistence

bash
Copy
Edit

## Getting Started

1. Clone the repo  
```bash
git clone https://github.com/khaira43/iExpense.git
cd iExpense
Open the project in Xcode

bash
Copy
Edit
open iExpense.xcodeproj
Build and Run

Select an iOS Simulator or a physical device

Press Cmd + R to run the app

Usage
Tap the Add Expense button (+) to open the add expense form.

Enter the expense name, select a type (Business or Personal), and input the amount.

Tap Save to add the expense to the list.

Swipe left on any expense to delete it.

Expenses are saved locally and persist between app launches.

Data Persistence
Expenses are saved in UserDefaults as JSON-encoded data every time an expense is added or removed.

On app launch, saved data is loaded and decoded back into the expense list.
