# FULL STACK - QUICK EXAM NOTES (THANGLISH)

---

## PART-A (2 MARKS)

### 1. Frontend vs Backend

| Frontend | Backend |
|----------|---------|
| User paakkura part | Server-side logic |
| HTML, CSS, JavaScript | Node.js, Python, Java |
| Browser la run | Server la run |
| UI/UX design | Database, API handling |

---

### 2. Frontend - 2 Key Responsibilities

1. **UI Rendering** - HTML/CSS use panni pages display
2. **User Interaction** - Clicks, forms, backend-ku requests

---

### 3. MERN Stack Components

**M** = MongoDB (Database)  
**E** = Express.js (Backend framework)  
**R** = React (Frontend library)  
**N** = Node.js (Runtime)

---

### 4. Express.js Role

- HTTP requests handle (GET, POST, PUT, DELETE)
- Routes create panna
- MongoDB-ku connect
- Middleware support

```javascript
app.get('/api/users', (req, res) => {
    res.json({users: ['Ram', 'Sita']});
});
```

---

### 5. CSS Box Model

```
┌─────────────────┐
│    MARGIN       │
│  ┌───────────┐  │
│  │  BORDER   │  │
│  │ ┌───────┐ │  │
│  │ │PADDING│ │  │
│  │ │┌─────┐│ │  │
│  │ ││CONT││ │  │
│  │ │└─────┘│ │  │
│  │ └───────┘ │  │
│  └───────────┘  │
└─────────────────┘
```

**Components:**  
Content → Padding → Border → Margin

---

### 6. Display Properties

| Type | Behavior | Width/Height |
|------|----------|--------------|
| **inline** | Same line | Set panna mudiyaadhu |
| **block** | New line | Set pannalam |
| **inline-block** | Same line | Set pannalam |

---

### 7. Grid vs Flexbox

| Grid | Flexbox |
|------|---------|
| 2D (rows + columns) | 1D (row OR column) |
| Complex layouts | Simple alignment |
| Dashboard, gallery | Navbar, cards |

---

### 8. z-index Property

- Elements overlap aacha yaar top-la nu decide
- Higher value = top la
- Only positioned elements-ku work (position: relative/absolute)

```css
.box1 { z-index: 1; }   /* Behind */
.box2 { z-index: 10; }  /* Front */
```

---

### 9. var, let, const

| Feature | var | let | const |
|---------|-----|-----|-------|
| **Scope** | Function | Block {} | Block {} |
| **Reassign** | ✅ | ✅ | ❌ |
| **Modern** | ❌ Avoid | ✅ Use | ✅ Default |

---

### 10. Arrays & map()

```javascript
let nums = [1, 2, 3, 4];

// map() - new array create
let doubled = nums.map(n => n * 2);
// [2, 4, 6, 8]
```

---

## PART-B (13 MARKS)

### 11A. Three-Tier Architecture

**Layers:**
```
Frontend (Browser) 
    ↓ HTTP
Backend (Server/API)
    ↓ Query
Database (MongoDB/MySQL)
```

**Example:** E-commerce
- Frontend: Product display
- Backend: Order processing
- Database: User data, products

**Monolithic vs Microservices:**

| Monolithic | Microservices |
|-----------|---------------|
| Single codebase | Multiple services |
| Easy deploy | Complex deploy |
| Full app scale | Individual scale |
| Fast (no network) | Slower (network calls) |
| **Use:** Small apps | **Use:** Large apps |

---

### 11B. MERN Stack Overview

**Components:**

**1. MongoDB** - NoSQL, JSON format
```javascript
{name: "Ram", age: 25}
```

**2. Express.js** - Backend routes
```javascript
app.get('/users', (req,res) => res.json(users));
```

**3. React** - Frontend UI
```javascript
function App() { return <h1>Hello</h1>; }
```

**4. Node.js** - Server runtime

**Why MERN > LAMP:**
- Single language (JavaScript everywhere)
- JSON native
- Fast, modern, async

---

### 12A. MERN Setup

**Steps:**

1. **Install:** Node.js, npm
2. **Backend:**
```bash
npm init -y
npm i express mongoose cors
```

3. **Frontend:**
```bash
npx create-react-app frontend
```

4. **MongoDB:** Compass or Atlas

5. **Git:**
```bash
git init
```

**Troubleshooting:**
- Port busy → `kill -9 <PID>`
- CORS error → `app.use(cors())`
- Module error → `npm install`

---

### 12B. HTML5 Structure

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Page</title>
</head>
<body>
    <header>
        <nav><a href="#home">Home</a></nav>
    </header>
    
    <main>
        <section>
            <h1>Welcome</h1>
            <img src="pic.jpg" alt="Image">
            <video controls><source src="v.mp4"></video>
        </section>
        
        <form>
            <input type="email" required>
            <select><option>Chennai</option></select>
            <textarea></textarea>
            <button type="submit">Send</button>
        </form>
    </main>
    
    <footer>&copy; 2024</footer>
</body>
</html>
```

**Responsive Support:**
- Viewport meta tag
- Media queries
- Flexible images (max-width: 100%)

---

### 13A. Box Model, Flexbox, Grid

**Box Model:**
```css
.box {
    width: 200px;
    padding: 20px;
    border: 2px solid;
    margin: 10px;
}
Total = 200 + 40 + 4 = 244px
```

**Flexbox Center:**
```css
.container {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
}
```

**Grid Center:**
```css
.container {
    display: grid;
    place-items: center;
    height: 100vh;
}
```

**When to Use:**
- Flexbox: 1D (navbar, cards)
- Grid: 2D (dashboard, gallery)

**Browser Support:** Both 97%+ ✅

---

### 13B. CSS Typography

**Font Stacks:**
```css
font-family: Arial, Helvetica, sans-serif;
```

**Units:**
- `px` - Fixed
- `rem` - Relative to root (best)
- `em` - Relative to parent

**Responsive Scale:**
```css
:root {
    --font-sm: 0.875rem;  /* 14px */
    --font-base: 1rem;    /* 16px */
    --font-lg: 1.25rem;   /* 20px */
    --font-xl: 2rem;      /* 32px */
}

h1 { font-size: var(--font-xl); }
p { font-size: var(--font-base); }
```

**Accessibility:**
- Contrast: 4.5:1 minimum
- Min font-size: 16px
- Line-height: 1.5

---

### 14A. Mobile-First vs Desktop-First

**Mobile-First:**
```css
/* Base: Mobile */
.container { padding: 1rem; }

/* Tablet+ */
@media (min-width: 768px) {
    .container { padding: 2rem; }
}
```

**Desktop-First:**
```css
/* Base: Desktop */
.container { padding: 3rem; }

/* Tablet- */
@media (max-width: 767px) {
    .container { padding: 1rem; }
}
```

**Hero Section:**
```css
.hero {
    min-height: 100vh;
    padding: clamp(1rem, 5vw, 3rem);
}

.title {
    font-size: clamp(2rem, 5vw, 4rem);
}
```

**Performance:** Mobile-first better (smaller CSS)

---

### 14B. Bootstrap Dashboard

```html
<!-- Navbar -->
<nav class="navbar navbar-dark bg-dark">
    <a class="navbar-brand">Dashboard</a>
</nav>

<!-- Layout -->
<div class="container-fluid">
    <div class="row">
        <div class="col-md-3 sidebar">Sidebar</div>
        <div class="col-md-9">
            <!-- Cards -->
            <div class="row">
                <div class="col-md-3">
                    <div class="card">
                        <div class="card-body">
                            <h5>Users</h5>
                            <h2>1,234</h2>
                        </div>
                    </div>
                </div>
            </div>
            
            <!-- Table -->
            <table class="table">
                <thead><tr><th>Name</th></tr></thead>
                <tbody><tr><td>Ram</td></tr></tbody>
            </table>
        </div>
    </div>
</div>

<!-- Modal -->
<div class="modal" id="myModal">
    <div class="modal-dialog">
        <div class="modal-content">
            <div class="modal-header">Title</div>
            <div class="modal-body">Content</div>
        </div>
    </div>
</div>
```

**Utility Classes:**
- `mb-3` - margin-bottom
- `d-flex` - display flex
- `justify-content-center` - center
- `d-none d-md-block` - hide mobile, show tablet+

**Customization:**
```css
/* Override */
.btn-primary {
    background-color: #6366f1 !important;
}
```

---

### 15A. JavaScript Scope & Functions

**Scope:**
```javascript
// var - Function scope
function test() {
    if (true) {
        var x = 10;
    }
    console.log(x); // 10 (accessible)
}

// let - Block scope
function test() {
    if (true) {
        let y = 20;
    }
    console.log(y); // Error (not accessible)
}

// const - Cannot reassign
const PI = 3.14;
PI = 3.15; // Error
```

**Functions:**
```javascript
// Declaration (hoisted)
sayHi(); // Works
function sayHi() {}

// Expression (not hoisted)
sayHi(); // Error
const sayHi = function() {}

// Arrow
const add = (a, b) => a + b;

// Event handler
btn.addEventListener('click', () => {
    console.log('Clicked');
});
```

**Best Practice:** Use `const` default, `let` if needed, avoid `var`

---

### 15B. Todo List with localStorage

**HTML:**
```html
<input id="todoInput" type="text">
<button id="addBtn">Add</button>
<ul id="todoList"></ul>
```

**JavaScript:**
```javascript
let todos = JSON.parse(localStorage.getItem('todos')) || [];

// Add
function addTodo() {
    const text = document.querySelector('#todoInput').value;
    const todo = {
        id: Date.now(),
        text: text,
        completed: false
    };
    todos.push(todo);
    localStorage.setItem('todos', JSON.stringify(todos));
    renderTodos();
}

// Render
function renderTodos() {
    const list = document.querySelector('#todoList');
    list.innerHTML = ''; // Clear
    
    todos.forEach(todo => {
        const li = document.createElement('li');
        li.innerHTML = `
            <input type="checkbox" ${todo.completed ? 'checked' : ''} 
                   onclick="toggleTodo(${todo.id})">
            <span>${todo.text}</span>
            <button onclick="deleteTodo(${todo.id})">Delete</button>
        `;
        list.appendChild(li);
    });
}

// Toggle
function toggleTodo(id) {
    todos = todos.map(t => 
        t.id === id ? {...t, completed: !t.completed} : t
    );
    localStorage.setItem('todos', JSON.stringify(todos));
    renderTodos();
}

// Delete
function deleteTodo(id) {
    todos = todos.filter(t => t.id !== id);
    localStorage.setItem('todos', JSON.stringify(todos));
    renderTodos();
}

// Event delegation (better)
document.querySelector('#todoList').addEventListener('click', (e) => {
    if (e.target.tagName === 'BUTTON') {
        deleteTodo(e.target.dataset.id);
    }
});

// Load on start
renderTodos();
```

**Security:**
- ❌ `innerHTML` - XSS risk if user data
- ✅ `textContent` - Safe (text only)
- ✅ `insertAdjacentHTML` - Modern alternative

---

## PART-C (20 MARKS)

### 16A. MERN Stack Detailed

**Architecture:**
```
┌──────────────────────┐
│   REACT (Frontend)   │
│   - Components       │
│   - State mgmt       │
└──────────┬───────────┘
           │ Axios/Fetch
           ↓
┌──────────────────────┐
│ EXPRESS.js (Backend) │
│   - Routes           │
│   - Middleware       │
└──────────┬───────────┘
           │ Mongoose
           ↓
┌──────────────────────┐
│ MONGODB (Database)   │
│   - Collections      │
│   - Documents        │
└──────────────────────┘
```

**Data Flow:**
1. User clicks button (React)
2. HTTP request → Backend (Express)
3. Query database (MongoDB)
4. Return JSON → Frontend
5. Update UI (React)

**vs MEAN:** Angular instead of React  
**vs Django:** Python vs JavaScript

**Chat App Setup:**

**Backend (server.js):**
```javascript
const express = require('express');
const mongoose = require('mongoose');
const http = require('http');
const socketio = require('socket.io');

const app = express();
const server = http.createServer(app);
const io = socketio(server);

// MongoDB
mongoose.connect('mongodb://localhost/chat');

// Message model
const Message = mongoose.model('Message', {
    user: String,
    text: String,
    timestamp: Date
});

// Socket.io
io.on('connection', (socket) => {
    console.log('User connected');
    
    // Send message
    socket.on('sendMessage', async (data) => {
        const msg = await Message.create(data);
        io.emit('newMessage', msg); // Broadcast
    });
    
    socket.on('disconnect', () => {
        console.log('User disconnected');
    });
});

server.listen(5000);
```

**Frontend (React):**
```javascript
import io from 'socket.io-client';
import { useState, useEffect } from 'react';

const socket = io('http://localhost:5000');

function Chat() {
    const [messages, setMessages] = useState([]);
    const [input, setInput] = useState('');
    
    useEffect(() => {
        socket.on('newMessage', (msg) => {
            setMessages([...messages, msg]);
        });
    }, [messages]);
    
    const sendMessage = () => {
        socket.emit('sendMessage', {
            user: 'Ram',
            text: input,
            timestamp: new Date()
        });
        setInput('');
    };
    
    return (
        <div>
            {messages.map(m => (
                <div key={m._id}>{m.user}: {m.text}</div>
            ))}
            <input value={input} onChange={e => setInput(e.target.value)} />
            <button onClick={sendMessage}>Send</button>
        </div>
    );
}
```

**Security:**
- JWT authentication
- Input validation
- CORS configuration
- Helmet.js middleware
- Rate limiting

**Performance:**
- MongoDB indexing
- React.memo for components
- Socket.io rooms
- Caching (Redis)

---

### 16B. Responsive Dashboard (Advanced)

**HTML:**
```html
<div class="dashboard">
    <header class="header">
        <button id="darkToggle">🌙</button>
        <nav role="navigation">
            <a href="#">Home</a>
        </nav>
    </header>
    
    <aside class="sidebar" aria-label="Main navigation">
        <a href="#" tabindex="0">Dashboard</a>
        <a href="#">Users</a>
    </aside>
    
    <main class="content">
        <div class="cards">
            <div class="card" role="article">
                <h2>Stats</h2>
                <p>1,234</p>
            </div>
        </div>
        
        <table role="table">
            <thead><tr><th>Name</th></tr></thead>
            <tbody><tr><td>Ram</td></tr></tbody>
        </table>
    </main>
</div>
```

**CSS (Grid + Flexbox):**
```css
:root {
    --bg: #ffffff;
    --text: #1a1a1a;
    --sidebar-bg: #2d3748;
}

[data-theme="dark"] {
    --bg: #1a1a1a;
    --text: #ffffff;
}

* { margin: 0; padding: 0; box-sizing: border-box; }

body {
    font-family: system-ui;
    background: var(--bg);
    color: var(--text);
    transition: background 0.3s;
}

/* Grid Layout */
.dashboard {
    display: grid;
    grid-template-areas:
        "header header"
        "sidebar content";
    grid-template-columns: 250px 1fr;
    grid-template-rows: 60px 1fr;
    min-height: 100vh;
}

.header {
    grid-area: header;
    background: var(--sidebar-bg);
    color: white;
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 0 20px;
}

.sidebar {
    grid-area: sidebar;
    background: var(--sidebar-bg);
    padding: 20px;
}

.sidebar a {
    display: block;
    color: #cbd5e0;
    padding: 10px;
    text-decoration: none;
    border-radius: 5px;
    margin-bottom: 5px;
}

.sidebar a:hover,
.sidebar a:focus {
    background: #4a5568;
    color: white;
    outline: 2px solid white;
}

.content {
    grid-area: content;
    padding: 20px;
}

/* Flexbox for cards */
.cards {
    display: flex;
    gap: 20px;
    flex-wrap: wrap;
    margin-bottom: 30px;
}

.card {
    flex: 1;
    min-width: 250px;
    padding: 20px;
    background: var(--bg);
    border: 1px solid #e2e8f0;
    border-radius: 8px;
    box-shadow: 0 2px 4px rgba(0,0,0,0.1);
}

/* Table */
table {
    width: 100%;
    border-collapse: collapse;
    background: var(--bg);
}

th, td {
    padding: 12px;
    text-align: left;
    border-bottom: 1px solid #e2e8f0;
}

/* Responsive */
@media (max-width: 768px) {
    .dashboard {
        grid-template-areas:
            "header"
            "content";
        grid-template-columns: 1fr;
        grid-template-rows: 60px 1fr;
    }
    
    .sidebar {
        display: none;
    }
    
    .cards {
        flex-direction: column;
    }
}

/* Accessibility - Focus states */
:focus {
    outline: 3px solid #4299e1;
    outline-offset: 2px;
}

/* Dark mode toggle */
#darkToggle {
    background: none;
    border: none;
    font-size: 24px;
    cursor: pointer;
}
```

**JavaScript (Dark Mode):**
```javascript
const toggle = document.querySelector('#darkToggle');
const theme = localStorage.getItem('theme') || 'light';

document.documentElement.setAttribute('data-theme', theme);

toggle.addEventListener('click', () => {
    const current = document.documentElement.getAttribute('data-theme');
    const newTheme = current === 'dark' ? 'light' : 'dark';
    
    document.documentElement.setAttribute('data-theme', newTheme);
    localStorage.setItem('theme', newTheme);
    
    toggle.textContent = newTheme === 'dark' ? '☀️' : '🌙';
});
```

**ARIA Labels:**
```html
<nav role="navigation" aria-label="Main">
<button aria-label="Toggle dark mode">
<table role="table" aria-labelledby="tableTitle">
```

**Performance:**
- CSS Grid (better than floats)
- Flexbox (efficient alignment)
- CSS variables (dynamic theming)
- Minimal JavaScript
- localStorage (persist theme)

---

## QUICK REVISION

**MERN:**
- M = MongoDB (DB)
- E = Express (Backend)
- R = React (Frontend)
- N = Node.js (Runtime)

**CSS:**
- Box Model: Content → Padding → Border → Margin
- Flexbox: 1D (navbar)
- Grid: 2D (dashboard)

**JavaScript:**
- Use `const` default
- `let` for reassignment
- Avoid `var`
- Arrow functions in React

**Responsive:**
- Mobile-first: `min-width`
- Desktop-first: `max-width`
- Use `rem`, `clamp()`

**Bootstrap:**
- Utility: `mb-3`, `d-flex`
- Components: navbar, card, modal
- Override: `!important` or Sass

**Accessibility:**
- Contrast: 4.5:1
- ARIA labels
- Keyboard navigation
- Focus states

---

## EXAM TIPS

1. **Diagrams:** Draw architecture, box model
2. **Code:** Short, clean, comments
3. **Examples:** Real-world (Amazon, WhatsApp)
4. **Compare:** Always use tables
5. **Keywords:** Bold important terms

**All the best! 💻**
