# VTE evidence interfaces

This is an export prepared for an initial commit. It contains only two Daml interface files, the license texts and a few short notes about a Canton DevNet demonstration.

It does not contain the service, the API, the user interface or anything needed to reproduce the recorded runs.

The demo uses team-operated parties and synthetic data. The available evidence does not establish a full four-mode run with two real Loop wallets. Ledger commands are sent by demonstration parties, not by the wallet. Not a pilot, and we know of no customer using it.

The demo service stores the figures it is given. Nothing here promises absolute privacy. VTE does not check that a declared figure is true; it only looks at whether the declarations agree with each other.

## What is here

- `contracts/vte-evidence-api/`: a standalone Daml package with two interface files and no templates. See `docs/architecture.md`.
- `docs/`: two short notes, one on the package and one on what the notes report and what is not established.
- `evidence/README.md`: one page with aggregate results of the demonstration runs and their limits.
- `LICENSE`, `LICENSES/Apache-2.0.txt` and `NOTICE`: licensing and attribution.
- `MANIFEST.txt`: SHA-256 of every other file in the repository.

## What is not here

- No service, REST API, user interface, wallet code or recordings.
- No Daml implementation, test suite or participant configuration.
- No way to rerun or check the recorded runs from this repository alone.
- No claim about legal validity, custody, settlement or readiness for production use.

Some assertion messages inside the interfaces are in Spanish. They are left as written because changing them would change the package id, and this source must match the package that was built from it.

## License

This repository is licensed under the PolyForm Noncommercial License 1.0.0 (`LICENSE`). The licensor is Veridex Alethia Labs Ltd. One file, `contracts/vte-evidence-api/daml/VteHoldingInterfaceAPI.daml`, is adapted from the Splice token standard and stays under the Apache License 2.0 (`LICENSES/Apache-2.0.txt`). See `NOTICE` for the attribution, including the exact upstream files.
