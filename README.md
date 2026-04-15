# 💈 Philly Youth Haircare Platform

## “Community-funded dignity, one cut at a time.”

A mobile-first platform that enables communities in Philadelphia to fund haircuts for youth under 18 by connecting donors, trusted organizations, and participating barbers through simple booking, SMS coordination, and accountable payouts.

---

## 🧠 Core Idea

This is not just a booking app.

This is:
- a **community funding system**
- a **service dispatch platform**
- a **youth support infrastructure**
- a **barber payout network**

We are building a system where:
> A haircut can be funded, requested, fulfilled, verified, and paid out — reliably and at scale.

---

## 🔁 The Core Loop (MVP)

1. A haircut is funded (pool or partner allocation)
2. A youth or guardian requests a booking
3. A barber accepts via SMS
4. The youth arrives and checks in
5. The haircut is completed
6. The barber gets paid

If this loop works → the product works.

---

## 🎯 MVP Philosophy

We are not building a full marketplace yet.

We are building:
> the **simplest possible system that proves trust + fulfillment works**

---

## 👥 Users

### Youth
- Needs a haircut
- May request directly (depending on age)
- Receives check-in code

### Parent / Guardian
- Books on behalf of youth
- Receives confirmations and reminders

### Partner Organizations
- Schools, nonprofits, rec centers
- Distribute access / validate eligibility

### Barbers
- Opt in to participate
- Receive booking requests via SMS
- Accept or decline jobs
- Confirm check-in
- Get paid

### Admin
- Oversees system
- Manages funding, barbers, and disputes
- Approves payouts

---

## 📱 Product Features (MVP)

### 🧾 Booking
- Mobile-first booking flow
- Zip code-based routing
- Option to select a specific barber OR request nearby

### 📲 SMS Coordination
- Barber receives request via text
- Replies YES / NO to accept
- Automated confirmations to users

### 🔐 Check-In Verification
- One-time check-in code sent to user
- Barber confirms code at appointment
- Prevents fraud and false claims

### 💰 Funding System
- Central funding pool OR partner-based allocations
- Each appointment linked to a funded credit
- Fixed subsidy amount per haircut

### 💸 Barber Payouts
- Completed appointments → queued for payout
- Manual review (MVP phase)
- Weekly payouts

### 🧠 Admin Dashboard
- Track appointments
- Monitor funds
- Review flags
- Manage barbers

---

## 🧩 Key Design Decisions (Must Answer Before Build)

### 1. Eligibility
- Who qualifies?
- Open access vs partner-only?
- Guardian requirements?

### 2. Funding Model
- Pooled fund?
- Sponsored cuts?
- Partner-funded allocations?

### 3. Pricing
- Fixed haircut subsidy? (Recommended)
- Example: $25 per cut

### 4. Booking Logic
- Allow barber selection?
- Auto-route by zip?
- How many barbers receive a request?

### 5. Verification
- Is check-in code required? (Yes)
- Is barber confirmation enough?
- Do we need guardian confirmation?

### 6. Payouts
- Weekly or biweekly?
- Manual approval at first?

---

## ⚠️ Risks & Problems to Solve

### Fraud
- Fake bookings
- Code reuse
- Barber false claims

### No-Shows
- Youth doesn’t show up
- Barber loses time

### Supply / Demand
- Too many requests → not enough barbers
- Too many barbers → not enough funding

### Trust
- Barbers must trust payouts
- Users must trust availability

---

## 🛡️ MVP Anti-Fraud Strategy

- One-time check-in codes
- Code expiration window
- SMS logging
- Admin review of early payouts
- Partner-controlled access (initially)

---

## 🗺️ Scheduling Strategy (MVP)

NO full calendar sync yet.

Use:
- Availability blocks
  - e.g. Mon 3–6 PM
  - Sat 10–2 PM

Why:
- simpler logic
- easier SMS routing
- faster to build

---

## 🔄 Appointment State Machine
