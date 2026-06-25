# TELEGRAM_MINI_APP

## MODULE

Telegram Mini App

---

## PURPOSE

Define the Telegram Mini App structure, user entry flow, navigation, core screens, Telegram integration, and MVP behavior.

---

## PLATFORM

- Telegram Mini App
- Mobile First
- WebView
- Telegram Login
- Telegram Payments
- Telegram Sharing

---

## MVP SCREENS

1. Welcome
2. Login
3. Main Dashboard
4. Aircraft NF-001
5. Parts Catalog
6. Buy Part
7. User Profile
8. Team
9. Referral
10. Wallet
11. Progress
12. Notifications

---

## USER FLOW

1. User opens Telegram bot.
2. User clicks Open App.
3. App receives Telegram user data.
4. Backend verifies Telegram auth.
5. User profile is created or loaded.
6. User sees NF-001 dashboard.
7. User selects aircraft part.
8. User creates order.
9. User completes payment.
10. Part is assigned to user.
11. Aircraft progress is updated.
12. User sees contribution history.

---

## MAIN DASHBOARD

Display:

- Aircraft name
- Aircraft progress
- Active users
- Current stage
- User contribution
- Team progress
- Main action button

Primary action:

- Build / Buy Part

---

## AIRCRAFT SCREEN

Display:

- Aircraft ID
- Progress %
- Aircraft zones
- Available parts
- Completed parts
- User-owned parts

Actions:

- Select zone
- View parts
- Buy part
- View history

---

## PARTS CATALOG

Display:

- Part name
- Category
- Price
- Quantity
- Aircraft zone
- Availability

Actions:

- Buy
- View details
- Add to team progress

---

## PAYMENT FLOW

1. User selects product.
2. App creates order.
3. Payment request is sent.
4. Payment is confirmed.
5. Transaction is saved.
6. Part is assigned.
7. Progress is updated.

---

## PROFILE

Display:

- Telegram ID
- Username
- Level
- Status
- Owned parts
- Contribution history
- Team
- Referral link

---

## TEAM

Functions:

- Create team
- Join team
- View members
- View team progress
- View team ranking

---

## REFERRAL

Functions:

- Generate referral link
- Track invited users
- Show referral rewards
- Show referral statistics

---

## WALLET

Display:

- Balance
- Payments
- Transactions
- Rewards
- Refunds

---

## NOTIFICATIONS

Types:

- Purchase confirmed
- Aircraft progress updated
- Team event
- Referral joined
- New part available
- First flight event

---

## TELEGRAM INTEGRATIONS

- Telegram Login
- Telegram Bot
- Telegram Mini App SDK
- Telegram Payments
- Telegram Share Links
- Telegram Notifications

---

## API DEPENDENCIES

- Auth API
- User API
- Aircraft API
- Parts API
- Payment API
- Wallet API
- Team API
- Referral API
- Notification API

---

## DATABASE DEPENDENCIES

- Users
- Aircraft
- Parts
- Orders
- Payments
- Transactions
- Teams
- Referrals
- Wallets
- Notifications

---

## ADMIN DEPENDENCIES

- Manage users
- Manage aircraft
- Manage parts
- Manage payments
- Manage teams
- Manage notifications

---

## MVP LIMITS

- One aircraft: NF-001
- One main catalog
- Basic payments
- Basic profile
- Basic team system
- Basic referral system
- Basic admin control

---

## FUTURE

- Multiple aircraft
- Advanced teams
- Country rankings
- Marketplace
- Academy
- Museum
- Aircraft biography
- Corporate accounts

---

## STATUS

Draft v1.0
