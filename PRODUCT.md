# Product

<!-- impeccable:product-schema 1 -->

## Platform

web

## Users

Two audiences, weighted equally:

- **Delivery orderers:** hungry locals, mostly on a phone and mostly at night, browsing the menu to place a delivery order.
- **People at the truck:** customers in line or nearby who open the menu (for example from a QR code) to browse and pre-order for pickup.

Both need to find something they want fast, understand the price, and send an order with as little friction as possible.

Behind the fictional brand sits a second, real audience: prospective restaurant and food-business clients who evaluate this site as a portfolio piece.

## Product Purpose

Chispa is a **portfolio demo**: a fictional Venezuelan street-food truck whose web menu shows what a small food business can get. The menu lets a visitor browse by category, search, customize items, build a cart, and send the order by WhatsApp for delivery or pickup.

Success means a visitor can go from opening the page to sending a complete order on their phone without confusion, and a prospective client sees a menu they would want for their own business.

## Positioning

A menu that is the ordering channel: no app, no account, no payment gateway. The cart composes a ready-to-send WhatsApp message (items, options, notes, total, delivery mode, name, address), which matches how small Venezuelan and Latin American food businesses already take orders.

## Operating Context

- Visitors are on mobile, often at night, often outdoors or in line at the truck.
- Orders end in WhatsApp; the business confirms delivery cost and payment there. Pickup orders are paid at the truck.
- Content lives in a single editable `MENU` object (brand, categories, items, options, featured items, combos, promo, marquee, info), so the demo can be re-skinned with a real client's menu.

## Capabilities and Constraints

- Category navigation, search, item detail sheet with options and notes, quantity, cart with delivery/pickup toggle, name and address fields, WhatsApp hand-off.
- Cart and customer details persist locally in the browser.
- Structured data (schema.org `Restaurant` / `Menu`) is generated from `MENU`.
- All visible copy is in Spanish.
- Ordering is WhatsApp-only: no online payment, accounts, or checkout. This is binding.
- Menu items, prices, combos, promo, and hours are sample content and may change.
- Current implementation is one static `index.html` with no build step; that is the incumbent setup, not a binding constraint.
- Open: real address, WhatsApp number, and Instagram handle are placeholders (`[TU DIRECCIÓN]`, `[TU NÚMERO]`, `[TU USUARIO]`, empty `whatsapp`) and stay so until a real client adopts the demo.

## Brand Commitments

- Name: **Chispa** ("Comida callejera con chispa").
- Logo assets: `assets/chispa-logo.png`, `assets/chispa-logo-noche.png`, `assets/chispa-isotipo.png`.
- Voice: casual, warm Venezuelan Spanish street-food voice, with names and phrases like "Pa' picar", "Combo Pana", "Combo Rumba", "¡recién salidas!".

## Evidence on Hand

- Product photos in `assets/fotos/`: burger-chispa-doble, cachapa-queso, combo-rumba, papas-con-todo, papelon-limon, perro-full-todo, quesillo, reina-pepiada, tequenos-x12 (all `.webp`). Other items have no photo.
- No testimonials, reviews, ratings, press, order counts, or real customer data exist. The brand is fictional; do not invent social proof or claims that imply a real business.

## Product Principles

1. **Order in one hand.** Every path is designed for a phone at night: browse, choose, send.
2. **WhatsApp is the checkout.** The order message must be complete and correct enough that the business never has to ask what was meant.
3. **Menu as data.** Content stays in one editable structure so the demo can become any real client's menu without touching the interface.
4. **Truthful demo.** It should feel like a real truck without pretending to be one: no fake proof, placeholders stay visible as placeholders.
