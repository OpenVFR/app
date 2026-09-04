# Contributing to OpenVFR

Thanks for your interest — source code is not yet public. This file is a
placeholder for governance once the initial codebase lands.

## Flight-critical changes

Any pull request touching flight-critical calculations must include test
coverage before merge. This includes, but is not limited to:

- Fuel burn and range calculations
- Weight & balance
- True airspeed / wind triangle math
- Magnetic variation / declination models
- Great-circle and geodesic distance/bearing calculations
- Airspace intersection / containment logic

## Data licensing

Do not add datasets, sample flight plans, or navigation databases without
confirming their license permits redistribution in this repository (see
README.md → Data & attribution). When in doubt, ask before committing.

## Secrets

Never commit API keys, tokens, or credentials. This repo will run
gitleaks in pre-commit and CI once source lands — treat any flagged
match as a hard stop, not a warning.
