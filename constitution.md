# Offware constitution

The rules every app in the `offware-apps` organisation keeps. An app that
cannot keep one is not an Offware app, whatever else it does well. Each app's
own constitution, under `apps/`, adds to these and never subtracts.

## I. Offline first

The app's whole job runs on the device, with the network off, after its first
load. A feature that needs a server present at every use is redesigned to run
on downloaded data, scheduled outside the app, or dropped.

## II. Self-reliant, no account

Nothing to sign up for. The app runs on data it downloaded, so nothing has to
be online when it is used, and static files on free hosting run it
indefinitely at zero cost. Where it talks to a server, the API or protocol is
open and documented, so anyone can run a compatible one or build on the app.

## III. Private by default

No telemetry, analytics, tracking or beacon. Nothing about the user leaves the
device unless they take an explicit, informed action: an export, a share, a
sync they configured.

## IV. One portable file the user owns

The user's data lives in one human-readable file they can read, diff, back up
and move anywhere, against a documented, versioned schema, and the app imports
it back without loss.

## V. Aggregator, never an author

Every fact about the world comes from a named, openly licensed dataset with
recorded provenance. The app invents nothing: where the data does not say, the
app does not claim.

## VI. Network is opt-in

Every network feature is off by default, labelled, and declined without loss:
the app stays whole without it. An online service, where one exists, sits
outside this constitution under its own name, speaks an open, documented API,
and the app never needs it.

## VII. Open and replaceable

Open source, AGPL-3.0 by default and MIT where the app is one file with
nothing to build. Open and replaceable components only: no proprietary SDK,
no Google, no cloud dependency for a core feature. Anyone can host a copy.

## VIII. Data is inert

A data file, the user's own or shared, is parsed and validated, never
evaluated: no code, no formula, no template.

## IX. Fast, accessible, keyboard-first

Mobile first, WCAG 2.1 AA, full keyboard operability, a small bundle, and a
working escape hatch on a low-end device.

## Governance

An amendment is a documented change to this file with its rationale. Every
app's plan carries a constitution check against these rules and its own, and
an unjustified violation blocks the merge.
