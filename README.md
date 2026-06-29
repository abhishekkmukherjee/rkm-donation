# Ramakrishna Temple — Sponsor a Square Foot

A single-page UPI donation page for the Ramakrishna Temple, Ranchi.

Donors choose how many square feet to sponsor (₹2,100 each), then pay via:

- **Scan & Pay** — a QR code that fills in the amount automatically.
- **Pay via UPI** — opens the donor's UPI app (GPay / PhonePe / Paytm / BHIM) with the amount pre-filled.
- **Copy UPI ID** — for manual payment.
- **Share on WhatsApp** — invite others to contribute.

## Hosting

This is a static site (`index.html`). Deploy on Netlify by connecting this repo —
no build command or build directory is needed.

## Configuration

Edit the `CONFIG` block near the bottom of `index.html`:

```js
const CONFIG = {
  upiId:      "ramakrishnamissionas.99856572@hdfcbank",
  payeeName:  "Ramakrishna Mission Ashram",
  templeName: "Ramakrishna Temple, Ranchi",
  ratePerSqFt: 2100
};
```

## Note

UPI payment apps only open when the page is viewed **on a phone with a UPI app installed**.
On a desktop browser, use the QR code or copy the UPI ID.
