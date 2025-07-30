# Custom Productivity Homepage

This project is a **custom-built productivity dashboard** designed to serve as your browser's personal start page. Built with pure HTML, CSS, and JavaScript, it offers a clean, modern, and interactive interface focused on maximizing daily productivity—combining fast access to tools, task managers, notes, Pomodoro timer, and inspiration all in one place.

---

## Overview

This homepage provides a productive, user-centered dashboard with dedicated panels for **quick links**, **deadlines**, a **live clock and dynamic greeting**, **to-do manager**, **Pomodoro timer**, **notes scratchpad**, and **rotating motivational quotes**.

- **Modern dark theme** with accent colors.
- Fully **responsive layout** via CSS Grid and media queries.
- **All features work offline**, data is private (stored in your browser).
- **Single HTML file**—no dependencies besides Google Fonts.

---

## Sections and Features

### 1. Global Styles and Layout

**CSS Root Variables**
- All main colors, typography, border-radius, and transitions are managed through `:root` variables:
  - `--bg`, `--accent`, `--card-bg`, `--text`, `--muted`
- **Key feature:** Create and test your own color theme by modifying just 3-4 variables—no need to touch the whole CSS for theming.

**Body and Container**
- Gradient background smoothly transitions from deep indigo to blue, with orange and white at the edges.
- Main layout: `display: grid; grid-template-columns: 1fr 1.5fr 1fr;` (three columns).

**Cards**
- Content blocks use a dark blue background, subtle shadow, rounded corners, and padding.
- **Visual feedback:** Hover effect increases shadow depth.

**Responsive Design**
- At widths below 900px, layout automatically switches to single column for mobile-friendly usability.

---

### 2. Left Sidebar

**Quick Links**
- A grid of buttons linking to core tools: Email, Scholar, Notes, Calendar, Calculator, and Dictionary.
- Consistent visual design and clear hover states.

**Deadlines Card**
- Add a task and attach a due date using a text input and date picker.
- All deadlines listed below (sorted by soonest date), showing:
  - Task name and **date formatted as DD-MM** (year hidden).
  - **Dynamic status**: Days left (gray), Today (blue), Overdue (red).
  - One-click delete button for each entry.
- All deadlines **persist in localStorage**, updated live as you add/delete.
- Inputs use flex to keep the task field big and date/button compact.

---

### 3. Center Panel

**Clock and Greeting**
- Large, live-updating digital clock (24-hour).
- Shows current date (weekday, month, day, year).
- **Greeting** updates by time of day: morning, afternoon, or evening.

**Today's Focus**
- Input field to type your main goal/focus of the day.
- Automatically saved to localStorage and restored each session.

**To-Do List**
- Add tasks quickly; mark them as done (✓ button) to remove.
- Easily clear all with a dedicated trash icon.
- Tasks persist in localStorage until removed.

**Pomodoro Timer**
- Classic Pomodoro (25 min) timer with Start, Pause, and Reset.
- Sounds an alert when finished.
- Quick visual at-a-glance and manual controls for productivity sessions.

---

### 4. Right Sidebar

**Notes**
- A textarea for ad-hoc notes and ideas.
- Instant local save as you type; restored on reload.

**Motivational Quotes**
- Displays a random quote from a selected list of Naval Ravikant insights.
- Rotates every hour to keep inspiration fresh.

---

### 5. JavaScript Functionality

- **Live clock** and greeting with `setInterval`.
- **LocalStorage** for all persistence (to-dos, deadlines, focus, notes).
- **Deadline management**: Sorted display, color-coded status, DD-MM format.
- **Dynamic updates**: DOM rendering for all main lists/blocks.
- **Keyboard accessibility**: Add entries with Enter; buttons have titles/tooltips.
- **Responsive updates**: Layout and content adapt instantly.
- **Timer logic**: Simple countdown with notification.
- **Quote rotation**: Picks and shows a new quote hourly.

---

### 6. Accessibility and User Experience

- Semantic HTML and clear headings.
- Button tooltips for clarity (e.g., delete, clear).
- Visual feedback with color and shadow cues.
- Keyboard input works for major actions (Enter to add tasks/deadlines).
- Mobile-friendly grid collapse.

---

## How to Use

1. **Open the homepage** in any modern browser (`index.html`).
2. Use **Quick Links** panel for instant access to commonly used web tools.
3. **Add deadlines** for important tasks—track how soon or late you are.
4. Set your **focus** for the day.
5. Manage your **to-dos**: add, mark complete, or clear all.
6. Use the **Pomodoro timer** for focused work sessions.
7. **Jot notes** and let your ideas flow with persistent storage.
8. Stay inspired with **rotating quotes** in the sidebar.

---

## Customization

- Easily swap fonts and colors through the `:root` CSS variables.
- Edit/add Quick Links by changing `.links-grid` in HTML.
- Change or add quotes by editing the JavaScript `quotes` array.
- Tweak spacing/layout by changing grid column settings in CSS.

---

## Project Structure

root/
└── index.html # All code: HTML structure, CSS in <style>, JS in <script>



---

## License

Open for personal use, learning, and adaptation. No backend, no tracking—just your data in your browser.

---

Enjoy your streamlined, focused, and inspiring new home page!
---

## Summary

This homepage brings together a suite of productivity and wellness tools in a clean, single-html-file UI:

- **Everything is modular, persistent, and instantly responsive.**
- **Cards:** All content widgets (deadlines, notes, todos, focus, quotes, timer) are organized as movable, visually separated cards for clear mental boundaries.
- **No backend or tracking:** All your data (tasks, notes, deadlines, focus) is private, living 100% in your browser via localStorage.
- **Live updating:** Time, greeting, quotes, and all panels update instantly without reloading. Keyboard shortcuts (Enter for add) and tooltips streamline your flow.
- **Customizable look and feel:** Change the visual theme or function by simply modifying color/font variables in the CSS root section or adjusting the quick links, layout, or quotes in the html/js.

This homepage offers a unified, beautiful productivity launchpad for daily organization, deep work, and motivation, designed for maximum flexibility and ease of use.

Give it a try—just open `index.html` in your browser and make the dashboard your own!
