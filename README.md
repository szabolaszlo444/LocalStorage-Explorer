# LocalStorage-Explorer (LSE)

A lightweight, reactive LocalStorage development tool for web developers.

🚀 Overview

LocalStorage Explorer (LSE) is a standalone, Vanilla JS tool that lets developers view, edit, and manage browser LocalStorage in real-time.

Perfect for frontend developers and QA engineers who want to quickly inspect or modify app data without any frameworks.

✨ Features

Reactive UI – automatically updates keys and editor when LocalStorage changes

JSON editor & prettify – easily read and edit JSON-formatted values

Search / Filter keys – quickly locate the key you need

Save / New / Delete / Clear – fully manage LocalStorage

Storage event listener – updates if LocalStorage changes in another tab

Standalone HTML file – can be used as a bookmarklet or opened in any browser tab

Export / Import JSON – save all keys to a file or load from a file

Dark Mode – toggle dark mode for comfortable viewing

💻 Installation & Usage (HTML file)

The LocalStorage Explorer is designed to be used as a standalone HTML file. No build tools or frameworks are required.

1️⃣ Place the file in your project

Copy localstorage-explorer.html into your project folder.

Example for Vue:

my-vue-project/
├─ public/
│  └─ localstorage-explorer.html
└─ src/


Example for React: place it in the public/ folder or any folder served by the dev server.

2️⃣ Run the Explorer

Start your development server:

npm run dev
# or
yarn dev


Open a new tab and navigate to the LocalStorage Explorer file:

http://localhost:5173/localstorage-explorer.html


The Explorer will load all LocalStorage entries for the current origin.

You can view, edit, delete, or create keys, and the UI updates in real-time.

3️⃣ Additional Features

Export / Import JSON:

Export LocalStorage data as a .json file.

Import a .json file to restore or preload LocalStorage.

Dark Mode:

Toggle dark mode directly in the Explorer for comfortable viewing in low-light environments.

🔧 Examples

Create a new key: Enter a key name and value → Save New

Edit an existing key: Click a key → modify value → Save

Delete a key: Select a key → Delete

Clear all keys: Clear All → confirm deletion

Search: Type a key or substring in the search field → only matching keys appear

📌 Notes

LocalStorage is origin-specific: you only see the keys for the current domain.

You can keep two tabs open in your dev environment: one for your app, one for the Explorer. Changes in your app reflect immediately.

⚡ Future Improvements

Nested JSON editor (multi-level editing)

Drag & drop key reordering

Theme support (multiple themes / dark mode presets)

Fully offline bookmarklet version

📝 License

MIT License – free to use, modify, and distribute
