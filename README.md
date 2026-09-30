# ROUTE 234

ROUTE 234 is a compact, operations-led Nigerian logistics template. Its layout borrows from waybills, dispatch ledgers and corridor boards instead of a conventional startup landing page.

## Stack

- React 18
- Vite 5
- TypeScript
- Tailwind CSS
- Frontend only; no backend or database

## Routes

- `#/` — tracking-first home and active network overview
- `#/services` — service levels and handling exclusions
- `#/routes` — corridor ledger and relay notes
- `#/track` — frontend-only waybill demonstration
- `#/business` — recurring pickup and fulfilment format
- `#/contact` — validated demonstration enquiry form

Hash routing keeps all routes compatible with static hosting.

## Setup and commands

```bash
npm install
npm run dev
npm run typecheck
npm run build
```

## Tracking demonstration

The tracking screen contains three static records in `src/App.tsx`:

- `R234-LAG-24091`
- `R234-ABJ-11884`
- `R234-PHC-07215`

The interface does not contact a carrier, store user data or claim to show live movements. Unknown references return an explicit no-match state.

## Customization

Routes, corridors, services and sample records are centralized near the top of `src/App.tsx`. Colors are controlled in `tailwind.config.js`; operational effects and layout details live in `src/index.css`. Replace the fictional telephone number, address and email before production use.

## Assets and licenses

- `public/images/lagos-delivery-rider.webp` — photograph by Fawaz Onakoya, “Motorbike Delivery in Rural Lagos, Nigeria,” downloaded from [Pexels](https://www.pexels.com/photo/motorbike-delivery-in-rural-lagos-nigeria-37405046/). Used under the [Pexels License](https://www.pexels.com/license/), which permits free website and template use. The local copy is an optimized WebP rendition.
- `public/images/route-network.svg` and `public/images/hub-yard.svg` — original schematic illustrations supplied with this template.

No third-party logos are included.

## Deployment

`vite.config.ts` uses `/route-234/` as its production base. The included GitHub Pages workflow builds and deploys `dist`, but no repository or deployment is created as part of the visual-acceptance phase.
