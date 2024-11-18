
# Admin Panel Dashboard

This is an Admin Panel Dashboard built with Next.js v15 and Node.js v18.19.1. 
This project is built to provide insights and management tools through a robust, secure interface. It includes authentication, data visualization, and management capabilities, allowing administrators to view, monitor, and manage system resources effectively.


## Features

- Authentication: Secure login with role-based access control for administrators.
- Dashboard: Displays an overview of key metrics and trends.
- Drawer Navigation: Expandable and collapsible menu for easy navigation.
- Form Components: Custom input and select fields for forms.


## Tech Stack

- Framework: Next.js with App Router
- Next.js v15: The React framework for building the application.
- UI Components: Material-UI (MUI) for a sleek, responsive interface. For UI components like the side drawer, buttons, etc.
- Authentication: NextAuth for session management and cookie-based authentication
- State Management: React and Context API


## Getting Started
Prerequisites

Ensure you have the following installed:

- Node.js v18.19.1
- Yarn or npm

Installation

1. Clone the repository

```bash
git clone https://github.com/your-username/admin-panel-dashboard.git
```
2. Navigate to the project directory:

```bash
cd admin-panel-dashboard
```
3. Install dependencies:

```bash
npm install
# or
yarn install

```
## Environment Variables

Create a .env.local file in the root directory and add the following variables:

```bash
NEXTAUTH_URL=http://localhost:3000
DATABASE_URL=your_database_url
SECRET=your_nextauth_secret
```

## Run Locally

To start the development server:

```bash
npm run dev
# or
yarn dev
```
Open http://localhost:3000 in your browser to view the app.



## Usage

Authentication
- Login: Only administrators can log in. The login form uses credentials and validates them through NextAuth.
- Protected Routes: Once authenticated, users are redirected to the dashboard

Navigation
- Drawer: The drawer component displays main sections. It expands on hover, with child elements nested under parent menu items.
- Dynamic Active States: Each menu item displays an active state when selected.

## Folder Structure
Here's a general overview of the folder structure:


```bash
├── components     # Reusable components (e.g., Drawer, Navbar, Charts)
├── pages          # Next.js pages
│   ├── api        # API routes for NextAuth and other endpoints
│   ├── auth       # Authentication pages
│   └── dashboard  # Main dashboard page and sub-pages
├── public         # Public assets (e.g., images, icons)
├── styles         # Global and component-specific styles
└── utils          # Utility functions (e.g., route URLs)
```
