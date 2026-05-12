# NDIS Service Agreement Generator

A free, open-source React app for NDIS service providers. It forecasts support hours and costs, generates quotes, and produces a formatted Service Agreement document — all in the browser, no backend required.

Deployed via Cloudflare Pages.

View the live demo here: https://ndis-sa-generator.pages.dev/

## Setup

### Prerequisites
[Node.js](https://nodejs.org/) 18+

### Install & run locally
```sh
npm install
npm run dev
```

Open `http://localhost:5173` in your browser.

### Configure your organisation
Edit the `PROVIDER_DETAILS` constant near the top of `src/App.jsx`:
```js
const PROVIDER_DETAILS = {
    name: 'NAME OF YOUR ORGANISATION',
    abn: 'ABN #',
    email: 'info@example.com.au',
    phone: '00 0000 0000',
    address: 'Address',
    website: 'https://example.com',
};
```

Replace the header and footer images at `public/images/header.png` and `public/images/footer.png` with your own branding (recommended size: 800×100px header, 800×80px footer).

### Deploy to Cloudflare Pages
```sh
npm run deploy
```

Build command: `npm run build` | Output directory: `./dist`

## Frameworks & Libraries

- [React](https://reactjs.org/)
- [Vite](https://vitejs.dev/)
- [Tailwind CSS](https://tailwindcss.com/) (via CDN)
- [docxtemplater](https://docxtemplater.com/) — Word document generation
- [Cloudflare Pages](https://pages.cloudflare.com/) — hosting

## Disclaimer

NDIS rates data is provided for estimation and forecasting purposes only. Always verify results against official NDIS Pricing Arrangements.
