# 🖨️ SmartPrint — Cloud Xerox Ecosystem
> Live submission for **Hack Devengers 2.0**

🔗 **Live Deployment:** [https://peaceful-licorice-b81700.netlify.app/](https://peaceful-licorice-b81700.netlify.app/)

---

## 📌 Problem Statement
Campus print shops face major bottlenecks during peak hours. Students lose valuable study time standing in physical queues, handing over USB drives, or dealing with loose cash. Shop owners struggle to manage unorganized queues, track document owners, and balance print jobs manually.

## 💡 Solution Overview
**SmartPrint** digitizes the campus printing workflow:
* **For Students:** Upload files (PDF/images), select print settings (B/W vs. Color, copy counts, Spiral vs. Tape binding), view a real-time price calculator, and pay via simulated UPI or choose counter cash payment.
* **For Shop Owners:** A live, prioritized print queue dashboard with one-click PDF viewing, native print spooling, order search, and individual job status tracking.

---

## ✨ Key Features & Innovations

1. **Dual-Portal Architecture:** Dedicated interfaces for students and copy-shop operators with role-specific authentication.
2. **Smart Priority Queue:** UPI-paid orders automatically jump ahead of cash-pending orders to incentivize digital payments and reduce shop crowd congestion.
3. **Dynamic Pricing Engine:** Calculates print costs (₹2 B/W, ₹10 Color) and binding add-ons (Tape at ₹20, Spiral at ₹20 for ≤40p or ₹40 for >40p) in real time.
4. **Automated UPI Verification Simulation:** Emulates merchant payment webhook callbacks with animated visual feedback and automatic Order ID generation.
5. **Hardware Auto-Spooling:** An operator-side print action that automatically launches the document print dialog without manual keyboard commands.
6. **Live Order Search:** Instant real-time filtering in the queue by Order ID for fast handovers.
7. **Client-Side Persistence:** Zero external database required for the demo—uses browser `localStorage` and `FileReader API` for persistent, offline-capable state.

---

## 🔑 Demo Credentials

| Role | Username | Password / PIN |
|---|---|---|
| **Student** | `ARJUN` (or `YUKESWAR`, `PRIYA`, `KAVYA`, `ROHIT`) | `1234` |
| **Operator / Admin** | `ADMIN` | `5678` |

---

## 🛠️ Tech Stack
* **Markup & Styling:** HTML5, Modern CSS3 (Skeuomorphic "Paper & Ink" theme, Dark/Light modes)
* **Logic:** Vanilla JavaScript (ES6+)
* **APIs & Storage:** HTML5 FileReader API, Web Storage API (`localStorage`)
* **Libraries:** `QRCode.js` (via CDN)
