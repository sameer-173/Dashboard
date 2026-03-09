# DigiSpace Frontend Task

Pixel-focused implementation of the provided DigiSpace dashboard design using React + TypeScript + Vite.

## Tech

- React
- TypeScript
- Vite
- Apache ECharts (`echarts` + `echarts-for-react`)
- Redux Toolkit + React Redux
- Vitest + Testing Library

## Fixed Resolution Used

The dashboard is built as a non-responsive layout at:

- `1366 x 768`

## Responsiveness

- This implementation is intentionally **not responsive** as per the task instruction.
- Layout is fixed for the above resolution to match the given design.

## Run Locally

```bash
npm install
npm run dev
```

## Build

```bash
npm run build
```

## Test

```bash
npm run test
```

## Notes

- Each dashboard card is implemented as an individual component.
- Design assets from the task folder are served from `public/assets`.
- Font used: `Poppins`.
- Color tokens used: `#3FFDE0`, `#E6EAF5`, `#FFFFFF`, `#000000`.
- Charts are implemented using **Apache ECharts**.

## Extra Credit Coverage

- Tests added with Vitest:
  - `src/store/cardsSlice.test.ts`
  - `src/pages/dashboardLayout.test.ts`
- Adaptive design added:
  - Card grid automatically switches to adaptive mode when the visible card count is not 5.
  - Redux state drives card visibility (`src/store/cardsSlice.ts`).
- TypeScript is used across app code and state management.
- State management library added:
  - Redux Toolkit + React Redux.
- Interactive functionality added:
  - Lights knob drag interaction (knob-only drag).
  - Lights control drives overall page ambient lighting in real time (temperature + on/off).
  - Functional cards for Water, Carbon, Energy, and Footfall (preset/data switching).
  - Sidebar persistent selected state with functional Home / Analyse / Control views.
  - Animated view transitions when switching sidebar modes.
  - Interactive profile avatar menu with status toggle.

## Submission Note

- This implementation intentionally follows the task instruction for a fixed, non-responsive layout.
- LinkedIn Profile: [www.linkedin.com/in/subhakanta-sahu-sam](https://www.linkedin.com/in/subhakanta-sahu-sam)
- Hosted URL: https://jazzy-cobbler-784f5a.netlify.app/ 
