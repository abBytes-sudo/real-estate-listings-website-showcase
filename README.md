# Rent A Roof — Public Property Website

The public **rentaroof.in** site — a standalone Laravel app that turns the brokerage's live inventory into a fast, honest, conversion-focused property website for South Delhi, Gurugram and Noida.

> 🔒 **This is a public showcase.** The site's source lives in a **private** repository — happy to grant access to serious reviewers on request. The screenshots below are of the **live production site** (real listings & photography).

---

## What it is

A separate Laravel 13 front-end that reads the CRM's inventory read-only and presents it as a polished consumer site:

- **Home** — hero search, featured/verified listings, locality entry points, and the on-site **Roofie** assistant.
- **Listings & search** — live, filterable inventory with verified badges, photo galleries, and residential-first relevance.
- **Property detail** — full spec sheet, photo gallery, "verified by us", neighbourhood context (metro / schools / connectivity), similar listings, a locality guide, and an enquiry path.
- **Locality guides** — every serviced colony written up by the team, with price bands and live listings.
- **Testimonials, About, Contact, List-your-property** — the trust + supply pages.
- **Customer area** — phone-OTP sign-in to a saved-shortlist dashboard.

Design: Tailwind v4 `@theme` tokens (Rubik + IBM Plex Mono; warm cream / navy ink / amber), no CDNs, mobile-first.

---

## 📸 Screenshots · *live production*

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

### 📱 Mobile
| Home | Listings | Property | Localities |
|---|---|---|---|
| ![](screenshots/m-home.jpg) | ![](screenshots/m-listings.jpg) | ![](screenshots/m-property.jpg) | ![](screenshots/m-localities.jpg) |

| Locality guide | Testimonials | About | Contact |
|---|---|---|---|
| ![](screenshots/m-locality-detail.jpg) | ![](screenshots/m-testimonials.jpg) | ![](screenshots/m-about.jpg) | ![](screenshots/m-contact.jpg) |

---

## 🧰 Tech
`Laravel 13` · `Blade` · `Alpine.js` · `Tailwind CSS v4` (`@theme` tokens) · `MySQL` (read-only CRM inventory) · `PHP 8.4` · phone-OTP customer area

## 🔑 Want to see the code?
The complete source is in a **private repository** — reach out for access.

---
Built by **[@abBytes-sudo](https://github.com/abBytes-sudo)** · abhimasih0505@gmail.com · +91 73039 37702
