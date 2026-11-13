# Project Overview

## Purpose

AISOC is a front-end concept for viewing events from three smart-city domains in one operations dashboard:

- Traffic
- Public safety
- Utilities

The prototype also demonstrates a simple rule-based mechanism that correlates selected events from different domains when they occur close together in time and map position.

## How the prototype works

1. JavaScript periodically generates a simulated event.
2. Each event is assigned a domain, event type, zone, severity, timestamp, and schematic map position.
3. The event is added to the raw feed and displayed as a marker.
4. The correlation routine checks recent events from other domains.
5. If its conditions are met and a random probability check passes, a combined incident is created.
6. An operator can acknowledge and resolve an incident in the interface.

## Important distinction

The current implementation is a simulation. It does not connect to real city infrastructure, receive real emergency reports, or run a trained deep-learning model. Any accuracy/confidence values shown in the UI are illustrative and should not be presented as validated model performance.

## Suggested next development stages

1. Separate HTML, CSS, and JavaScript into maintainable files.
2. Add a backend API and persistent event storage.
3. Define event schemas and validation.
4. Replace random data with a documented test dataset or sensor integration.
5. Implement and evaluate ML models; publish reproducible metrics.
6. Add security, privacy, accessibility, and operational safeguards before any real-world deployment.
