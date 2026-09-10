# Agents in the Offware organisation

Read this file before the first command in any `offware-apps` repository.
`constitution.md` beside it is the rule every app keeps; `apps/` holds each
app's own constitution, copied from its repository with the source and sha on
its first line. The app's own file wins where the copy has drifted, and the
copy is refreshed in the same change.

## Before writing

- Read `constitution.md` whole, then the app's file under `apps/`, then the
  repository's own `AGENTS.md`, `CLAUDE.md` and `specs/` where they exist.
- A feature that needs an account, or a server present at every use, is out
  of scope. Redesign it on downloaded data, make the network part opt-in and
  labelled, or stop and say why it cannot be built here.
- Where the app talks to a server, its API or protocol is open and documented,
  so anyone can run a compatible one or build on the app.
- A fact about the world comes from a named, openly licensed dataset with
  recorded provenance. Never invent a station, a boundary, a weight or a score.
- A data file is inert: parsed and validated, never evaluated.

## Before shipping

- The app works with the network off after its first load. Prove it with a
  test or a run, never with a claim.
- Nothing leaves the device without an explicit user action. Grep the diff for
  `fetch`, `XMLHttpRequest`, `sendBeacon`, `<script src` and
  `<link rel="stylesheet"`, and account for every hit.
- The app's own gates run: its constitution check, its Spec Kit flow where it
  uses one, its test suite.
- No commit, body, issue or comment claims AI authorship or discloses AI use.

## A new app

Joins the organisation once it keeps every rule in `constitution.md`, ships as
static files a free host serves, and carries its own constitution, copied into
`apps/` here. A single-file page joins under the same rules, its constitution
being the README section that states them.

## Words

- Offware: software that works switched off, and the organisation.
- Offgiciel: French for one Offware app, on the pattern of progiciel and
  ludiciel.
- Offline first: the app's whole job runs on the device; the network adds,
  never enables.
