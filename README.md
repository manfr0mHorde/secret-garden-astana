# Secret Garden Astana — floral storefront demo

Independent static demonstration of a flower-shop ordering experience. **Not affiliated with Qalta** and not an official website of Secret Garden Astana.

## Features

- **Customer:** ready-made and made-to-order bouquets, search and filters, cart, delivery or pickup, customer phone and separate phone number for a remote Kaspi invoice, WhatsApp handoff.
- **Florist demo:** product catalog, create/edit/duplicate bouquets, photo management, sold/available status, simulated order list and statistics.
- **Design:** olive-green and soft-cream palette inspired by the publicly supplied Secret Garden Astana Instagram screenshot. Product pictures and prices are illustrative.

## Important: demo only

- Catalog changes and simulated requests are stored in browser `localStorage` and **do not sync across devices**.
- The florist demo mode has **no real login or access control**. Do not use it to manage real orders.
- WhatsApp links prepare messages but do not automatically send them; the customer must manually confirm. Contacting the actual shop is disabled by default for testing.
- A field for the Kaspi invoice phone **does not initiate a bank payment**. The florist must independently confirm availability and send an invoice using the shop's own Kaspi Pay.
- Demo statistics are not verified payments or completed sales.
- Obtain the shop owner's permission and ensure appropriate processing of customer personal data before real use.

## Local preview

```bash
python3 -m http.server 8000
```

Open `http://localhost:8000/`.

## GitHub Pages

Use this repository's root as the published site:

1. Open **Settings → Pages** in GitHub.
2. Under **Build and deployment**, choose **Deploy from a branch**.
3. Select `main` and `/(root)`, then click **Save**.
4. Expected URL: https://manfr0mhorde.github.io/secret-garden-astana/

All styles, scripts and images use relative paths so this deployment works at the project URL.

## Production roadmap

A real multi-shop product would need secure shop login, database and image storage, isolation of shop data, order status verification, proper delivery and payment handling, privacy controls, and a supported WhatsApp integration if automated messaging is ever needed.

<!-- Pages: verify a branch-based deployment after configuration. -->
