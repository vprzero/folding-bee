# 🐝 Folding Bee

Concierge in-home laundry folding & organizing — serving **Towson, Ruxton & Roland Park, Maryland**.

This is the complete website. It's a single self-contained file (`index.html`) — the design, content, photo, favicon, booking, and contact form are all baked in. No build step, no installs, no dependencies. Just upload and deploy.

---

## What's in this folder

- **`index.html`** — the entire website
- **`README.md`** — this file (instructions; does not appear on the site)

---

## Step 1 — Put it online (GitHub → Vercel)

You'll make two free accounts. No command line needed. Do this on a computer.

1. **GitHub:** go to github.com, sign up, verify your email.
2. **New repository:** click the **+** (top-right) → **New repository**. Name it `folding-bee`, keep it **Public**, click **Create repository**.
3. **Upload the files:** on the new repo page, click **"uploading an existing file,"** drag in `index.html` (and optionally `README.md`), then click **Commit changes**.
4. **Vercel:** go to vercel.com → **Sign Up** → **Continue with GitHub** → approve.
5. **Deploy:** in Vercel click **Add New… → Project**, find `folding-bee`, click **Import**, then **Deploy** (don't change any settings).
6. After ~30 seconds you get a live URL like `folding-bee.vercel.app`. That's the site.

To update the site later, just upload a new `index.html` to the same repo — Vercel redeploys automatically in seconds.

---

## Step 2 — Activate the contact form (1 minute)

The **"send a note"** form is built in, but needs one free key before it can deliver emails.

1. Go to **web3forms.com**, enter the email address where booking requests should arrive, and create an access key (it's emailed instantly).
2. Open `index.html` in any text editor, search for **`YOUR_ACCESS_KEY_HERE`**, and replace it with your key (keep the quotation marks). Save.
3. Done — every form submission now emails that inbox. The key is safe to leave in the public file; it only points *to* the inbox.

Free plan handles 250 submissions/month and includes basic spam protection.

---

## How booking works

- **"Choose your time" button** → opens the Google Calendar booking page. Booked slots land directly on the connected Google Calendar with an email confirmation.
  - *Currently connected to the test calendar `adriancuriel22@gmail.com`.* To switch to the business calendar later, create a new Appointment Schedule in that Google account, copy its booking-page link, and replace the calendar URL in `index.html`.
- **"Send a note" form** → emails the request (name, phone, email, neighborhood, service, notes) via Web3Forms once Step 2 is done.

---

## Not wired up yet (optional, for later)

- **Payments** — Stripe Payment Links for the VIP membership ($20/mo) and gift cards, or a tool like Koalendar that bundles calendar + reminders + payment.
- **Automatic reminders** — needs a paid Google plan or a scheduler like Koalendar/Calendly.
- **Custom domain** — buy one (~$12/yr) and connect it free in Vercel → Domains.
- **Google Business Profile** — the single biggest local-SEO boost; set one up once there's a business phone number.

---

*Built as a single static page. Coastal blue, light and airy. 🐝*
