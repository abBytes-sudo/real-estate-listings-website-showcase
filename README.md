# Rent A Roof — Public Property Website

I built this for **Rent A Roof**, a real-estate brokerage in South Delhi — the public **rentaroof.in** site that turns their live inventory into a fast, honest, conversion-focused property website for South Delhi, Gurugram and Noida. One-man team, design through deploy, driven end to end through agentic AI workflows, and it's in production.

Every screenshot below is of the live production site — real listings and real photography.

*The source is in a private repo; happy to share it with a serious reviewer on request.*

---

## What it is

A standalone Laravel front-end that reads the CRM's inventory read-only and presents it as a polished consumer site:

- **Home** — hero search, featured/verified listings, locality entry points, and the on-site Roofie assistant.
- **Listings & search** — live, filterable inventory with verified badges, photo galleries, and residential-first relevance.
- **Property detail** — full spec sheet, photo gallery, "verified by us", neighbourhood context (metro / schools / connectivity), similar listings, a locality guide, and an enquiry path.
- **Locality guides** — every serviced colony written up by the team, with price bands and live listings.
- **Testimonials, About, Contact, List-your-property** — the trust and supply pages.
- **Customer area** — phone-OTP sign-in to a saved-shortlist dashboard.

Design: Tailwind v4 `@theme` tokens (Rubik + IBM Plex Mono; warm cream / navy ink / amber), no CDNs, mobile-first.

---

## Screenshots · *live production*

### Home
![Home](screenshots/d-home.jpg)

### Listings & property detail
**Listings** — live inventory with verified badges & galleries
![Listings](screenshots/d-listings.jpg)
**Property detail** — spec, gallery, neighbourhood, similar listings, locality guide
![Property detail](screenshots/d-property.jpg)

### Locality guides
**Localities index** ![Localities](screenshots/d-localities.jpg)
**Locality guide** ![Locality detail](screenshots/d-locality-detail.jpg)

### Trust & supply
**Testimonials** ![Testimonials](screenshots/d-testimonials.jpg)
**About** ![About](screenshots/d-about.jpg)
**Contact** ![Contact](screenshots/d-contact.jpg)

### Mobile
| Home | Listings | Property | Localities |
|---|---|---|---|
| ![](screenshots/m-home.jpg) | ![](screenshots/m-listings.jpg) | ![](screenshots/m-property.jpg) | ![](screenshots/m-localities.jpg) |

| Locality guide | Testimonials | About | Contact |
|---|---|---|---|
| ![](screenshots/m-locality-detail.jpg) | ![](screenshots/m-testimonials.jpg) | ![](screenshots/m-about.jpg) | ![](screenshots/m-contact.jpg) |

---

## Tech
Laravel 13 · Blade · Alpine.js · Tailwind CSS v4 (`@theme` tokens) · MySQL (read-only CRM inventory) · PHP 8.4 · phone-OTP customer area

---
Developed by **[@abBytes-sudo](https://github.com/abBytes-sudo)** for Rent A Roof · abhimasih0505@gmail.com · +91 73039 37702
