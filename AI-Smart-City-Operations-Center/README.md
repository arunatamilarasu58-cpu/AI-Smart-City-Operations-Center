# AI Smart City Operations Center (AISOC)

A front-end prototype of an AI-assisted Smart City Operations Center dashboard. It demonstrates how traffic, public-safety, and utility events could be monitored in one interface and how nearby cross-domain events could be grouped into incidents.

> **Prototype notice:** This repository currently contains a browser-based simulation, not a production AI system. Events, sensor counts, confidence values, and map locations are generated or represented in the front end. There is no live sensor integration, trained machine-learning model, backend API, database, authentication, or real emergency dispatch.

## Features demonstrated

- Dark operations-dashboard interface
- Traffic, public-safety, and utility event categories
- Simulated event feed with timestamps and severity labels
- Generated city-grid map with event markers
- Basic cross-domain event correlation using time and map-distance conditions
- Incident list with an acknowledge/resolve interaction
- Domain filters, KPI counters, and a scrolling activity ticker

## Run locally

No build step is required.

1. Download or clone this repository.
2. Open `index.html` in a modern web browser.

Optional: run a local static server from the repository folder:

```bash
python -m http.server 8000
```

Then open `http://localhost:8000`.

## Project structure

```text
AI-Smart-City-Operations-Center/
├── index.html
├── README.md
├── .gitignore
├── LICENSE
├── docs/
│   └── PROJECT_OVERVIEW.md
└── screenshots/
    └── .gitkeep
```

## Screenshots

Add genuine screenshots of the running prototype to the `screenshots/` folder. Suggested filenames:

- `dashboard.png` - full dashboard view
- `incident-feed.png` - incident panel and raw event feed

Do not use placeholder images as evidence of working features.

## Current limitations

- The event stream is randomly simulated in JavaScript.
- The city map is a generated schematic grid, not a geographic map.
- The displayed model-accuracy values are illustrative static values, not measured evaluation results.
- The correlation logic is a simple rule-based demonstration, not a trained AI model.
- Data is not persisted after refreshing the page.
- The page imports Google Fonts from an external service, so the font may fall back if offline.

## Future improvements

- Connect real or mock sensor APIs through a backend
- Store events and incidents in a database
- Add authenticated operator roles and audit history
- Replace the schematic map with a geographic map
- Evaluate and document actual ML models with datasets and metrics
- Add automated tests, accessibility checks, and responsive layouts

## License

See [LICENSE](LICENSE).
