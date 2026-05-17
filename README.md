# The Royal Court Event Center

Website for **The Royal Court Event Center, LLC.** — an event planning company founded in 2018 by Vanessa Greene, providing complete event coordination, venue selection, furniture rental, and event decorating services.

**Live site:** [royalcourteventcenter.com](https://royalcourteventcenter.com)

---

## Project Structure

```
royalcourteventcenter.com/
├── index.html              # Single-page application (HTML, CSS, JS all inline)
├── images/
│   ├── gallery/            # 61 event photos
│   ├── drapery/            # 16 drapery photos
│   ├── vanessa-greene.jpg  # Owner portrait
│   └── royal-court-event-center.png  # Business logo
├── favicon.ico
├── apple-touch-icon.png
├── robots.txt
└── CNAME                   # royalcourteventcenter.com
```

## Tech Stack

- **Pure static HTML** — no build step, no framework, no dependencies
- **Vanilla CSS** — embedded in `<head>`
- **Vanilla JavaScript** — embedded before `</body>`; handles SPA navigation, image galleries, and modal lightbox

## Pages (Single-Page Navigation)

| Page | ID | Content |
|------|----|---------|
| Home | `#home` | Our Story, owner bio (Vanessa Greene), Products & Services |
| Drapery | `#drapery` | 16-photo drapery gallery with lightbox |
| Gallery | `#gallery` | 61-photo event gallery with lightbox |

## Structured Data (Schema.org)

A JSON-LD `@graph` block in `<head>` covers:

- **`LocalBusiness` + `ProfessionalService`** — business identity, contact info, 5 service offerings via `hasOfferCatalog`
- **`WebSite`** — enables Google Sitelinks eligibility
- **`Person`** — Vanessa Greene linked as founder and owner

Validate at: [search.google.com/test/rich-results](https://search.google.com/test/rich-results)

### Known Schema Gaps

Adding the following to the JSON-LD block would further improve local SEO:

- `address` (PostalAddress) — unlocks the full Google Local Business rich result with map pin
- `openingHours` — business hours

## Development

No build process required. Edit `index.html` directly and open in a browser.

```bash
# Serve locally (Python 3)
python3 -m http.server 8080
# then open http://localhost:8080
```

## Contact

- **Phone:** [314.226.4111](tel:+13142264111)
- **Email:** [royalcourteventcenter@gmail.com](mailto:royalcourteventcenter@gmail.com)
