# HotDoc (hotdoc)

HotDoc is an Australian patient-engagement platform, founded in 2012 and headquartered in Melbourne, that connects patients with general practices, dentists, and specialists. Roughly one in three Australians use HotDoc to find and book healthcare, and the platform serves more than 21,000 practitioners. Its clinic-facing SaaS provides online bookings, telehealth, appointment reminders, SMS recalls, mobile and kiosk check-in, digital new-patient registration forms, online repeat prescription requests, and preventative-health outreach. HotDoc was acquired by Potentia in February 2026.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/hotdoc/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/hotdoc/refs/heads/main/apis.yml)

## Tags

- Healthcare
- Australia
- Patient Engagement
- Online Booking
- Appointment Scheduling
- Telehealth
- Practice Management
- Primary Care
- Digital Health
- e-Prescribing

## Timestamps

- **Created:** 2026-07-24
- **Modified:** 2026-07-24

## API Posture

HotDoc operates as an engagement layer on top of Australian practice-management systems (Best Practice, MedicalDirector, Zedmed, Genie, Cliniko, Nookal and others). A clinic connects HotDoc by entering its practice-management-system API key into the HotDoc dashboard, so HotDoc **consumes** those PMS APIs rather than publishing its own.

As of the review date (2026-07-24) HotDoc exposes:

- **No public developer portal** — the `developer.`, `docs.`, `api.`, and `fhir.` subdomains all resolve to the same catch-all HotDoc web application and serve the consumer site, not API documentation.
- **No documented third-party REST/OpenAPI** — `/openapi.json` and `/swagger.json` return HTTP 404.
- **No HL7 FHIR CapabilityStatement** — `/metadata`, `/fhir/metadata`, and `/.well-known/smart-configuration` return HTTP 404.

Its integration surface is partner/PMS-gated. See [`review.yml`](review.yml) for the full reviewer finding.

## Common Properties

- [Website](https://www.hotdoc.com.au/)
- [Practice / Product Site](https://practices.hotdoc.com.au/)
- [Blog](https://www.hotdoc.com.au/blog/)
- [Status Page](https://status.hotdoc.com.au/)
- [GitHub Organization](https://github.com/htdc)
- [LinkedIn](https://www.linkedin.com/company/hotdoc)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
