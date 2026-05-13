# 📋 To-Do List Application with Local Storage

A modern, fully-featured to-do list web application with persistent local storage, built with vanilla JavaScript, HTML5, and CSS3.

## ✨ Features

### Core Features
- ✅ **Add Tasks** - Quick task entry with Enter key support
- ✅ **Mark Complete** - Check off completed tasks
- ✅ **Delete Tasks** - Remove individual tasks
- ✅ **Local Storage** - Automatically saves all tasks to browser storage
- ✅ **Persistent Data** - Tasks remain after page refresh/browser restart

### Advanced Features
- 🔍 **Filter Tasks** - View All, Active, or Completed tasks
- 📊 **Statistics** - Real-time counter for Total, Active, and Completed tasks
- 🗑️ **Clear Completed** - Bulk delete all completed tasks
- 💾 **Export Tasks** - Download tasks as JSON file with timestamp
- 📥 **Import Tasks** - Load tasks from exported JSON files
- 🔄 **Reset All** - Clear entire to-do list with confirmation
- 📱 **Responsive Design** - Works perfectly on desktop, tablet, and mobile
- 🎨 **Modern UI** - Beautiful gradient design with smooth animations

## 🚀 Getting Started

### Installation

1. **Download the files:**
   ```bash
   git clone https://github.com/vijayjangir5087-creator/GSTR-2A-Export-TDL.git
   cd GSTR-2A-Export-TDL/todo-app
   ```

2. **Open in Browser:**
   - Simply open `index.html` in your web browser
   - No server or installation required!
   - Works offline (uses local storage)

### Quick Usage

1. **Add a Task:**
   - Type task in the input field
   - Press Enter or click "Add Task" button

2. **Mark as Complete:**
   - Check the checkbox next to the task
   - Task text will appear strikethrough

3. **Delete a Task:**
   - Click the "Delete" button on the task
   - Confirm the deletion

4. **Filter Tasks:**
   - Click "All" to see all tasks
   - Click "Active" for incomplete tasks
   - Click "Completed" for finished tasks

5. **Export/Import:**
   - Click "Export Tasks" to download as JSON
   - Click "Import Tasks" to load from a file

## 📁 Project Structure

```
todo-app/
├── index.html        # Main HTML file
├── styles.css        # All styling and animations
├── app.js           # JavaScript logic and storage
└── README.md        # This file
```

## 💾 Local Storage

### How It Works
- All tasks are automatically saved to browser's `localStorage`
- Storage key: `todoList`
- Data persists across:
  - Browser refreshes (F5)
  - Browser closing and reopening
  - Computer restarts
  - Tab switches

### Clearing Storage
Click "Reset All" button or use browser DevTools:
```javascript
localStorage.removeItem('todoList');
```

## 📋 Task Object Structure

```json
{
  "id": 1234567890,
  "text": "Buy groceries",
  "completed": false,
  "createdAt": "5/13/2026, 10:30:45 AM"
}
```

## 🎯 Export/Import Feature

### Export Format
Tasks are exported as JSON with the filename: `todos_YYYY-MM-DD.json`

```json
[
  {
    "id": 1234567890,
    "text": "Task 1",
    "completed": false,
    "createdAt": "5/13/2026, 10:30:45 AM"
  },
  {
    "id": 1234567891,
    "text": "Task 2",
    "completed": true,
    "createdAt": "5/13/2026, 10:31:00 AM"
  }
]
```

### Import Options
- **Replace**: Existing tasks are deleted and replaced with imported ones
- **Merge**: Imported tasks are added to existing tasks

## 🎨 Styling & Themes

### Color Scheme
- **Primary**: Purple gradient (#667eea to #764ba2)
- **Accent Colors**:
  - Active: #667eea (Purple)
  - Success: #4CAF50 (Green)
  - Info: #2196F3 (Blue)
  - Warning: #ffc107 (Yellow)
  - Danger: #f44336 (Red)

### Animations
- Slide-in animation on page load
- Fade-in animation when adding tasks
- Smooth transitions on all interactive elements
- Hover effects on buttons and task items

## 📱 Responsive Breakpoints

- **Desktop**: Full 800px width container
- **Tablet**: Adjusted grid layouts
- **Mobile**: Single column layouts, optimized spacing

## ⌨️ Keyboard Shortcuts

| Action | Shortcut |
|--------|----------|
| Add Task | Enter |
| Focus Input | Tab to input field |

## 🔒 Data Privacy

- ✅ All data stored locally on your device
- ✅ No server communication or cloud storage
- ✅ No tracking or analytics
- ✅ Fully private and secure
- ✅ Complete control over your data

## 🐛 Troubleshooting

### Tasks Not Saving
- **Check**: Is localStorage enabled in your browser?
- **Fix**: Browser might have disabled it in settings

### Import Not Working
- **Check**: Is the file in JSON format?
- **Fix**: Export from this app to ensure format compatibility

### Data Lost After Update
- **Note**: Clearing browser data deletes local storage
- **Solution**: Export tasks before clearing browser data

## 🔧 Browser Compatibility

| Browser | Version | Status |
|---------|---------|--------|
| Chrome | 90+ | ✅ Fully Supported |
| Firefox | 88+ | ✅ Fully Supported |
| Safari | 14+ | ✅ Fully Supported |
| Edge | 90+ | ✅ Fully Supported |
| IE | 11 | ❌ Not Supported |

## 📚 Technologies Used

- **HTML5**: Semantic markup
- **CSS3**: Flexbox, Grid, Animations, Gradients
- **JavaScript (ES6+)**:
  - Classes and Object-Oriented Design
  - LocalStorage API
  - Event Listeners
  - File API
  - DOM Manipulation

## 🚀 Future Enhancements

- [ ] Due dates and reminders
- [ ] Task categories/tags
- [ ] Priority levels
- [ ] Search functionality
- [ ] Dark mode theme
- [ ] Cloud synchronization
- [ ] Multi-device sync
- [ ] Recurring tasks
- [ ] Subtasks support
- [ ] Custom colors and themes

## 📄 License

Open source and free to use

## 👨‍💻 Author

Vijayjangir5087-creator

## 💬 Support

Have questions? Issues? Feel free to reach out or create an issue on GitHub.

---

**Made with ❤️ using vanilla JavaScript**
