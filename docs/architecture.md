# The interface package

`contracts/vte-evidence-api/` is a Daml package with `sdk-version: 3.4.11`. It depends only on `daml-prim` and `daml-stdlib` and defines no templates. Canton requires interface definitions to live in a package that contains only interfaces, so that a party who wants to read a receipt can import this small package without any implementation.

## Files

- `daml/IVteRelianceReceipt.daml`: a receipt interface. Its view carries the subject, the relying party, the modes that were combined, an epoch and a validity window. It carries no amounts and no attestation details. One choice lets the declared relying party check whether the receipt is still within its validity window.
- `daml/VteHoldingInterfaceAPI.daml`: holding and metadata types adapted from the Splice token standard, under Apache-2.0. See `NOTICE`.

## Building

With the legacy `daml` assistant and SDK 3.4.11, run `daml build` inside `contracts/vte-evidence-api/`. The package id of the result is `b83c90c8bcbbbc5f2c4079afbe26dea926a9d9b503eb21a05748cb67d0e74845`.

## Not included

The package that implements the demonstration, the service and the user interface are not part of this repository.

Error messages and error names in the interface files are part of the source and some are written in Spanish. Changing them requires a new build and produces a different package id.
