# Humanoid Robots Dataset

A research index of 615 humanoid robots, built while researching candidates for [Botlero](https://botlero.com) — a sourced, cited humanoid-robot spec directory.

## What this is

Each entry is a **candidate index record**, not a verified spec sheet: a robot's name, a source URL, and a verbatim quote confirming it's a real humanoid robot. Some entries also carry a `company`, `country` or `category` field, each with its own `*Evidence` quote+URL when stated by a source.

## What this is NOT

This file has **not** been through Botlero's verification pipeline (fetch → extract → gate-check every value against a verbatim quote → hand review). A `source given here` ≠ a verified spec. A growing subset of these robots — fully sourced, quoted and checked — is published live at **[botlero.com](https://botlero.com)**. Treat this file as a discovery/candidate list, not a dataset of confirmed facts.

## Format

`humanoid-robots.json` — a JSON array of objects:

| field | meaning |
|---|---|
| `name` | the robot's name as stated by its source |
| `company` / `companyEvidence` | maker, if stated (`{quote, url}`) |
| `country` / `countryEvidence` | design/HQ country code, if stated |
| `year` / `yearEvidence` | a year associated with the robot, if stated |
| `categories` / `categoryEvidenceUrl` / `categoryQuote` | use-case category, if stated |
| `sourceUrl` | the page this record was found on |
| `humanoidQuote` | the verbatim sentence confirming it's a humanoid robot |

A `null` field means no source stated it — nothing is guessed or filled in.

## License

Data: [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) — attribution: "Humanoid Robots Dataset, botlero.com".

## More

For fully verified specs — every value with its source, a verbatim quote, and the date it was checked — see [botlero.com](https://botlero.com).
