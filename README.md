# Coquette Task Manager ✧

A beautiful desktop task management application built with Electron, featuring a pink "coquette" aesthetic and modern UI design.

## Features

- **Task Management**: Add, edit, delete, and mark tasks as complete.
- **Priority System**: Organize tasks with High, Medium, and Low priority levels.
- **Due Dates**: Set and track task deadlines.
- **Filtering & Search**: Filter by status (All/Active/Done) and search through tasks.
- **Sorting Options**: Sort by creation date, due date, or priority.
- **Progress Tracking**: Visual progress bar showing completion percentage.
- **Local Storage**: Persistent data storage using browser localStorage. 

## Getting Started

### Prerequisites
- Node.js installed on your system
- npm package manager

### Installation

1. Clone the repository:
```bash
git clone https://github.com/raniawijaya/DesktopApp.git
cd DesktopAppTutorial
```

2. Install dependencies:
```bash
npm install
```

3. Start the application:
```bash
npm start
```

## Architecture

This Electron application follows standard security practices with:
- **Sandboxed Renderer Process**: The UI runs in a secure, isolated environment.
- **Main Process**: Handles window management and system-level operations
- **Preload Script**: Provides secure communication between processes

## Project Structure

```
DesktopApp/
├── index.html          # Main UI and application logic
├── index.js            # Electron main process
├── preload.js          # Security bridge (referenced but not shown)
├── package.json        # Project configuration and dependencies
└── package-lock.json   # Dependency lock file
```

## UI Design

The application features a distinctive "coquette" aesthetic with:
- Pink color scheme with soft gradients.
- Rounded corners and soft shadows.
- Bow ribbon decorative elements.
- Modern typography using system fonts.

## Data Management

Tasks are stored locally using browser localStorage with the following structure:
- Unique ID generation using crypto.randomUUID.
- Task properties: title, due date, priority, completion status, creation timestamp.
- Automatic save on every state change.
  
## Contributing

This appears to be an educational/tutorial project demonstrating Electron development patterns.

## Notes

This is a complete Electron desktop application that demonstrates modern web technologies in a desktop environment. The codebase shows good practices for state management, UI design, and local data persistence. The application uses a single HTML file with embedded CSS and JavaScript, making it easy to understand and modify for learning purposes.
