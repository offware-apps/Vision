# Offware

Software that works switched off.

Offware is a family of apps for daily life, built offline first: each one
does its whole job on your device, with no signal, no server and no account.
The French word for one is an offgiciel, on the pattern of progiciel and
ludiciel.

## The promise

Every app published here keeps these rules. An app that cannot keep one is
not an Offware app.

1. It works with zero network after its first load.
2. It needs no account and no server of ours to do its job.
3. Nothing leaves your device unless you take an explicit action: an export,
   a share, a sync you configured.
4. Your data lives in one portable, human-readable file you can back up,
   diff and move anywhere.
5. Every fact about the world comes from a named, openly licensed dataset
   with recorded provenance. The app invents nothing.
6. Every network feature is opt-in, off by default and labelled, and the app
   stays whole without it.
7. Open source under AGPL-3.0, with open, replaceable components only: no
   proprietary SDK and no cloud dependency for any core feature.

An online service, where one exists, sits outside this promise under its own
name: the app never needs it.

## The apps

| App | What it does |
| --- | --- |
| [MAX Finder](https://github.com/offware-apps/MAX-Finder) | Every SNCF train where a free MAX seat is reservable, from open data. |
| [Postcards](https://github.com/offware-apps/Postcards) | Every place you have been, privately, in a file you own. |
| [CVSS Lens](https://github.com/offware-apps/cvss-lens) | A CVSS 3.1 vector read in plain words, scored in one file that fetches nothing. |

Shared pieces, the offline map store first, live here as packages every app
consumes, so one downloaded map serves them all.
