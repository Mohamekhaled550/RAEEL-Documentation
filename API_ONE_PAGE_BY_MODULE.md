# Raeel Backend APIs — One Page (Grouped by Module)

> صفحة واحدة تشمل كل APIs الحالية تحت بعض ومقسمة حسب الموديول.
> Base URL: `{{base_url}} = http://127.0.0.1:8000/api`

---

## Health
- `GET /api/health`
- `GET /api/health/database`
- `GET /api/health/queue`
- `GET /api/health/storage`

## Auth
- `POST /api/v1/auth/register`
- `POST /api/v1/auth/login`
- `POST /api/v1/auth/forgot-password`
- `POST /api/v1/auth/reset-password`
- `GET /api/v1/auth/me`
- `POST /api/v1/auth/logout`
- `POST /api/v1/auth/logout-all`
- `POST /api/v1/auth/refresh`
- `POST /api/v1/auth/email/verification-notification`
- `POST /api/v1/auth/email/verify`
- `POST /api/v1/auth/otp`

## ActivityLogs (Admin)
- `GET /api/v1/admin/activity-logs`
- `POST /api/v1/admin/activity-logs`
- `GET /api/v1/admin/activity-logs/{activity_log}`
- `PUT|PATCH /api/v1/admin/activity-logs/{activity_log}`
- `DELETE /api/v1/admin/activity-logs/{activity_log}`

## Addons
- `GET /api/v1/addons`
- `POST /api/v1/addons`
- `GET /api/v1/addons/{addon}`
- `PUT|PATCH /api/v1/addons/{addon}`
- `DELETE /api/v1/addons/{addon}`

## Amenities
- `GET /api/v1/amenities`
- `POST /api/v1/amenities`
- `GET /api/v1/amenities/{amenity}`
- `PUT|PATCH /api/v1/amenities/{amenity}`
- `DELETE /api/v1/amenities/{amenity}`

## Authorization (Admin)
- `GET /api/v1/admin/roles`
- `POST /api/v1/admin/roles`
- `GET /api/v1/admin/roles/{role}`
- `PUT|PATCH /api/v1/admin/roles/{role}`
- `DELETE /api/v1/admin/roles/{role}`
- `GET /api/v1/admin/permissions`
- `POST /api/v1/admin/permissions`
- `GET /api/v1/admin/permissions/{permission}`
- `PUT|PATCH /api/v1/admin/permissions/{permission}`
- `DELETE /api/v1/admin/permissions/{permission}`

## Branches
- `GET /api/v1/branches`
- `POST /api/v1/branches`
- `GET /api/v1/branches/{branch}`
- `PUT|PATCH /api/v1/branches/{branch}`
- `DELETE /api/v1/branches/{branch}`

## SpaceCategories
- `GET /api/v1/space-categories`
- `POST /api/v1/space-categories`
- `GET /api/v1/space-categories/{space_category}`
- `PUT|PATCH /api/v1/space-categories/{space_category}`
- `DELETE /api/v1/space-categories/{space_category}`

## Spaces
- `GET /api/v1/spaces`
- `POST /api/v1/spaces`
- `GET /api/v1/spaces/{space}`
- `PUT|PATCH /api/v1/spaces/{space}`
- `DELETE /api/v1/spaces/{space}`
- `GET /api/v1/spaces/{id}/availability`
- `GET /api/v1/spaces/{id}/intelligence`

## Leads
- `GET /api/v1/leads`
- `POST /api/v1/leads`
- `GET /api/v1/leads/{lead}`
- `PUT|PATCH /api/v1/leads/{lead}`
- `DELETE /api/v1/leads/{lead}`

## Customers
- `GET /api/v1/customers`
- `POST /api/v1/customers`
- `GET /api/v1/customers/{customer}`
- `PUT|PATCH /api/v1/customers/{customer}`
- `DELETE /api/v1/customers/{customer}`

## Quotations
- `GET /api/v1/quotations`
- `POST /api/v1/quotations`
- `GET /api/v1/quotations/{quotation}`
- `POST /api/v1/quotations/{id}/accept`
- `POST /api/v1/quotations/{id}/recalculate`

## Bookings
- `GET /api/v1/bookings`
- `GET /api/v1/bookings/{booking}`
- `GET /api/v1/bookings/calendar`
- `POST /api/v1/bookings/{id}/confirm`
- `POST /api/v1/bookings/{id}/cancel`

## Contracts
- `GET /api/v1/contracts/{id}`
- `POST /api/v1/contracts/{id}/sign`
- `GET /api/v1/bookings/{id}/contract`

## Invoices
- `GET /api/v1/invoices`
- `GET /api/v1/invoices/{invoice}`
- `POST /api/v1/invoices/{id}/issue`

## Payments
- `GET /api/v1/payments`
- `POST /api/v1/payments`
- `GET /api/v1/payments/{payment}`
- `POST /api/v1/payments/{id}/gateway`
- `POST /api/v1/payments/{id}/refund`
- `POST /api/v1/payments/gateway/webhook`
- `GET /api/v1/payments/webhook-metrics`

## Notifications
- `GET /api/v1/notifications`
- `POST /api/v1/notifications`
- `GET /api/v1/notifications/{notification}`
- `PUT|PATCH /api/v1/notifications/{notification}`
- `DELETE /api/v1/notifications/{notification}`

## Favorites
- `GET /api/v1/favorites`
- `POST /api/v1/favorites`
- `GET /api/v1/favorites/{favorite}`
- `PUT|PATCH /api/v1/favorites/{favorite}`
- `DELETE /api/v1/favorites/{favorite}`

## Reviews
- `GET /api/v1/reviews`
- `POST /api/v1/reviews`
- `GET /api/v1/reviews/{review}`
- `PUT|PATCH /api/v1/reviews/{review}`
- `DELETE /api/v1/reviews/{review}`

## Media
- `GET /api/v1/media`
- `POST /api/v1/media`
- `GET /api/v1/media/{medium}`
- `PUT|PATCH /api/v1/media/{medium}`
- `DELETE /api/v1/media/{medium}`
- `POST /api/v1/media/upload`

## Settings (Admin)
- `GET /api/v1/admin/settings`
- `POST /api/v1/admin/settings`
- `GET /api/v1/admin/settings/{setting}`
- `PUT|PATCH /api/v1/admin/settings/{setting}`
- `DELETE /api/v1/admin/settings/{setting}`

## Reports
- `GET /api/v1/dashboard/overview`
- `GET /api/v1/dashboard/occupancy`
- `GET /api/v1/dashboard/revenue`
- `GET /api/v1/dashboard/funnel`
- `GET /api/v1/dashboard/space-cards`

## Customer Portal
- `GET /api/v1/customer/dashboard`
- `GET /api/v1/customer/bookings`
- `GET /api/v1/customer/invoices`
- `GET /api/v1/customer/contracts`
- `GET /api/v1/customer/payments`
- `GET /api/v1/customer/notifications`
- `GET /api/v1/customer/favorites`
- `GET /api/v1/customer/reviews`

## Admin Operations (Admin)
- `POST /api/v1/admin/operations/status`
- `POST /api/v1/admin/operations/notifications/resend`
- `POST /api/v1/admin/operations/pdf/regenerate`
- `POST /api/v1/admin/operations/quotations/{id}/recalculate`
- `POST /api/v1/admin/operations/quotations/{id}/expire`
- `POST /api/v1/admin/operations/invoices/{id}/recalculate`
- `POST /api/v1/admin/operations/payments/{id}/resync`
- `POST /api/v1/admin/operations/dashboard/cache/refresh`

---
