# Automated File Organizer 📂

A professional desktop application built with **Python** and **Tkinter** that automatically organizes files inside a selected folder into categorized subfolders based on their file extensions.

> Developed as part of a **Python Programming Internship** project.
> 


## 📋 Project Overview

Managing files on a computer can become chaotic, especially when downloads pile up with no structure. The **Automated File Organizer** solves this problem by scanning a selected folder and intelligently sorting files into categorized subfolders — all through a sleek, user-friendly graphical interface.

With a single click, your messy folder transforms into a neatly organized directory structure.

---

## ✨ Features

| Feature | Description |
|---------|-------------|
| 📁 Folder Selection | Browse and select any folder on your computer |
| 🔍 Smart Scanning | Scans all files in the selected directory |
| 📂 Auto-Categorization | Creates and sorts files into 7 categories |
| 📊 Progress Tracking | Real-time progress bar with percentage display |
| 📋 Activity Log | Scrollable log showing every file operation |
| 📝 Log File | Generates `organizer_log.txt` for record keeping |
| 🔄 Duplicate Handling | Safely renames duplicate files (appends `_1`, `_2`, etc.) |
| ⚡ Non-Blocking UI | File operations run on background threads |
| ✅ Summary Popup | Shows completion summary with category breakdown |
| 🛡️ Error Handling | Graceful exception handling prevents crashes |

---

## 📂 File Categories

| Category | Extensions |
|----------|-----------|
| 🖼️ Images | `.jpg`, `.jpeg`, `.png`, `.gif`, `.bmp`, `.svg`, `.webp`, `.ico`, `.tiff` |
| 📄 Documents | `.pdf`, `.docx`, `.doc`, `.txt`, `.pptx`, `.xlsx`, `.csv`, `.rtf`, `.odt` |
| 🎬 Videos | `.mp4`, `.avi`, `.mkv`, `.mov`, `.wmv`, `.flv`, `.webm` |
| 🎵 Audio | `.mp3`, `.wav`, `.aac`, `.flac`, `.ogg`, `.wma` |
| 📦 Archives | `.zip`, `.rar`, `.7z`, `.tar`, `.gz`, `.bz2` |
| ⚙️ Programs | `.exe`, `.msi`, `.deb`, `.dmg`, `.apk` |
| 📁 Others | Any file type not listed above |

---

## 🛠️ Technologies Used

- **Python 3** — Core programming language
- **Tkinter** — GUI framework (built-in with Python)
- **os** — File system operations and path handling
- **shutil** — High-level file moving operations
- **threading** — Background thread for non-blocking UI
- **logging** — Professional log file generation

---

## 📥 Installation Steps

### Prerequisites

- Python 3.6 or higher installed on your system
- No additional packages required (all libraries are part of the Python standard library)

### Steps

1. **Clone or download** this project to your local machine:
   ```bash
   git clone https://github.com/yourusername/Automated_File_Organizer.git
   ```

2. **Navigate** to the project directory:
   ```bash
   cd Automated_File_Organizer
   ```

3. **Run** the application:
   ```bash
   python main.py
   ```

---

## 🚀 Usage Instructions

1. **Launch** the application by running `main.py`.
2. Click the **Browse** button to select a folder you want to organize.
3. Review the folder path displayed in the application.
4. Click the **⚡ Organize Files** button.
5. Confirm the action in the popup dialog.
6. Watch the **progress bar** and **activity log** as files are organized.
7. View the **completion summary** popup with a category breakdown.
8. Check `organizer_log.txt` in the organized folder for a detailed record.

---

## 📸 Screenshots

### Main Interface
*The application features a modern dark-themed interface with folder selection, progress tracking, and a real-time activity log.*

### Organization in Progress
*Files are moved with live progress updates, showing each file and its destination category.*

### Completion Summary
*A popup displays the total files organized with a per-category breakdown.*

> **Note:** Add your own screenshots in the `assets/` folder and update the paths above.

---

## 📁 Project Structure

```
Automated_File_Organizer/
│
├── main.py              # GUI application (Tkinter interface)
├── organizer.py          # Core file organization engine
├── organizer_log.txt     # Generated log file (created on first run)
├── assets/               # Application assets (icons, screenshots)
└── README.md             # Project documentation
```

### Module Breakdown

| File | Purpose |
|------|---------|
| `main.py` | Contains the `FileOrganizerApp` class — builds the GUI, handles user interactions, and manages background threads |
| `organizer.py` | Contains the `FileOrganizer` class — handles file scanning, categorization, safe moving, and log generation |

---

## 🏗️ Architecture

```
┌──────────────────────────┐
│       main.py (GUI)       │
│  ┌────────────────────┐  │
│  │  FileOrganizerApp  │  │
│  │  - Browse folder   │  │
│  │  - Start organize  │  │
│  │  - Show progress   │  │
│  │  - Activity log    │  │
│  └────────┬───────────┘  │
│           │               │
│    Background Thread      │
│           │               │
│  ┌────────▼───────────┐  │
│  │   organizer.py     │  │
│  │  ┌──────────────┐  │  │
│  │  │FileOrganizer │  │  │
│  │  │- scan_files  │  │  │
│  │  │- categorize  │  │  │
│  │  │- move_file   │  │  │
│  │  │- log actions │  │  │
│  │  └──────────────┘  │  │
│  └────────────────────┘  │
└──────────────────────────┘
```

---

## 🔮 Future Enhancements

- [ ] **Recursive Organization** — Support for organizing files in subdirectories
- [ ] **Custom Categories** — Allow users to define their own file categories and extensions
- [ ] **Undo Feature** — Ability to reverse the last organization operation
- [ ] **Scheduling** — Auto-organize folders at scheduled intervals
- [ ] **Drag & Drop** — Support folder selection via drag and drop
- [ ] **File Preview** — Preview files before organizing
- [ ] **Statistics Dashboard** — Visual charts showing file distribution
- [ ] **Multi-folder Support** — Organize multiple folders in one session
- [ ] **Settings Persistence** — Save user preferences between sessions
- [ ] **Dark/Light Theme Toggle** — Allow users to switch between themes

---

## 📄 License

This project is open source and available for educational purposes.

---

## 👨‍💻 Author

**Karthick Raja B**  
Computer Science Engineering Student  
Python Programming Internship Project

---

> *Built with ❤️ using Python and Tkinter*
