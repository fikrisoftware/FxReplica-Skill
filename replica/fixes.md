# Fixes: replica-skill

Sample: 10 GitHub issues (Oct 9 to Nov 3, 2026), 1 source. Hacker News: 0 relevant hits.
Far below the 100+ reviews across 3 sources the method asks for. Issue titles only; bodies were not read.
Every theme below is thin. Treat as leads, not trends.

## What they hate (thin, 1 source each)

1. Plugin install fails. 1 issue, 1 source.
   "Plugin install fails to load: "Path escapes plugin directory: ./ (skills)"" https://github.com/Jakeschincariol/replica-skill/issues/18
2. imgdiff.py crashes with a raw traceback on a truncated PNG. 1 issue, 1 source.
   "imgdiff.py dies with a raw struct.error traceback on a PNG whose IHDR chunk is truncated, instead of its usual clean error" https://github.com/Jakeschincariol/replica-skill/issues/10

## What is missing

None stated by name. Nothing in the sample is a feature request for the pack itself.

## What is unsolved (inference, thin)

8 of 10 issues are title-only app ideas or greetings ("Instagram", "Klon", "App AI", "لعبة", ride-hailing for Yemen, "hello friend", "Replica", "replica"). Users file app requests in the issue tracker, so the repo gives no clear route for "what do I do first". Cannot confirm cause from titles alone.

## Fix plan

| # | fix | size | skill | evidence |
| --- | --- | --- | --- | --- |
| 1 | Make install path valid so plugin loads (no path escaping the plugin directory) | S | repo manifest | issue 18 |
| 2 | Catch truncated PNG in imgdiff.py, print a clean error | S | replica-diff | issue 10 |
| 3 | Add issue template and a README "start here" with an example prompt | S | repo docs | 8 of 10 issues, thin |
| 4 | Verify stack choices against current docs with context7 | S | replica-architect | internal observation, not from reviews; already applied in SKILL.md Step 1 |

## Angle

No positioning recommended. One source and 10 title-only items do not support a claim. Collect app-store, Reddit and HN feedback on the original, then rerun.

## Not done

Issue bodies, comments and any other source were not read. No reviews were invented.
