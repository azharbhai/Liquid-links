# 🎯 Next Session Roadmap: Connected Logistics Flow

This plan outlines the priority workflow for our next session: linking the entire oil transport lifecycle into a single persistent data stream.

## 🔄 The "Order-to-Assignment" Chain

### 1. Phase: Order Initiation (Customer Portal)
- **Feature**: Build a "Request Shipment" card inside the Customer Portal.
- **Action**: Customer enters Origin, Destination, Cargo Class, and Volume (KL).
- **Outcome**: Order is created in a `PENDING_ADMIN_APPROVAL` state.

### 2. Phase: Strategic Pricing (Admin Command)
- **Feature**: A "Review & Price" queue in the Admin Logistics dashboard.
- **Action**: Admin reviews pending customer orders, sets a **Base Price**, and moves the order to `OPEN_FOR_BID`.
- **Outcome**: The load becomes visible to all qualified transporters.

### 3. Phase: Competitive Tendering (Transporter Hub)
- **Feature**: An "Open Tenders" feed for transporters.
- **Action**: Transporters see the Admin's base price and submit their bids relative to that price.
- **Outcome**: Bids are logged in real-time.

### 4. Phase: Load Assignment & Dispatch
- **Feature**: Winner Selection Engine.
- **Action**: Admin (or automated system) selects the optimal bidder and **Assigns the Load** to a specific truck in that transporter's registered fleet.
- **Outcome**: Order moves to `IN_TRANSIT`.

---
*Capture this file during the next session to begin implementation.*
