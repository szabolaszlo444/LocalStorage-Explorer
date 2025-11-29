# LocalStorage-Explorer (LSE)

A lightweight, reactive LocalStorage development tool for web developers.

---

## 🚀 Overview

LocalStorage Explorer (LSE) is a **standalone, Vanilla JS tool** that lets developers **view, edit, and manage browser LocalStorage in real-time**.

Perfect for frontend developers and QA engineers who want to quickly inspect or modify app data **without any frameworks**.

---

## 🤔 Why LSE?

While browser developer tools offer a way to view LocalStorage, they often lack reactivity and user-friendly editing features. LSE solves this by providing:

- **A Reactive UI:** No more manual refreshing. Changes made in your app or another tab are reflected instantly.
- **Superior JSON Handling:** The built-in DevTools are clumsy for editing complex JSON. LSE offers a dedicated editor with syntax highlighting and formatting.
- **A Dedicated Workspace:** Keep LSE open in its own tab for a persistent, clear view of your storage, separate from the clutter of other DevTools panels.

---

## ✨ Features

- **Reactive UI** – automatically updates keys and editor when LocalStorage changes
- **JSON editor & prettify** – easily read and edit JSON-formatted values
- **Search / Filter keys** – quickly locate the key you need
- **Save / New / Delete / Clear** – fully manage LocalStorage
- **Storage event listener** – updates if LocalStorage changes in another tab
- **Standalone HTML file** – can be used as a bookmarklet or opened in any browser tab
- **Export / Import JSON** – save all keys to a file or load from a file
- **Dark Mode** – toggle dark mode for comfortable viewing

---

## 🛠️ Technology Stack

LSE is built with simplicity in mind.

- **Vanilla JavaScript (ES6+):** No frameworks, no libraries, no dependencies.
- **HTML5 & CSS3:** Clean, semantic markup and modern styling.
- **No Build Step:** Just a single HTML file you can use immediately.

---

## ⚙️ How It Works

The core of LSE's reactivity is the browser's native `StorageEvent`. The tool listens for this event, which fires whenever a storage item is changed in the same origin from another document (like your app running in a different tab). When an event is detected, the UI automatically updates to reflect the new state of the LocalStorage.

## 💻 Installation & Usage (HTML file)

The LocalStorage Explorer is designed to be used as a **standalone HTML file**. No build tools or frameworks are required.

### 1️⃣ Place the file in your project

- Copy `localstorage-explorer.html` into your project folder.
- Example for **Vue**:

```text
my-vue-project/
├─ public/
│  └─ localstorage-explorer.html
└─ src/
```

- Example for **React**: place it in the `public/` folder or any folder served by the dev server.

### 2️⃣ Run the Explorer

1. Start your **development server**:

npm run dev

# or

yarn dev

Open a new tab and navigate to the LocalStorage Explorer file:

`http://localhost:5173/localstorage-explorer.html`

The Explorer will load all LocalStorage entries for the current origin.

You can now view, edit, delete, or create keys, and the UI updates in real-time.

### 3️⃣ Additional Features

- **Export / Import JSON:**

  - Export LocalStorage data as a `.json` file.
  - Import a `.json` file to restore or preload LocalStorage.

- **Dark Mode:**
  - Toggle dark mode directly in the Explorer for comfortable viewing in low-light environments.

### 🔧 Examples

- **Create a new key:** Enter a key name and value → Save New
- **Edit an existing key:** Click a key → modify value → Save
- **Delete a key:** Select a key → Delete
- **Clear all keys:** Clear All → confirm deletion
- **Search:** Type a key or substring in the search field → only matching keys appear

### 📌 Notes

- LocalStorage is origin-specific: you only see the keys for the current domain.
- Keep two tabs open in your dev environment: one for your app, one for the Explorer. Changes in your app reflect immediately.

### ⚡ Future Improvements

- **Nested JSON Editor:** A tree-view editor for complex, multi-level JSON objects.
- **Drag & Drop Key Reordering:** Allow reordering keys in the list via drag and drop.
- **Theme Support:** Introduce multiple themes beyond the default light/dark modes.
- **Fully Offline Bookmarklet Version:** A self-contained bookmarklet that can be injected into any page without needing the HTML file.
- **SessionStorage Support:** Add a toggle to switch between managing LocalStorage and SessionStorage.

---

## 🌐 Browser Compatibility

This tool is tested and works on the latest versions of all modern desktop browsers:

- Google Chrome
- Mozilla Firefox
- Apple Safari
- Microsoft Edge

---

## 🤝 Contributing

Contributions are welcome! Whether it's a bug report, feature request, or a pull request, we appreciate your help.

**Bug Reports & Feature Requests**

Please open an issue on GitHub and provide a detailed description of the bug or feature. For bugs, include steps to reproduce, the expected behavior, and the actual behavior.

**Pull Requests**

1.  Fork the repository.
2.  Create your feature branch (`git checkout -b feature/AmazingFeature`).
3.  Commit your changes (`git commit -m 'Add some AmazingFeature'`).
4.  Push to the branch (`git push origin feature/AmazingFeature`).
5.  Open a Pull Request.

---

## ❓ FAQ

**Q: Why don't I see any keys when I open the file?**
**A:** LocalStorage is origin-specific. Make sure you are running the `localstorage-explorer.html` file from the same origin (e.g., `http://localhost:5173`) as your application. Opening the HTML file directly from your filesystem (`file:///...`) will only show keys for that local file path.

### 📝 License

MIT License – free to use, modify, and distribute

---

## ✉️ Contact

For questions or support, please open an issue on the project's GitHub repository.

```

```
