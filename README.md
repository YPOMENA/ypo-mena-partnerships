# MENA Partnerships Directory

A directory of restaurants, bars and clubs across the MENA region offering benefits to YPO members. Styled on the United MENA Playbook.

## What's inside

```
index.html   The full site (HTML, CSS and JavaScript in one file)
README.md    This file
vercel.json  Optional settings for deploying on Vercel
```

There is no build step. Open `index.html` in a browser to view it locally.

## Editing venues

All venues live in the `VENUES` list near the bottom of `index.html` (inside the `<script>` tag). Each venue has:

| Field | Example |
|---|---|
| `name`, `initials` | `'Gymkhana'`, `'G'` (shown in the round logo until a real logo is added) |
| `cat`, `catLabel` | `'restaurant'` / `'bar'` / `'club'` |
| `city`, `area` | `'Dubai'`, `'DIFC · Gate Village, Building 7'` |
| `cuisine`, `cuisineTags` | Display text, plus the list used by the Cuisine filter |
| `type` | Venue type, e.g. `'Fine dining restaurant'` |
| `website`, `booking` | Links (with `websiteLabel`, `bookingLabel`) |
| `short`, `quote`, `desc` | Card summary, snapshot headline, description paragraphs |
| `offer`, `terms` | Member offer (standard: 20% off the food bill) and its terms |
| `hours`, `dress`, `note` | Fact list on the snapshot |
| `member` | `name`, `role`, `initials`, `url` (YPO Connect profile) |

To add a venue, copy an existing entry, change the values and add it to the list. New cuisines or cities also need an `<option>` in the matching filter.

## Publishing with GitHub Pages

1. Create a new repository on GitHub and upload these files (keep `index.html` at the top level).
2. Go to **Settings → Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**, select `main` and `/ (root)`, then **Save**.
4. The site appears at `https://<your-account>.github.io/<repo-name>/` after a minute or two.

## Publishing with Vercel

Import the GitHub repository in Vercel. No framework or build command is needed.

## Before going live

- Replace the initials in the round logo with each venue's logo.
- Confirm each member offer with the venue.
- Confirm the Gymkhana website address.
- Make the repository private if the content should stay internal to YPO.
