# Monster Kanban Board

Welcome to the Monster Kanban Board!

This project is designed to teach beginners the basics of:

- React components

- Passing props

- Using useState

- Drag and drop

- Tailwind CSS styling

- Fun interactive UI (monsters following your mouse 👀)

Anyone can fork this and learn step‑by‑step.

---

📌 1. How to Fork This Project

1. Go to the GitHub repo page.

2. Click the Fork button (top‑right).

3. Choose your GitHub account.

4. GitHub will create your own copy of the repo!

Now you can edit, experiment, and push changes without affecting the original.

---

🛠️ 2. How to Run the Project Locally

After forking:

1. Clone your fork to your computer:

   git clone <https://github.com/YOUR-USERNAME/monster-kanban.git>

2. Go into the project folder:

   cd monster-kanban

3. Install dependencies:

   npm install

4. Start the development server:

   npm start

Your browser will open automatically at:

    http://localhost:3000

---

📂 3. Project Structure (Beginner Friendly Explanation)

This project was intentionally built in a simple, understandable way.

    monster-kanban/
    ├── src/
    │   ├── App.jsx
    │   ├── index.js
    │   ├── index.css
    │   └── components/
    │       ├── KanbanBoard.jsx
    │       ├── Column.jsx
    │       ├── Task.jsx
    │       └── Monster.jsx
    ├── tailwind.config.js
    ├── postcss.config.js
    ├── package.json
    └── README.md

Now let’s explain every file in easy terms.

---

📌 /src/App.jsx — The App Root

This is the main component of the whole app.

It’s the “entry point” for your UI.

It:

- Sets the background

- Displays the title

- Renders the entire Kanban board

Think of it as the “stage” where everything else is placed.

---

📌 /src/index.js — React Entry File

This file tells React where to place your app in the HTML page.

It mounts <App /> into the DOM:

    root.render(<App />);

You almost never edit this as a beginner.

---

📌 /src/index.css — Tailwind Setup

This file activates Tailwind CSS in your project:

    @tailwind base;
    @tailwind components;
    @tailwind utilities;

This gives you all the Tailwind utility classes used in the UI.

---

📦 Inside the Components Folder

Every UI piece is a small reusable component.

---

👾 /components/Monster.jsx

This creates the little monsters above each column.

They have:

- A body (color + height)

- Two eyes

- Pupils that follow the mouse

(using useEffect, useRef, and some simple math)

This teaches:

- refs

- event listeners

- DOM measurements

---

📋 /components/KanbanBoard.jsx

This is the brain of the app.

It stores the full Kanban board state:

    backlog: [...]
    doing: [...]
    review: [...]
    done: [...]

It also contains functions to:

- Add tasks

- Remove tasks

- Move tasks between columns

Then it renders four <Column /> components, one for each section.

Beginners learn:

- useState

- How state updates work

- Passing functions down as props

---

📌 /components/Column.jsx

Each Kanban column (Backlog, Doing, Review, Done) is created by this component.

It handles:

- Showing the column name

- Listing tasks

- A little box to add new tasks

- Accepting dragged tasks

- Rendering the monster above the column

Beginners learn:

- Controlled inputs (value + onChange)

- Component props

- Handling events (onDrop, onDragOver)

---

📝 /components/Task.jsx

Represents one task card.

It:

- Shows the task text

- Can be dragged between columns

- Has a ✖ remove button

Beginners learn:

- How draggable elements work

- Passing data through drag events

- Event handlers

---

⚙️ /tailwind.config.js

This file tells Tailwind which files to scan for class names.

We include everything in src/:

    content: ["./src/**/*.{js,jsx}"],

You rarely touch this as a beginner.

---

⚙️ /postcss.config.js

Used by Tailwind internally.

Beginners don’t need to edit this.

---

📦 /package.json

Lists project dependencies (React, Tailwind, etc.).

Also contains commands like:

    "start": "react-scripts start"

You don’t edit this manually unless you're adding libraries.

---

🧪 What Students Can Learn From This Project

This repo is perfect for teaching:

✔️ Components & Props

(your UI is built from small reusable blocks)

✔️ State Management (useState)

(tasks added, removed, moved around)

✔️ Handling User Input

(adding tasks inside a column)

✔️ Drag-and-Drop

(the simplest possible implementation!)

✔️ Tailwind CSS

(styling without writing CSS files)

✔️ DOM Refs & Effects

(monsters’ eyes follow the mouse)

✔️ Clean, readable beginner code

(each file has one clear purpose)

---

🎉 Final Message

This project is designed to be:

- Fun 👾

- Beginner-friendly 💡

- Easy to expand 🧱

- A great teaching tool 🎓

Fork it, explore, and make it your own!

Add new monsters, animations, or even user accounts — the sky’s the limit.
