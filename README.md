# 109. Subscription Creep Tracker

Part of [AppADay](https://augustineiacopelli.github.io/appaday/) — one app, every day.

## What it does

Tracks recurring subscriptions and normalizes every one of them to a single monthly-equivalent cost, regardless of billing cadence, so the real size of your subscription spend is visible at a glance instead of hidden across weekly, monthly, quarterly, and yearly charges.

## Features

- Add, edit, and delete subscriptions with name, cost, billing frequency, renewal date, and category
- Smart statement scan: upload a CSV export or paste transaction lines, and the app groups charges by merchant, checks amount consistency and billing interval, and flags likely recurring subscriptions for one-tap add. Recognizes ~35 common subscription services by name (Netflix, Spotify, Adobe, and others) even from a single charge; unrecognized merchants need at least two consistent, recently active charges to surface. Entirely client-side, nothing is uploaded anywhere
- Every cost is normalized to a monthly equivalent through a single conversion function, so totals and comparisons are always apples to apples
- Summary strip showing total monthly and yearly spend, active subscription count, and anything renewing within 7 days
- Chart.js bar chart that toggles between spend by category and spend by individual service
- Sortable subscription list, click any column header to sort by name, monthly cost, or renewal date
- Renewal-soon flagging highlights any subscription due within a week
- Two-tap delete confirmation on each row, no browser confirm dialogs
- Data persists locally in the browser, nothing leaves the device

## Tech

Single self-contained `index.html`. Vanilla HTML, CSS, and JavaScript. Chart.js loaded from CDN for the bar chart. No build step, no other dependencies. Fonts via Google Fonts CDN (Fraunces, IBM Plex Sans, IBM Plex Mono).

## Category

Data Viz and Dashboards (D)

---

Built as part of a daily app-a-day discipline project. See the [full portfolio](https://augustineiacopelli.github.io/appaday/) for the rest of the archive.
