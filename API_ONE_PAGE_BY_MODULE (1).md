# Raeel Backend APIs — One Page (Grouped by Module)

> صفحة واحدة تشمل كل الـ APIs الحالية ومقسمة حسب الموديول.
> Base URL: `{{base_url}} = http://127.0.0.1:8000/api`

## قواعد التنظيم السريعة
- كل مسارات `/api/v1/admin/**` تحتاج `auth:sanctum` + صلاحية admin عبر `EnsureAdminRole`.
- أي عملية إدارة/Backoffice مثل إضافة أو تعديل أو حذف أو اعتماد أو إصدار أو استرداد أو تقارير إدارية موجودة تحت `/admin`.
- مسارات العميل أو البوابة أو الإجراء الخارجي فقط تظل خارج `/admin`.

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

---

# Admin / Backoffice APIs

## ActivityLogs (Admin)
- `GET /api/v1/admin/activity-logs`
- `POST /api/v1/admin/activity-logs`
- `GET /api/v1/admin/activity-logs/{activity_log}`
- `PUT|PATCH /api/v1/admin/activity-logs/{activity_log}`
- `DELETE /api/v1/admin/activity-logs/{activity_log}`

## Addons (Admin)
- `GET /api/v1/admin/addons`
- `POST /api/v1/admin/addons`
- `GET /api/v1/admin/addons/{addon}`
- `PUT|PATCH /api/v1/admin/addons/{addon}`
- `DELETE /api/v1/admin/addons/{addon}`

## Amenities (Admin)
- `GET /api/v1/admin/amenities`
- `POST /api/v1/admin/amenities`
- `GET /api/v1/admin/amenities/{amenity}`
- `PUT|PATCH /api/v1/admin/amenities/{amenity}`
- `DELETE /api/v1/admin/amenities/{amenity}`

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

## Branches (Admin)
- `GET /api/v1/admin/branches`
- `POST /api/v1/admin/branches`
- `GET /api/v1/admin/branches/{branch}`
- `PUT|PATCH /api/v1/admin/branches/{branch}`
- `DELETE /api/v1/admin/branches/{branch}`

## SpaceCategories (Admin)
- `GET /api/v1/admin/space-categories`
- `POST /api/v1/admin/space-categories`
- `GET /api/v1/admin/space-categories/{space_category}`
- `PUT|PATCH /api/v1/admin/space-categories/{space_category}`
- `DELETE /api/v1/admin/space-categories/{space_category}`

## Spaces (Admin)
- `GET /api/v1/admin/spaces`
- `POST /api/v1/admin/spaces`
- `GET /api/v1/admin/spaces/{space}`
- `PUT|PATCH /api/v1/admin/spaces/{space}`
- `DELETE /api/v1/admin/spaces/{space}`
- `GET /api/v1/admin/spaces/{id}/intelligence`

## Leads (Admin)
- `GET /api/v1/admin/leads`
- `POST /api/v1/admin/leads`
- `GET /api/v1/admin/leads/{lead}`
- `PUT|PATCH /api/v1/admin/leads/{lead}`
- `DELETE /api/v1/admin/leads/{lead}`

## Customers (Admin)
- `GET /api/v1/admin/customers`
- `POST /api/v1/admin/customers`
- `GET /api/v1/admin/customers/{customer}`
- `PUT|PATCH /api/v1/admin/customers/{customer}`
- `DELETE /api/v1/admin/customers/{customer}`

## Quotations (Admin)
- `GET /api/v1/admin/quotations`
- `POST /api/v1/admin/quotations`
- `GET /api/v1/admin/quotations/{quotation}`
- `POST /api/v1/admin/quotations/{id}/recalculate`

## Bookings (Admin)
- `GET /api/v1/admin/bookings`
- `GET /api/v1/admin/bookings/{booking}`
- `GET /api/v1/admin/bookings/calendar`
- `POST /api/v1/admin/bookings/{id}/confirm`
- `POST /api/v1/admin/bookings/{id}/cancel`

## Contracts (Admin)
- `GET /api/v1/admin/contracts/{id}`
- `GET /api/v1/admin/bookings/{id}/contract`

## Invoices (Admin)
- `GET /api/v1/admin/invoices`
- `GET /api/v1/admin/invoices/{invoice}`
- `POST /api/v1/admin/invoices/{id}/issue`

## Payments (Admin)
- `GET /api/v1/admin/payments`
- `POST /api/v1/admin/payments`
- `GET /api/v1/admin/payments/{payment}`
- `POST /api/v1/admin/payments/{id}/refund`
- `GET /api/v1/admin/payments/webhook-metrics`

## Notifications (Admin)
- `GET /api/v1/admin/notifications`
- `POST /api/v1/admin/notifications`
- `GET /api/v1/admin/notifications/{notification}`
- `PUT|PATCH /api/v1/admin/notifications/{notification}`
- `DELETE /api/v1/admin/notifications/{notification}`

## Reviews (Admin)
- `GET /api/v1/admin/reviews`
- `POST /api/v1/admin/reviews`
- `GET /api/v1/admin/reviews/{review}`
- `PUT|PATCH /api/v1/admin/reviews/{review}`
- `DELETE /api/v1/admin/reviews/{review}`

## Media (Admin)
- `GET /api/v1/admin/media`
- `POST /api/v1/admin/media`
- `GET /api/v1/admin/media/{medium}`
- `PUT|PATCH /api/v1/admin/media/{medium}`
- `DELETE /api/v1/admin/media/{medium}`
- `POST /api/v1/admin/media/upload`

## Settings (Admin)
- `GET /api/v1/admin/settings`
- `POST /api/v1/admin/settings`
- `GET /api/v1/admin/settings/{setting}`
- `PUT|PATCH /api/v1/admin/settings/{setting}`
- `DELETE /api/v1/admin/settings/{setting}`

## Reports / Dashboard (Admin)
- `GET /api/v1/admin/dashboard/overview`
- `GET /api/v1/admin/dashboard/occupancy`
- `GET /api/v1/admin/dashboard/revenue`
- `GET /api/v1/admin/dashboard/funnel`
- `GET /api/v1/admin/dashboard/space-cards`

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

# Non-Admin / Customer / Integration APIs

## Spaces
- `GET /api/v1/spaces/{id}/availability`

## Quotations
- `POST /api/v1/quotations/{id}/accept`

## Contracts
- `POST /api/v1/contracts/{id}/sign`

## Payments
- `POST /api/v1/payments/{id}/gateway`
- `POST /api/v1/payments/gateway/webhook`

## Favorites
- `GET /api/v1/favorites`
- `POST /api/v1/favorites`
- `GET /api/v1/favorites/{favorite}`
- `PUT|PATCH /api/v1/favorites/{favorite}`
- `DELETE /api/v1/favorites/{favorite}`

## Customer Portal
- `GET /api/v1/customer/dashboard`
- `GET /api/v1/customer/bookings`
- `GET /api/v1/customer/invoices`
- `GET /api/v1/customer/contracts`
- `GET /api/v1/customer/payments`
- `GET /api/v1/customer/notifications`
- `GET /api/v1/customer/favorites`
- `GET /api/v1/customer/reviews`

---
