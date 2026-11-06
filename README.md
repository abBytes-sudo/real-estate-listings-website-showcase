# Real Estate Platform — public website

**Case study 02 · Real Estate Platform · public website** · relaunched Sep 2026 · [Live site: rentaroof.in](https://rentaroof.in)

### A property site that answers the way people *actually* search.

Plain-English search, a colony price guide and **Roofie**, a scripted enquiry assistant, for a Delhi property brokerage. Relaunched in Sep 2026 alongside a self-hosted CRM.

**Status:** live since the 9 Sep 2026 relaunch. Live site: [rentaroof.in](https://rentaroof.in).

**My role:** product owner, AI-assisted build. I set the requirements and made the product decisions; AI coding tools write the code under my direction, and I test every change. The site is the public side of the [Real Estate Platform — CRM & operations](https://github.com/abBytes-sudo/real-estate-crm-showcase).

| Role | Live | Stack |
|---|---|---|
| Product owner · AI-assisted build | [rentaroof.in](https://rentaroof.in) | Laravel · Livewire · MySQL |

| **6,564** | **20** |
|---|---|
| active listings on the site · *6 Nov 2026* | organic listing enquiries · *9 Sep → 6 Nov 2026* |

> **Case study PDF.** This page tells the same story as my 20-page PDF case study, *Real Estate Platform — public website*, chapter for chapter (01–11 below), with more screens. The PDF itself is not in this repo; ask for it through the contact details on my [GitHub profile](https://github.com/abBytes-sudo).

![Search results on desktop for "3 bhk in vasant vihar under 1.5 lakh": 3 BHK listings in Vasant Vihar with the Roofie panel beside them](screenshots/search-desktop.jpg)

*Search, desktop: one typed sentence, read as filters, with Roofie open beside the results. Screens: white-labelled demo copy, fictional data.*

<p align="center">
  <img src="screenshots/roofie-1.jpg" alt="Roofie chat on a phone: a visitor types a 3 BHK brief for Vasant Vihar and Roofie replies with the top live matches" width="280"><br>
  <em>Roofie, phone: a typed brief becomes matches from live stock.</em>
</p>

### What makes it different
- **Read plain English.** One box takes a whole sentence; the colony becomes a chip and the rest become filters you can remove.
- **Filtered lists are the landing pages.** A search such as "3 BHK for rent in Vasant Vihar" is itself the landing page, with its own title and Google tags: 7,474 pages built from live stock.
- **Show what's fair.** Rent and sale bands, with gross yield, by colony, from the team's curated pricing matrix, not averaged asking prices.
- **Scripted by design.** Roofie is a scripted, rule-based enquiry assistant, not AI: no external API and no LLM, as the owner required. Any thread can pass to a person.
- **Channel ≠ capture.** A visitor who googled, then used Roofie, reads "Google search" + "Roofie", so search gets credit for the lead.
- **One source of truth.** Listings publish straight from the CRM's inventory, with a publish switch on each listing. No second copy to keep in sync, and a let or sold home is never advertised.

### Run from the CRM, without a developer
The points the team changes themselves, as described in the chapters below:
- **Listings:** each listing has a publish switch in the CRM; publish refuses a let or sold home (01, 07).
- **Homepage:** the headline, photo and stat bar are edited in the CRM (04).
- **Search shorthand:** "DC" for Defence Colony is a synonym row admins edit in the CRM, with no code change (04).
- **Roofie's answers:** paperwork and viewing questions are answered from the FAQ the team edits in the CRM, so editing an answer changes Roofie's reply (06).
- **Locality guides:** 78 guides the team writes in the CRM (notes, nearby places and photos); map, prices and live listings are added automatically (03).
- **Journal:** staff draft, schedule or publish, with each post's category, cover and featured flag (10).
- **The rest of the site:** homepage, new pages from ready-made blocks, menus, footer and FAQ, under separate permissions (10).

<sub>*About the screenshots:* screens are from a white-labelled demo build: "abBytes" is a placeholder brand standing in for Rent A Roof, and the listings, people, stock photos (any faces blurred), phone numbers (masked) and emails are placeholders; figures marked "demo" are fictional. Layouts match production. The only production numbers are the dated ones in this write-up. The source is in a private repo; walkthrough on request.</sub>

---

**Contents:** [01 The brief](#01--the-brief) · [02 Results](#02--results) · [03 On-page SEO](#03--on-page-seo) · [04 Plain-English search](#04--plain-english-search) · [05 Price guide](#05--price-guide) · [06 Roofie](#06--roofie) · [07 Listings](#07--listings) · [08 Customer dashboard](#08--customer-dashboard) · [09 List your property](#09--list-your-property) · [10 The journal](#10--the-journal) · [11 How it was built](#11--how-it-was-built) · [More screens](#more-screens-full-pages-from-the-demo-build)

---

## 01 · The brief

### What's there? What's fair? Who do I *talk to*?
Every renter brings the same three questions. A Delhi property brokerage was relaunching its website alongside a new self-hosted CRM, and visitors don't think in dropdowns: they type a sentence, want to know what's fair, and want a person when they ask for one, even after hours.

> **A brief, as people type it**
>
> *"Looking for a 3 BHK to rent in Vasant Vihar under 1.5 lakh, family of 4, moving in December."*
>
> Not ~~City ▾~~ ~~Locality ▾~~ ~~Budget ▾~~

| 01 · Read plain English | 02 · Show what's fair | 03 · Answer first | 04 · One source of truth |
|---|---|---|---|
| A sentence becomes filters: bedrooms, colony, budget. | Rent and sale bands, with gross yield, by colony. | A scripted assistant that matches, saves, requests visits and passes to a person. | Listings publish straight from the CRM's inventory, with a publish switch on each listing. No second copy to keep in sync. |

---

## 02 · Results

### Found on Google within a *month*.

**26 → 103** engaged visitors from Google search a week, within two months of the relaunch.

| Week (IST) | Dates | Engaged visitors from Google search | |
|---|---|---:|---|
| W37\* | 11–13 Sep | 3 | █ |
| W38 | 14–20 Sep | 26 | █████ |
| W39 | 21–27 Sep | 34 | ███████ |
| W40 | 28 Sep – 4 Oct | 41 | ████████ |
| W41 | 5–11 Oct | 89 | █████████████████ |
| W42 | 12–18 Oct | 77 | ███████████████ |
| W43 | 19–25 Oct | 79 | ███████████████ |
| **W44** | **26 Oct – 1 Nov** | **103** | **████████████████████** |
| W45\* | 2–6 Nov | 47 | █████████ |

<sub>\*Part weeks: the tracker went live on 11 Sep; W45 runs to 6 Nov. · *6 Nov 2026 · first-party tracker*</sub>

| **43%** | **6,467** |
|---|---|
| of engaged visitors in the 30 days to 6 Nov came from Google search (**375 of 880**), up from 22% in the 30 days to 23 Oct. *6 Nov 2026* | site searches since 11 Sep. Searches naming a colony also feed the verification desk's list of where to check listings next. *6 Nov 2026* |
| **Page 1** | **499** |
| on Google for rent searches in 5 key South Delhi localities, within 30 days of the relaunch (Search Console + manual checks). *Sep–Oct 2026* | engaged visitors from Google search since 11 Sep, averaging **5 min 35 s** each. *6 Nov 2026* |

Counted by the site's own tracker, which filters known bots, burst crawlers and signed-in staff; Google figures count engaged visitors only (raw Google-referred counts include automated desktop bursts).

### About 2 months after go-live: *enquiries*, not just visits.
<sub>*9 Sep → 6 Nov 2026 · new leads only, imported history excluded*</sub>

| **32** | **20** | **101 of 119** |
|---|---|---|
| website & Roofie leads: 22 Roofie property enquiries, 8 Roofie chats, 2 website forms. | organic property enquiries: new leads who asked about one specific listing, all through Roofie on the listing page. **11 arrived from Google search.** | website chats since 7 Sep never needed an agent (85%); 35 became or joined an enquiry. |
| 12 Google search · 9 came direct · 9 social & tagged links · 2 Meta ads. **30 organic** · 12 from Google search · **17 of 32 (53%)** now have a qualified requirement. | 11 from Google search · 9 from other organic channels · 2 more came from a Meta ad. | Roofie only: 101 · An agent replied: 18. *6 Nov 2026* |

**Across every channel: 147 organic leads by source (not paid ads or portals) of 496 new leads.**

| Instagram DMs | Inbound calls | Website & Roofie | WhatsApp | Customer sign-ups | Broker referral |
|---:|---:|---:|---:|---:|---:|
| 55 | 33 | 32 | 24 | 2 | 1 |

Only the website & Roofie slice is website-attributable; Instagram and WhatsApp leads are messages logged by staff. Strictest count: 145 not linked to any ad.

**Organic leads qualify more than twice as often**

| | Now have a qualified requirement |
|---|---|
| Organic | **58%** · 85 of 147 |
| Meta ads | **23%** · 78 of 334 |

<sub>*6 Nov 2026 · CRM, read-only query*</sub>

---

## 03 · On-page SEO

### 7,474 pages, *built from live stock*.
Live listings, colonies and common searches (rent, buy, BHK, builder floor) get pages built from the CRM's inventory; new stock joins the sitemap the next night.

**All 7,474 URLs in the sitemap · 6 Nov 2026**

| Page type | URLs |
|---|---:|
| Listing pages | 6,561 |
| Locality × type landing pages (buy 327 · rent 192 · commercial 80) | 599 |
| Locality & type hubs | 163 |
| Locality guides | 77 |
| "Real-estate agency in &lt;colony&gt;" | 41 |
| Journal & site pages | 33 |
| **Total** | **7,474** |

Built the way Delhi searches: builder floors, kothis, a 3 BHK page with every colony page, a South Delhi page spanning three districts (owner decisions, Sep–Oct 2026).

**Where engaged Google visitors landed** · 499 engaged visitors from Google search since 11 Sep

| Landing page | Visitors | |
|---|---:|---|
| Home | 146 | ████████████████████ |
| Rent pages | 89 | ████████████ |
| Listing pages | 82 | ███████████ |
| Buy pages | 78 | ███████████ |
| Journal | 37 | █████ |
| Commercial | 32 | ████ |
| Locality guides | 22 | ███ |
| Site search | 9 | █ |

<sub>*6 Nov 2026 · first-party tracker*</sub>

#### What makes it different
1. **Filtered lists are the landing pages.** A search such as "3 BHK for rent in Vasant Vihar" is itself the landing page, with its own title and Google tags, so there is no second set of pages to maintain (SEO build plan, 24 Sep 2026).
2. **No thin pages.** Apart from each colony's 3 BHK page, a landing is indexed and linked only with 5+ live listings; a thin or empty 3 BHK page says so and offers real alternatives (`LandingLinks`, `ColonyThreeBhkPage`).
3. **Dated by real changes.** The sitemap rebuilds nightly; a page's date is when its listings or post last changed, never just "today", then IndexNow alerts Bing and others (`SitemapBuilder`).

### Three ways in from *Google*.
Locality × type, agency and locality-guide pages all read the same live inventory. The journal, a fourth way in, has its own chapter ([10](#10--the-journal)).

![Locality × type landing page for 3 BHK rentals in Chittaranjan Park on desktop: "Showing 1–1 of 1 property", then more homes in and around the colony and similar sizes](screenshots/seo-colony.jpg)

*`/rent/chittaranjan-park/3-bhk` · A thin 3 BHK page says so, then shows real nearby stock. Every colony with 5+ live homes gets one, among 599 landings, each with its own title and canonical. Demo stock.*

<p align="center">
  <img src="screenshots/seo-colony-phone.jpg" alt="The same Chittaranjan Park 3 BHK landing page on a phone: the colony chip, filters, the 'only a few' note and similar sizes" width="280"><br>
  <em>Phone: the same page and the same "only a few" note.</em>
</p>

![Agency page for Defence Colony on desktop: "Real estate agency in Defence Colony" with live counts of homes to rent and commercial listings](screenshots/agency-hero.jpg)

*`/real-estate-agency/defence-colony` · Agency pages: 41 colony pages, each needing 10+ live listings and its own local facts, such as price bands and local names. Demo figures.*

![Locality guide header for Vasant Vihar on desktop: live listings count, location and tabs for map, guide, around, prices and live listings](screenshots/locality-tile.jpg)

*`/localities/vasant-vihar` · Locality guides: 77 guides the team writes in the CRM (notes, nearby places and photos). Map, prices and live listings are added automatically.*

#### What makes it different
1. **Old links still land.** Pre-relaunch URLs 301 to the matching colony and BHK page (`LegacySlug`).
2. **Homes-only pages** for "flats for rent in…" searches: no shops mixed in (owner, 28 Sep 2026).

---

## 04 · Plain-English search

### Type it the way you'd *say* it.

**What people type → what the search reads**

| "3 bhk" | "in vasant vihar" | "under 1.5 lakh" |
|:---:|:---:|:---:|
| **3 BHK** · bedrooms | **Vasant Vihar** · colony | **Up to ₹1.5 L** · budget |

One box takes a whole sentence. The colony becomes a chip, the rest become filters you can remove, and the results update.

![Search page on desktop: Vasant Vihar as a colony chip, applied filters for 3 BHK and up to ₹1.5 L with clear all, then the matching 3 BHK homes](screenshots/search-chips.jpg)

*`/search` · Desktop: the colony chip, applied filters you can clear, then the matching homes.*

<p align="center">
  <img src="screenshots/search-phone2.jpg" alt="The same search on a phone: one search bar with the Vasant Vihar chip and the filters folded into a single control above the results" width="280"><br>
  <em>Phone: the same search in one bar, filters folded into a single control.</em>
</p>

**6,467** site searches since 11 Sep · *6 Nov 2026*

### Never a *dead end*.

#### What makes it different
1. **Reads local usage.** "Kothi" means an independent house and a bare price under ₹10 lakh means rent (`SearchParser`). Shorthand like "DC" for Defence Colony is a synonym row admins edit in the CRM, with no code change.
2. **One parser, three places.** The website, Roofie and the staff property search read briefs the same way (`InventorySearchInterpreter`).
3. **Help while typing.** Typeahead with live counts (owner, 31 Aug), a "Search for …" fallback and "did you mean" on thin results; rent and sale shown together by default (29 Aug 2026).

<p align="center">
  <img src="screenshots/home-search.jpg" alt="Home page hero on desktop: one search box with worked examples to tap, such as 3 BHK for rent in Defence Colony, and a link to classic search" width="560"><br>
  <em><code>/</code> · Home: one box, worked examples to tap, and classic filters one link away. The headline, photo and stat bar are edited in the CRM.</em>
</p>

![Roofie nudge: "I can shortlist the best few of these 4 for you — want me to?" with a "Yes, shortlist a few" button](screenshots/roofie-nudge.jpg)

*Roofie: when results are few, it offers to shortlist them.*

<p align="center">
  <img src="screenshots/close-desk.jpg" alt="Search results on desktop: a 'Just outside your budget' group of listings within about 25% of the visitor's range, then similar sizes" width="560"><br>
  <em><code>/search</code> · Close matches, labelled: with 8 or fewer strict results, the page adds groups that each widen one thing: budget ±25%, ±1 BHK or nearby colonies.</em>
</p>

---

## 05 · Price guide

### What's fair, before the *first call*.
Rent and sale bands by colony, each with its gross yield. Roofie can quote an area's band in chat, too.

Bands come from the team's curated pricing matrix, not averaged asking prices; a colony with no band shows nothing rather than a guess (`LocalityPricing`).

**Anatomy of a colony card**

| **Colony** · *gross yield* | |
|---|---|
| **Rent** | low ──────── high /mo |
| **Sale** | low ──────── high |

*Gross yield = 12 × monthly rent ÷ sale price.*

![Price guide on desktop: "What South Delhi actually rents and sells for", headline market figures, then colony cards with rent band, sale band and gross yield](screenshots/price-desk2.jpg)

*`/price-guide` · Desktop: headline market figures, then one card per colony: rent band, sale band, gross yield and a link to that colony's guide. Demo figures.*

<p align="center">
  <img src="screenshots/price-phone2.jpg" alt="The price guide on a phone: headline figures, then a colony card with its yield, rent band and sale band" width="280"><br>
  <em>Phone: the same guide, one colony card at a time. Demo figures.</em>
</p>

### Shows its *working*.

```mermaid
flowchart LR
  M["Pricing matrix<br/>curated bands per colony"] --> G[Price guide]
  M --> R["Roofie's answers"]
  M --> A[Agency pages]
  M --> S[Lead budget score]
```

#### What makes it different
1. **Medians, not averages;** 25th–75th percentile bands; no figure from fewer than 6 listings (`MarketReport`).
2. **Asking prices and desk quotes kept apart:** live asking prices in the report, the desk's curated bands in the guide.
3. **One matrix feeds** the guide, Roofie and the CRM's lead budget score (`PricingMatrixLookup`, `RoofiePriceGuide`, `RequirementScore`).

![Market report on desktop: "What South Delhi asks, colony by colony", median asking rents and sale prices from live inventory with the sample size](screenshots/report-desk.jpg)

*`/reports/south-delhi-rental-market` · Market report, desktop: medians from live inventory, with the sample size beside every figure. Demo figures.*

<p align="center">
  <img src="screenshots/report-phone.jpg" alt="The market report on a phone: 'How these numbers are made', explaining the source, medians, priced rows only and a floor of six listings" width="280"><br>
  <em>Phone: the method printed above the tables. Demo figures.</em>
</p>

![Agency page for Defence Colony on desktop: "What Defence Colony costs right now", with sale and rent bands from the pricing desk](screenshots/agency-costs.jpg)

*`/real-estate-agency/defence-colony` · Agency page: "What Defence Colony costs right now", from the pricing desk, not a portal average. Demo figures.*

---

## 06 · Roofie

### A front desk that follows a *script*.
Roofie is a scripted, rule-based enquiry assistant, not AI. One visitor, one thread, eight steps. *Ringed in orange: what's new at each step.*

**How the script works**
1. **Fixed moves.** Show matches, quote a price band, save a search, request a visit, take an enquiry, hand over.
2. **Sign-in inside the chat.** A mobile number and a one-time code, without leaving the thread.
3. **A person at the end.** Any thread can pass to the team (steps 5–8).

**119** chats since 7 Sep; 85% never needed an agent. · *6 Nov 2026*

**Steps 1–4**

| 1 · Say it your way | 2 · What's fair here |
|:---:|:---:|
| <img src="screenshots/roofie-s1.jpg" alt="Roofie step 1: the visitor types a 3 BHK brief for Vasant Vihar and Roofie replies with the top 3 of 4 live matches" width="400"> | <img src="screenshots/roofie-s2.jpg" alt="Roofie step 2: asked for the typical rent of a 3 BHK in Vasant Vihar, Roofie quotes the colony's band" width="400"> |
| A typed brief becomes matches from live stock. | Asked about price, it quotes the colony's band. |
| **3 · Save this search** | **4 · Verify by OTP** |
| <img src="screenshots/roofie-s3.jpg" alt="Roofie step 3: to save the search, Roofie asks for a mobile number inside the chat, with a Send code button" width="400"> | <img src="screenshots/roofie-s4.jpg" alt="Roofie step 4: a code has been texted to a masked number and the visitor enters it in the thread to verify and sign in" width="400"> |
| Saving asks for a mobile number, in the chat. | The code is sent and checked in the thread. |

**Steps 5–8**

| 5 · Search saved | 6 · Request a visit |
|:---:|:---:|
| <img src="screenshots/roofie-s5.jpg" alt="Roofie step 5: the visitor is signed in as Demo Guest and Roofie asks what they are after" width="400"> | <img src="screenshots/roofie-s6.jpg" alt="Roofie step 6: the visitor asks to visit listing VAV102 on Saturday at 11 am and Roofie shares the request with the team to confirm" width="400"> |
| Signed in, the search waits on their dashboard. | Listing, day and time go to the desk to confirm. |
| **7 · Enquire on a listing** | **8 · Callback booked** |
| <img src="screenshots/roofie-s7.jpg" alt="Roofie step 7: an enquiry about listing VAV72 is sent and noted against the visitor's brief" width="400"> | <img src="screenshots/roofie-s8.jpg" alt="Roofie step 8: the visitor asks to talk to a person after hours and Roofie sets up a callback inside office hours" width="400"> |
| Logged against the listing and the brief. | After hours, "call me" becomes a callback. |

### And a person, *when asked*.
Visit, enquiry and callback requests become tasks for the team; a callback goes to the agent who already owns the lead.

**The hand-off rule** · *"Can I talk to a person?"*

| Desk open | After hours |
|---|---|
| The chat is flagged in the CRM's chat inbox for an agent to take over. | Roofie books a callback inside office hours. |

**Scripted by design.** No external API and no LLM, as the owner required (Roofie spec). Paperwork and viewing questions are answered from the FAQ the team edits in the CRM, so editing an answer changes Roofie's reply.

### A chat on a listing becomes a *lead*, with its source.

| **20** | **115** |
|---|---|
| organic listing enquiries, all through Roofie on the listing page; **11 from Google search**. | Roofie chats since go-live on 9 Sep: 51 started on a listing page, 33 linked to a lead. *9 Sep → 6 Nov 2026* |

| On the listing → | In the CRM inbox → | CRM · Enquiry |
|:---:|:---:|:---:|
| <img src="screenshots/roofie-listing.jpg" alt="Roofie opened on listing VAV102: the listing card, an enquiry sent, and buttons to check availability, request details, WhatsApp or call" width="260"> | <img src="screenshots/crm-thread.jpg" alt="The same Roofie thread in the CRM's chat inbox on a phone, with a Take over button for the desk" width="200"> | <img src="screenshots/found-us.jpg" alt="CRM enquiry panel 'How they found us': channel Google search, organic; captured by Roofie, property enquiry; listing asked about, first page and first visit" width="320"> |
| Roofie opens on the listing being viewed (#VAV102) and offers availability, details, WhatsApp or a call. | The desk takes over in one tap. | Channel (Google search · Organic) and capture (Roofie · Property enquiry) kept apart, with the first page and first visit. A separate demo lead, not the chat shown. |

Ad and social links are tagged in the CRM's own link builder. **The full lead journey →** [Real Estate Platform — CRM & operations](https://github.com/abBytes-sudo/real-estate-crm-showcase)

#### What makes it different
1. **Channel ≠ capture:** a visitor who googled, then used Roofie, reads "Google search" + "Roofie", so search gets credit for the lead (`LeadChannel`; owner, 20 Oct 2026).
2. **Capture first:** a typed number becomes a callable lead, even if the OTP step is dropped (`RoofieSignup`).
3. **Roofie labels, people qualify:** it tags the lead and notes why, but never marks it qualified (`RoofieQualifier`).
4. **Browsing never creates a lead;** only an explicit action does (Roofie spec).

---

## 07 · Listings

### A listing page that says what was *checked*.

| **6,564** | **82** |
|---|---|
| active listings published straight from CRM inventory. *6 Nov 2026* | of the 499 engaged Google visitors since 11 Sep landed on a listing page. *6 Nov 2026* |

![Property page on desktop: photo gallery, Enquire, Save and Share, the property details the team verified, and Roofie open on this listing](screenshots/prop-desk.jpg)

*`/property/…` · Property page: gallery, Enquire / Save / Share, the details the team verified on the ground, and Roofie, the scripted assistant, already on this listing.*

| Phone | Verified, floor by floor |
|:---:|:---:|
| <img src="screenshots/prop-phone.jpg" alt="The same property page on a phone: price, a 'Verified by our team' badge and a sticky Enquire bar" width="260"> | <img src="screenshots/prop-units.jpg" alt="Verified by us block: listed by our team and photographed in person with dates, then 'Other units in this building'" width="360"> |
| The same listing: price, "Verified by our team", sticky Enquire bar. | When each fact was checked, and the building's other units (phone view). |

#### What makes it different
1. **Floor-by-floor stock.** Builder floors are rented and sold by floor, so each page lists the building's other units and compare has a Floor row (`CompareController`).
2. **Never advertises a let or sold home.** Publish refuses it; old links redirect to live listings in that colony, deal and BHK (`WebsitePublisher`, `PropertyController`).
3. **Fewer pop-ups.** One nudge per visit on phones, after a customer said there were too many (owner, 22 Oct 2026).

### Everything a renter comes *back* for.
Compare side by side, advisor shortlists shared as one link, and written guides for 77 colonies.

**Around the listings**
- Compare up to four, with a Floor row
- Advisor shortlists shared as one link
- "Not interested" clears a pick
- Written guides for 77 colonies
- Save to a shortlist with a phone number

![Compare page on desktop: two 3 BHK listings side by side with configuration, built-up area, floor, furnishing and locality rows, each with an Enquire button](screenshots/compare-hero2.jpg)

*`/compare` · Compare: up to four listings side by side, each one an Enquire tap away.*

<p align="center">
  <img src="screenshots/shortlist-two.jpg" alt="Shared shortlist 'Handpicked for you': two verified 3 BHK homes an advisor picked, each with Enquire and Not interested" width="560"><br>
  <em><code>/shortlist</code> · Shared shortlist: homes an advisor picked for one client, each with Enquire and "Not interested".</em>
</p>

![Locality guides index on desktop: "The colonies we know best, written up by the people who work them", a colony search and the South Delhi group](screenshots/localities-index.jpg)

*`/localities` · Locality index: every colony guide in one place, searchable, with a link to rent and sale bands. Demo counts.*

---

## 08 · Customer dashboard

### Signed in with a phone, *no password*.

**In the account**
- Save properties to a shortlist
- Track every enquiry and its status
- See requested visits
- Pick up the thread with the desk
- Edit their own brief (a CRM requirement)

![Customer dashboard on desktop: "Hello, Demo" with counts for saved properties, open enquiries, visits booked and new matches](screenshots/cust-dash.jpg)

*`/dashboard` · Dashboard: saved homes, open enquiries, visits and new matches, all read from the person's CRM record. Demo account.*

<p align="center">
  <img src="screenshots/cust-phone.jpg" alt="The customer dashboard on a phone: the same four tiles for saved properties, open enquiries, visits booked and new matches" width="280"><br>
  <em>Phone: the same dashboard, from the same CRM record.</em>
</p>

![Sign-in page on desktop: "Sign in or create an account" with a mobile number field, a Send me the code button and what happens next](screenshots/signin.jpg)

*`/account` · Sign in: a mobile number and a one-time code; no password.*

#### What makes it different
1. **No separate customer table.** The OTP-verified mobile is the account; the CRM enquiry is the record (`WebCustomer`, `CustomerDashboardData`).
2. **Browsing needs no account;** saving or viewing never creates a lead by itself (`BehaviourRecorder`).
3. **A customer's own brief becomes a CRM requirement,** and the desk is told of edits (`CustomerRequirementController`).

---

## 09 · List your property

### Owners list on the site; the desk *checks first*.

#### What makes it different
1. **Nothing an owner types goes live unchecked.** Figures stay free text until the desk verifies them and creates the listing itself (`ListPropertyController`).
2. **Owners and brokers get their own lists,** so neither lands in the sales pipeline as a client enquiry (`PropertyLeadsScreen`, `BrokerCallbacksScreen`).
3. **Broker numbers are never written to leads,** so they can't inflate lead counts (`RoofieBrokerCallback`).

![CRM list-your-property desk on desktop: owner submissions from the website with status filters New, Verifying, Listed and Dropped; owner phones masked and assignees blurred](screenshots/lyp-desk.jpg)

*CRM · List-your-property · The desk: owner submissions from the website arrive in the CRM as New, then Verifying, Listed or Dropped. Demo data.*

<p align="center">
  <img src="screenshots/lyp-phone.jpg" alt="The same list-your-property desk on a phone: submission cards with status tags and masked owner numbers" width="280"><br>
  <em>Phone: the same desk for agents away from a laptop.</em>
</p>

**11** owner submissions since the form went live on 20 Sep 2026

| Reviewed | Listed | Dropped | New |
|---:|---:|---:|---:|
| 10 | 6 | 4 | 1 |

All rentals: 8 residential, 3 commercial. A working supply channel, not a growth claim. · *6 Nov 2026*

---

## 10 · The journal

### A journal built for colony *deep-dives*.
A blog with a featured guide, filters for guides and localities, and pieces written by the desk.

![Journal home on desktop: "Notes on the Delhi NCR market, from the desk that works it", category filters, a featured guide and the latest pieces](screenshots/blog-desk2.jpg)

*`/blog` · Journal home: featured guide up top, then the latest pieces by category.*

<p align="center">
  <img src="screenshots/blog-phone.jpg" alt="The journal on a phone: All, Guides and Localities filters above the featured guide" width="280"><br>
  <em>Phone: Guides and Localities filters above the featured piece.</em>
</p>

**37** published posts (18 blog, 19 news); 11 drafts or scheduled. · *6 Nov 2026*

1. **Staff run it from the CRM:** draft, schedule or publish, with each post's category, cover and featured flag (`WebsiteBlogScreen`).
2. **The rest of the site, without a developer:** homepage, new pages from ready-made blocks, menus, footer and FAQ, under separate permissions (`SectionCatalog`).

### Laid out for *reading*.
Who each colony suits, in the desk's own words, then up to three related reads.

![Journal article on desktop: "Defence Colony vs Greater Kailash: which fits your brief?" with sections on the feel, rent and connectivity](screenshots/article-desk2.jpg)

*`/blog/defence-colony-vs-greater-kailash` · Article: a colony comparison laid out for reading: the feel, rent, connectivity.*

<p align="center">
  <img src="screenshots/article-phone2.jpg" alt="The same Defence Colony vs Greater Kailash article on a phone at reading size" width="280"><br>
  <em>Phone: the same piece at reading size.</em>
</p>

<p align="center">
  <img src="screenshots/related.jpg" alt="'More from the journal' block at the end of an article, linking a related guide" width="560"><br>
  <em>End of every article · More from the journal: every piece ends with related reads.</em>
</p>

3. **Scheduled posts go live on time** and the web team is told once (`NotifyPublishedBlogs`).

**37** of the 499 engaged visitors from Google search since 11 Sep landed on the journal. · *6 Nov 2026*

---

## 11 · How it was built

### One codebase with the CRM. *AI-assisted*, owner-directed.
1. **Requirements and product decisions.** I gathered what the desk and visitors needed and made the calls.
2. **Built with AI coding tools.** I directed the tools and tested every change before it shipped.
3. **Shipped with the CRM.** Site and self-hosted CRM replaced a 12-seat subscription CRM in 3 months (Jun–Sep 2026); production cutover 9 Sep 2026. I ran go-live and training.
4. **Before this version.** Earlier versions of the site were built by outside teams I coordinated.

```mermaid
flowchart LR
  CRM["CRM<br/>inventory · leads"] -- listings publish --> WEB["Website<br/>search · guides · Roofie"]
  WEB -- enquiries come back --> CRM
```

**Stack:** Laravel 13 · Blade + Livewire · Alpine.js · Tailwind CSS v4 (`@theme` tokens) · MySQL (shared with the CRM) · same codebase as the CRM · PHP 8.4 · phone-OTP customer area

**Design:** Tailwind v4 `@theme` tokens (Rubik + IBM Plex Mono; warm cream / navy ink / amber), no CDNs, mobile-first.

### See it live: try a sentence of *your own*.

| | |
|---|---|
| **Live site** | [rentaroof.in](https://rentaroof.in) |
| **Full write-up** | [abBytes-sudo / real-estate-listings-website-showcase](https://github.com/abBytes-sudo/real-estate-listings-website-showcase) (this page) |
| **The lead journey (CRM case study)** | [abBytes-sudo / real-estate-crm-showcase](https://github.com/abBytes-sudo/real-estate-crm-showcase) |
| **Try typing** | `3 bhk in vasant vihar under 1.5 lakh` |

---

## More screens: full pages from the demo build

Longer views from an earlier capture of the same demo build (placeholder brand "abBytes"; listing photos are random stock images standing in for real ones, any faces blurred; phone numbers masked, emails and the office address placeholders).

![Demo build, listings page on desktop: search bar, listing cards with prices and the Roofie quick-actions panel](screenshots/d-listings.jpg)

*Listings (demo build): search results with filters, compare tick-boxes and the Roofie quick-actions panel.*

![Demo build, property detail page on desktop: photo gallery, property details, verified-by-us block and what's around it](screenshots/d-property.jpg)

*Property detail (demo build): gallery, spec sheet, verified-by-us dates, other units in the building, what's around it, similar listings and the team's notes on the colony, top to bottom.*

![Demo build, compare page on desktop: two listings side by side with configuration, area, floor and furnishing](screenshots/d-compare.jpg)

*Compare (demo build): two listings side by side, with the Floor row.*

[![Demo build, locality guides index on desktop: header, colony search and the first colony cards for South Delhi](screenshots/d-localities-top.jpg)](screenshots/d-localities.jpg)

*Locality guides index (demo build): top of the page; select it for the [full page](screenshots/d-localities.jpg).*

![Demo build, locality guide on desktop: map, the team's notes on the area and what's around it](screenshots/d-locality-detail.jpg)

*Locality guide (demo build): the map, the team's notes on the area and what's around it.*

![Demo build, contact page on desktop: contact cards with a masked phone and a placeholder email, an enquiry form and office hours](screenshots/d-contact.jpg)

*Contact (demo build): contact cards (masked phone, placeholder email and office address), the enquiry form and a Roofie shortcut.*

| Listings | Property | Localities |
|:---:|:---:|:---:|
| <img src="screenshots/m-listings.jpg" alt="Demo build, listings page on a phone, full length" width="230"> | <img src="screenshots/m-property.jpg" alt="Demo build, property detail page on a phone, full length" width="230"> | <img src="screenshots/m-localities.jpg" alt="Demo build, locality guides index on a phone, top of the page" width="230"> |
| Listing cards stack into one column. | The whole property page on a phone. | Colony cards, one per row. |

| Locality guide | Contact | Compare |
|:---:|:---:|:---:|
| <img src="screenshots/m-locality-detail.jpg" alt="Demo build, locality guide on a phone, full length" width="230"> | <img src="screenshots/m-contact.jpg" alt="Demo build, contact page on a phone, full length, with masked phone and placeholder email" width="230"> | <img src="screenshots/m-compare.jpg" alt="Demo build, compare page on a phone, full length" width="230"> |
| Map, notes and nearby places, stacked. | Contact cards and the enquiry form. | Compare rows on a phone. |

---

## Designed & delivered (AI-assisted) by Abhishek M.
Operations & CRM lead. I design and deliver business software, AI-assisted.

**Live site:** [rentaroof.in](https://rentaroof.in) · **More work:** [github.com/abBytes-sudo](https://github.com/abBytes-sudo) · Related showcase: [Real Estate Platform — CRM & operations](https://github.com/abBytes-sudo/real-estate-crm-showcase)

© 2026 [@abBytes-sudo](https://github.com/abBytes-sudo). Write-up and screenshots shared for portfolio review; not licensed for reuse.
