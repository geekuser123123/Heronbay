# Information Required Before Launch

Run `node build.mjs` to see what's still missing. Nothing on the site has been invented.

## Already set

- [x] Name: **Heronbay**
- [x] Phone: **(656) 206-3496**
- [x] Site URL: `https://heronbay.kevin-c4h.workers.dev`
- [x] Hours: **Monday–Friday, 9:00 AM – 5:00 PM (Eastern Time)**, office meetings by appointment
- [x] Business type: **storefront office** at **2701 W Busch Blvd, Tampa, FL 33618** (Google Business Profile "Local store")
- [x] Services confirmed: plan setup, records and valuations, Form 5500-EZ preparation, ongoing
      support, Self-Directed and Solo 401(k) education, and office meetings
- [x] Role: administrative support alongside the client's plan provider, at the sponsor's
      direction. The business is not a fiduciary, trustee, custodian, registered investment
      adviser or broker-dealer.
- [x] Format: a one-page site, with separate Privacy, Terms and Disclosures pages

## Required

| Item | Notes |
|---|---|
| **Contact form (n8n)** | Create the n8n workflow (see `docs/N8N-FORM-SETUP.md`) and put its production webhook URL in `form.webhookUrl` in `site.config.mjs`. Until then the form shows a notice and doesn't send. |
| **Register the business name** | If "Heronbay" isn't the legal name of the business, register it as a fictitious name with the Florida Division of Corporations (Sunbiz). Florida requires advertising the name once in a newspaper in Hillsborough County before registering (if "Heronbay" isn't the legal name of the business). Then set `business.publicNameConfirmed: true`. Check the Florida Division of Corporations (Sunbiz), the USPTO and Google Maps for "Heronbay" conflicts first. |

Optional: `business.geo` with the office's real coordinates.

## Recommended before going public

- [ ] An attorney has reviewed the Privacy Policy, Terms and Disclosures (Florida law, administrative-services wording).
- [ ] An ERISA attorney has confirmed the administrative-services role.
- [ ] n8n: a test submission from the live site landed on the thank-you page and ran the workflow.
- [ ] Cloudflare Pages: the site is deployed. Then add the Search Console verification code to `site.googleSiteVerification`.

## Optional (hidden until set)

Business email, owner name, company history and credentials.
