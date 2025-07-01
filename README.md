Rooky Bunker is a open-source platform designed to support players in studying, annotating, and organizing their chess games. With an intuitive interface and powerful features, it’s the perfect tool for players who want to track progress, build repertoires, and explore games from major platforms. ♟️
---

## 🚀 Features

✅ **Decentralized & Secure:** Powered by Rust, Yew, and Nostr for speed, security, and resilience.  
✅ **Interactive UI:** Styled with TailwindCSS for a sleek and modern interface.
✅ **Efficient Testing:** Ensured reliability with Rust’s built-in testing framework.

### App Pages

Rooky Bunker is organized into five primary pages, each serving a specific purpose for chess study and game management:

- **Home:** Displays the total number of games stored in the local database and games currently in the box. Also shows the user's public key and Npub.

- **Annotate:** Provides an interactive game analysis interface with a card on the left that logs each move made during the game and a chessboard on the right to visualize and play through the moves.

- **Repertoire:** Shows a table listing all previously played games.

- **Search:** Enables searching for games across external platforms like Lichess and Chess.com to study them.

- **Settings:** Offers key management options where users can view their cryptographic keys.

---

## 🛠 Tech Stack

Rooky Bunker is built using the latest web technologies to ensure performance and scalability:

- **🦀 Rust** - High-performance, memory-safe programming language [(Download Rust)](https://www.rust-lang.org/learn/get-started)
- **🌿 Yew** - Rust-based framework for building interactive web apps [(Yew Docs)](https://yew.rs/docs/)
- **⚡ Nostr** - Decentralized protocol for secure communication [(Nostr Protocol)](https://nostr.com/)
- **🎨 TailwindCSS** - Utility-first CSS framework for styling [(Tailwind Docs)](https://tailwindcss.com/docs)
- **🗺️ Leaflet** - Interactive maps and location services [(LeafletJS)](https://leafletjs.com/)

---

## 🏗 Project Architecture

Rooky follows a modular frontend architecture within each app directory. The main source code resides in the `src/` folder, which is organized as follows:

- `src/` – Main application source code.
- `components/` – Reusable UI components (buttons, forms, widgets, etc.).
- `contexts/` – Application-wide state management and shared logic.
- `pages/` – Top-level views and route handlers for the app.
- `Cargo.toml` – App-specific dependencies and metadata.
- `manifest.json` – Web app manifest for PWA support.
- `serviceWorker.js` – Enables offline functionality.
- `Trunk.toml` – Build configuration for Trunk.
- `build.rs` – Optional custom build scripts.

There is no centralized backend. All communication occurs via **Nostr** relays, and local data is stored in **IndexedDB**, ensuring a fully decentralized architecture.

---

## 🌐 How Rooky Uses Nostr

Fuente leverages **Nostr** as its primary communication protocol for a trustless and decentralized experience. 

### 🔗 Communication with Relays
- All messages, transactions, and interactions are sent via **Nostr relays**, removing the need for centralized servers.
- Each app (consumer, business, admin, etc.) subscribes to specific events in the network, ensuring seamless interaction.

### 🔑 Authentication
- Users authenticate using **Nostr public/private keys** instead of traditional logins.
- Private keys are securely stored on the client-side, never exposing them to third parties.

### 📦 Data Storage
- No centralized database is used. Instead, **IndexedDB** is leveraged for local storage.
- Users retain control over their data, which can be synchronized across devices via Nostr relays.

Using **Nostr** ensures Rooky remains **censorship-resistant**, **fault-tolerant**, and **decentralized**, making it an ideal solution for borderless commerce.

---

## 🔗 Useful Links

- 📜 Official Rust Docs: [Rust Documentation](https://doc.rust-lang.org/)
- 🔧 Trunk Guide: [Trunk Docs](https://trunkrs.dev/)
- 🖥️ Yew Framework: [Yew Documentation](https://yew.rs/docs/)
- 🔑 Nostr Protocol: [Nostr](https://nostr.com/)
- 🎨 TailwindCSS: [Tailwind Docs](https://tailwindcss.com/docs)