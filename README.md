# ⚡ ParkEV

> Smart parking discovery, spot booking, and EV route planning — all in one platform.

![JavaScript](https://img.shields.io/badge/JavaScript-Vanilla-F7DC6F?style=flat&logo=javascript&logoColor=black)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-v3-38BDF8?style=flat&logo=tailwindcss&logoColor=white)
![License](https://img.shields.io/badge/license-MIT-green?style=flat)
![Status](https://img.shields.io/badge/status-prototype-orange?style=flat)

ParkEV is a frontend prototype that addresses real-world urban challenges: finding parking in congested cities and planning trips around EV charging constraints. It simulates a full ecosystem — peer-to-peer spot listings, time-slot booking, wallet-based billing, and AI-powered journey planning.

---

## ✨ Features

| Feature | Description |
|---|---|
| **Auth System** | Secure login for users and admins with role-based access control |
| **Dashboard** | Search and browse nearby parking spots with live availability |
| **P2P Listings** | Users list their spaces; admins review and approve before going live |
| **Booking System** | Time-slot selection with smart queue handling when spots are full |
| **Wallet System** | Minimum balance enforcement, billing approval, and simulated payments |
| **JourneyIQ** | EV range planner that maps charging stops along your route |
| **Session Management** | Start/end sessions with image proof upload and billing flow |
| **Profile & Rewards** | User profiles with a rewards system for frequent parkers |

---

## ⚙️ Tech Stack

- **JavaScript** — Vanilla, no frameworks or bundlers
- **Tailwind CSS** — Utility-first styling
- **HTML5** — Semantic markup

---

## 🚀 Getting Started

```bash
# Clone the repository
git clone https://github.com/your-username/ParkEV.git

# Navigate into the project
cd ParkEV
```

Open `index.html` in your browser — no build step, no installs, no config needed.

> **Tip:** Use a local server like [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) for the best experience.

---

## 📁 Project Structure

```
ParkEV/
├── index.html          # Entry point
├── assets/
│   ├── css/            # Tailwind output / custom styles
│   └── images/         # Icons and static assets
├── pages/
│   ├── dashboard.html
│   ├── booking.html
│   ├── profile.html
│   └── journey.html    # JourneyIQ route planner
└── js/
    ├── auth.js
    ├── booking.js
    ├── wallet.js
    └── journey.js
```

> Adjust the structure above to match your actual project layout.

---

## 🧠 How It Works

### Booking Flow
1. User searches for a parking spot by location and time
2. Available slots are displayed with pricing
3. User selects a slot — wallet balance is checked
4. Booking is confirmed or added to the queue if full
5. Session starts/ends with image proof; billing is approved

### P2P Listing Flow
1. User submits a parking space with details and availability
2. Admin reviews the listing on the admin dashboard
3. Approved listings go live and become bookable

### JourneyIQ (EV Route Planner)
1. User enters start/end destination and current battery level
2. JourneyIQ calculates if the trip is within range
3. If not, charging stops are suggested along the route

---

## 📚 What I Learned

- Designing end-to-end user flows for two-sided platforms — balancing user needs with admin oversight across listing, booking, and session management
- Implementing booking logic with time slots and a queue system to handle concurrency and over-demand gracefully
- Structuring wallet-based transactions with minimum balance rules and simulated billing approval cycles
- Building scalable, maintainable UI components with Tailwind CSS in a no-framework environment
- Modeling domain-specific logic for EV ecosystems — range constraints, charging stops, and journey planning

---

## 🔮 Roadmap

- [ ] Map integration (Google Maps / Leaflet) for visual spot discovery
- [ ] Real-time availability with WebSockets
- [ ] Mobile-responsive improvements
- [ ] Backend integration (Node.js + database)
- [ ] Push notifications for booking confirmations

---

## 🤝 Contributing

Contributions, issues, and feature requests are welcome!

1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## 📄 License

Distributed under the MIT License. See `LICENSE` for more information.

---

<p align="center">Built with ⚡ by <a href="https://github.com/your-username">your-username</a></p>
