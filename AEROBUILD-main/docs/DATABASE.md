# DATABASE

## MODULE

Database

---

## PURPOSE

Define the database structure for users, aircraft, parts, payments, teams, referrals, wallet operations, notifications, and admin control.

---

## DATABASE ENGINE

PostgreSQL

---

## CORE TABLES

- users
- aircraft
- aircraft_zones
- parts
- user_parts
- orders
- payments
- transactions
- wallets
- teams
- team_members
- referrals
- notifications
- admin_users
- audit_logs

---

## USERS

Fields:

- id
- telegram_id
- username
- first_name
- last_name
- language
- country
- level
- status
- created_at
- updated_at

---

## AIRCRAFT

Fields:

- id
- code
- name
- status
- progress_percent
- start_date
- first_flight_date
- created_at
- updated_at

---

## AIRCRAFT_ZONES

Fields:

- id
- aircraft_id
- name
- progress_percent
- status
- created_at
- updated_at

---

## PARTS

Fields:

- id
- aircraft_id
- zone_id
- name
- category
- price
- currency
- quantity_total
- quantity_available
- progress_value
- status
- created_at
- updated_at

---

## USER_PARTS

Fields:

- id
- user_id
- part_id
- aircraft_id
- order_id
- quantity
- created_at

---

## ORDERS

Fields:

- id
- user_id
- total_amount
- currency
- status
- payment_method
- created_at
- updated_at

---

## PAYMENTS

Fields:

- id
- order_id
- user_id
- provider
- provider_payment_id
- amount
- currency
- status
- created_at
- updated_at

---

## TRANSACTIONS

Fields:

- id
- user_id
- order_id
- payment_id
- type
- amount
- currency
- status
- created_at

---

## WALLETS

Fields:

- id
- user_id
- balance
- currency
- created_at
- updated_at

---

## TEAMS

Fields:

- id
- name
- owner_user_id
- country
- progress_score
- created_at
- updated_at

---

## TEAM_MEMBERS

Fields:

- id
- team_id
- user_id
- role
- joined_at

---

## REFERRALS

Fields:

- id
- referrer_user_id
- invited_user_id
- referral_code
- reward_status
- created_at

---

## NOTIFICATIONS

Fields:

- id
- user_id
- type
- title
- message
- status
- created_at
- read_at

---

## ADMIN_USERS

Fields:

- id
- user_id
- role
- permissions
- created_at

---

## AUDIT_LOGS

Fields:

- id
- admin_user_id
- action
- entity_type
- entity_id
- payload
- created_at

---

## RELATIONS

- user has one wallet
- user has many orders
- user has many transactions
- user has many user_parts
- aircraft has many zones
- aircraft has many parts
- part belongs to aircraft
- part belongs to aircraft_zone
- order has many payments
- payment belongs to order
- team has many members
- user can belong to many teams
- referral connects referrer and invited user

---

## INDEXES

- users.telegram_id
- aircraft.code
- parts.aircraft_id
- parts.zone_id
- orders.user_id
- payments.order_id
- transactions.user_id
- teams.country
- referrals.referral_code

---

## SECURITY

- Store payment provider IDs.
- Do not store raw card data.
- Use audit logs for admin actions.
- Use role-based access control.
- Backup database daily.

---

## STATUS

Draft v1.0
