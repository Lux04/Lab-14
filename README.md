# Bie Daalt 14 — Integration & API Testing

## Сонгосон API
DummyJSON API — https://dummyjson.com

## Ашигласан хэрэгсэл
- Postman
- Newman
- GitHub Actions
- DummyJSON Public API

## Newman ажиллуулах

```bash
npm install -g newman
npm install -g newman-reporter-htmlextra

newman run postman/collection.json -e postman/env.dev.json
```

## HTML report үүсгэх

```bash
newman run postman/collection.json -e postman/env.dev.json \
  --reporters cli,htmlextra \
  --reporter-htmlextra-export reports/api.html
```

## GitHub Actions
Push хийхэд `.github/workflows/api-tests.yml` автоматаар Newman тест ажиллуулна.
