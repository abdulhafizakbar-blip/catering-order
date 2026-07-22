# 🍱 Catering Order Form

A single-file WhatsApp catering order form. Customers fill in their details and
select quantities — hitting **"Order via WhatsApp"** opens WhatsApp with the
entire order pre-typed. They just press send.

**No backend. No dependencies. Works on any browser, including mobile.**

---

## Customising

Open `index.html` in any text editor and change these two sections near the top
of the `<script>` block:

### 1. Your WhatsApp number
```js
const WHATSAPP_NUMBER = "60123456789"; // country code, no + or spaces
const CURRENCY = "RM";
```

### 2. Your menu
```js
const MENU = [
  { name: "Nasi Lemak Set",    price: 12.00 },
  { name: "Chicken Rendang",   price: 15.50 },
  // add a line to add a dish, delete a line to remove one
];
```

Save → refresh browser → done.

---

## Hosting (free)

### Netlify Drop (fastest)
1. Go to https://app.netlify.com/drop
2. Drag the `index.html` file (or this folder) onto the page
3. You get a public URL instantly

### GitHub Pages
1. Push this repo to GitHub (already done if you're reading this)
2. Go to **Settings → Pages** → Source = `main` branch, `/root` → Save
3. Your link will be `https://<username>.github.io/catering-order/`

---

## Test checklist
- [ ] Set real WhatsApp number
- [ ] Update menu items and prices
- [ ] Open locally → add quantities → total updates live
- [ ] "Order via WhatsApp" only enables when total > 0
- [ ] Tap it → WhatsApp opens with full order pre-typed
- [ ] Test on a phone browser
