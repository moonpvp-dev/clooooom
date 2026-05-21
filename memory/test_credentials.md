# CurlLoom — Test Credentials

## Admin API
- **Endpoint base**: `/api/admin/*`
- **Auth**: Bearer token in `Authorization` header
- **Token**: `Kv9Up6myVI3C9WekNLy2bhhHM6sDbC17yO2kbQm8kJU`
- **Source**: `/app/backend/.env` → `ADMIN_TOKEN`

## Example
```
curl -H "Authorization: Bearer Kv9Up6myVI3C9WekNLy2bhhHM6sDbC17yO2kbQm8kJU" \
  https://<host>/api/admin/early-access
```

## Public endpoints (no auth)
- POST /api/early-access (5/min limit)
- POST /api/contact (5/min)
- POST /api/quiz (10/min)
- POST /api/waitlist (10/min)
- GET /api/referral/{code} (30/min, returns only referral_count)
