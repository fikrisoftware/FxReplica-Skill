# Brand: clone of replica-skill

Status: draft. No name check has been run. Angle is not set (see fixes.md: evidence too thin).
Note: the folder and target repo are both called "Replica-Skill", which is the original's name. Rename before any public release.

## Step 1: name

Candidates (20), grouped by style:
- descriptive: Appcloner, Cloneflow, Flowmap, Buildpath
- compound: Mapforge, Slotmap, Specbridge, Blueprintly (rejected: "-ly" twin pattern)
- invented: Remix-style coinages, Kalro, Mavio, Trelis, Orvane
- metaphor: Blueprint, Scaffold, Tracer, Harbor, Draftsman
- verb: Trace, Map, Rebuild

Cut to 5 (not confusingly similar to "replica", short, spellable):

| name | style | why |
| --- | --- | --- |
| Tracemap | compound | says "recon then map", no overlap with "replica" |
| Scaffold | metaphor | fits architect and build steps; very generic, weak for trademark |
| Orvane | invented | short, distinct; no meaning |
| Draftpath | compound | draft to build path |
| Specbridge | compound | recon notes to spec to build |

Recommendation: Tracemap (descriptive of the recon-first flow, not close to the original).
Final pick is the user's. Run Step 2 first.

## Step 2: checks (none run)

| check | Tracemap | Scaffold | Orvane | Draftpath | Specbridge |
| --- | --- | --- | --- | --- | --- |
| US trademark (tmsearch.uspto.gov, class 9, 42) | to run | to run | to run | to run | to run |
| EU trademark (EUIPO eSearch / TMview) | to run | to run | to run | to run | to run |
| Canada (ised-isde.canada.ca) | to run | to run | to run | to run | to run |
| WIPO Global Brand Database | to run | to run | to run | to run | to run |
| domain (whois) | to run | to run | to run | to run | to run |
| App Store / Play / GitHub | to run | to run | to run | to run | to run |
| handles (X, Instagram, TikTok, GitHub) | to run | to run | to run | to run | to run |
| web search "name + category" | to run | to run | to run | to run | to run |

Screening only. Not legal clearance. Get a trademark lawyer before spending money on the name.

## Step 3: palette

Not done. `replica/design/tokens.json` does not exist yet (run `/replica-design` first), so `contrast.py` cannot be run.
Rule when done: primary hue from a different family than the original's; zero AA failures. The original's brand colours are not recorded, so `brand.json` `colors` is empty.

## Step 4: logo brief

- Idea: a traced outline turning into a map pin or grid (recon to map).
- Mark type: symbol plus wordmark.
- Must work at 16px favicon and a 1024px app icon.
- Deliverables: SVG, app icon 1024x1024 with no transparency for iOS, favicon set, social image 1200x630.
- Must not resemble the original's mark. Put the original's logo next to the drafts and check before use.

## Step 5: voice

Direct, not blunt. Practical, not dry. Honest, not hedgy.

| do | don't |
| --- | --- |
| "Run recon first." | "You might want to consider recon." |
| "No reviews found." | "Great news, nothing to report!" |
| "Thin data. Treat as a lead." | "Trending now." |
| "Needs your yes before it pushes." | "Oops, something went wrong." |
| "Out of scope: brand assets." | "We can't do that, sorry." |

Strings to rewrite once the product has a UI: the 10 most-seen strings (sign up, empty states, main button, confirmation, error). The pack has no UI, so none exist yet.

## Step 6: sweep

Run `python3 sweep.py . --config replica/brand.json` after the rename. Result of the last run is in the report below.
