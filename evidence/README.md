# Evidence: aggregate results and limits

This page summarizes recorded demonstration runs. It is a summary, not a record: the detailed records were kept outside this repository, and none of the runs can be reproduced from it. The public names of the four modes are VTE Match, VTE Trade Check, VTE Reveal and VTE Policy.

## Runs on Canton DevNet (5 October 2026)

- Four fictional cases were run with all four modes one after the other, then the results were combined. The summary reports that the ledger accepted every combination and that no step failed or was retried. It does not include the run records needed to check the elapsed time.
- The summary reports that all four cases were happy paths: every condition was met. A case in which a condition is not met was not run live.
- The summary reports that one case used figures read from committed demonstration assets and a consent from a stand-in wallet, which is a test double and not a real wallet. In the other cases the figures were typed from a preset.
- Four kinds of attempt were each run once; the summary reports that each was refused and paired with an accepted control.

## Runs on Canton TestNet (4 October 2026)

- The summary reports a VTE Trade Check run of 14 transactions, all accepted on the first attempt.
- The summary reports a run combining VTE Policy and VTE Trade Check of 15 transactions, all accepted on the first attempt, about 36 seconds from first to last.
- The same four kinds of attempt, each run once; the summary reports that each was refused and paired with an accepted control.
- The summary reports that in both runs a few transactions were signed outside the participant. The signatures were produced under the control of the team and no person approved them, so these runs do not show a user signing from their own wallet.

## Wallet

The notes report that on 6 October 2026 a login with a real Loop wallet on DevNet worked from the public demo. It was a login only. Consent signed with a real wallet and any command authorised by a wallet are not established.

## Limits

- The demo uses team-operated parties and synthetic data. The available evidence does not establish a full four-mode run with two real Loop wallets. Ledger commands are sent by demonstration parties, not by the wallet. Not a pilot, and we know of no customer using it.
- The team reports that every party in these runs used one participant node operated by the team; this export does not independently establish separation between operators. What the ledger shows about who sees what is not a complete privacy statement.
- The demo service stores the figures it is given.
- VTE does not show that a declared figure is true. If every party states the same false figure, every check passes. What can be detected is disagreement, not falsehood.
- The team reports that refusal-case test keys were generated for the runs and that their private halves no longer exist; this export does not independently establish key destruction.
- No source outside the team took part. The sum across several custodians in one case was simulated by a single demonstration source, so it does not show independence between custodians.
- Network traffic costs on DevNet were not measured.
- The results do not establish a live external source of truth, legal validity, custody, settlement or readiness for production use.
