# HotDoc (hotdoc)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
