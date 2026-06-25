# DATABASE

## MODULE

Database

---

## PURPOSE

Define the complete database structure for the AEROBUILD platform.

---

## DATABASE ENGINE

PostgreSQL

---

## TABLES

Users

Profiles

Aircraft

AircraftParts

Products

Orders

Payments

Transactions

Wallets

Teams

TeamMembers

Referrals

Achievements

Levels

Inventory

Notifications

Sessions

AdminUsers

AuditLogs

Countries

Leaderboard

Campaigns

Settings

---

## USERS

Fields

- id
- telegram_id
- username
- first_name
- last_name
- language
- country
- avatar
- level_id
- reputation
- created_at
- updated_at
- status

---

## AIRCRAFT

Fields

- id
- code
- name
- model
- status
- progress
- launch_date
- completed_date

---

## AIRCRAFT PARTS

Fields

- id
- aircraft_id
- category
- name
- quantity
- installed
- progress
- price
- status

---

## PRODUCTS

Fields

- id
- name
- category
- aircraft_part_id
- price
- currency
- stock
- active

---

## ORDERS

Fields

- id
- user_id
- total
- currency
- payment_status
- created_at

---

## PAYMENTS

Fields

- id
- order_id
- provider
- transaction_id
- amount
- currency
- status
- created_at

---

## TRANSACTIONS

Fields

- id
- user_id
- payment_id
- product_id
- amount
- created_at

---

## WALLETS

Fields

- id
- user_id
- balance
- bonus_balance
- updated_at

---

## TEAMS

Fields

- id
- name
- country
- owner_id
- members
- progress

---

## TEAM MEMBERS

Fields

- id
- team_id
- user_id
- role
- joined_at

---

## REFERRALS

Fields

- id
- inviter_id
- invited_id
- reward
- created_at

---

## ACHIEVEMENTS

Fields

- id
- name
- description
- icon
- points

---

## INVENTORY

Fields

- id
- user_id
- product_id
- quantity

---

## COUNTRIES

Fields

- id
- name
- iso
- users
- teams
- progress

---

## LEADERBOARD

Fields

- id
- type
- object_id
- score
- position

---

## SETTINGS

Global configuration values.

---

## RELATIONS

User → Wallet

User → Orders

User → Transactions

User → Team

Aircraft → AircraftParts

AircraftParts → Products

Order → Payments

Order → Transactions

Country → Teams

Team → Members

User → Inventory

---

## INDEXES

telegram_id

username

country

aircraft_id

team_id

order_id

payment_id

created_at

---

## SECURITY

Encrypted sensitive data

Role-based access

Audit logging

Backups

---

## STATUS

Draft v1.0
