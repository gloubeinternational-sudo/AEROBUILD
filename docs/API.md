# API

## MODULE

API

---

## PURPOSE

Provide a secure, scalable, and versioned interface between the Telegram Mini App, Backend, Database, Admin Panel, and external services.

---

## API VERSION

v1

---

## AUTHENTICATION

- Telegram Login
- JWT Token
- Refresh Token
- Role Validation

---

## USER API

POST /auth/login

POST /auth/logout

GET /user/profile

PUT /user/profile

DELETE /user/account

---

## AIRCRAFT API

GET /aircraft

GET /aircraft/{id}

GET /aircraft/{id}/progress

GET /aircraft/{id}/parts

---

## PARTS API

GET /parts

GET /parts/{id}

POST /parts/buy

GET /parts/history

---

## PAYMENT API

POST /payment/create

POST /payment/confirm

POST /payment/refund

GET /payment/history

---

## WALLET API

GET /wallet

GET /wallet/history

POST /wallet/reward

---

## TEAM API

GET /teams

POST /teams/create

POST /teams/join

GET /teams/{id}

GET /teams/ranking

---

## REFERRAL API

GET /referral

POST /referral/create

GET /referral/statistics

---

## ADMIN API

GET /admin/dashboard

GET /admin/users

GET /admin/payments

GET /admin/aircraft

GET /admin/statistics

POST /admin/product

PUT /admin/product

DELETE /admin/product

---

## ANALYTICS API

GET /analytics/users

GET /analytics/revenue

GET /analytics/teams

GET /analytics/countries

GET /analytics/aircraft

---

## NOTIFICATION API

POST /notification/send

GET /notification/history

---

## FILE API

POST /upload

GET /download

DELETE /file

---

## SECURITY

- HTTPS
- JWT
- Rate Limiting
- Audit Logs
- Role Permissions

---

## RESPONSE FORMAT

- Success
- Error
- Validation Error
- Unauthorized
- Not Found
- Internal Error

---

## FUTURE

- GraphQL
- Public API
- Partner API
- Mobile SDK
- Webhooks

---

## STATUS

Draft v1.0
