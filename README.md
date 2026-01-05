# Unwrap AI Database

**Community-sourced information about AI services and their alternatives.**

## What This Is

This database powers the [Unwrap AI](https://github.com/xcqtnr/unwrap) browser extension. It contains information about AI services and potential free or lower-cost alternatives.

Every entry is contributed by the community based on personal experience. We don't make definitive claims — we provide data points to help users make informed decisions.

## Our Vision

We believe the AI ecosystem benefits when users can easily compare options. This database exists to:

- **Surface alternatives** that users might not discover on their own
- **Share community knowledge** about AI tools and their underlying technology
- **Encourage informed choices** without telling users what to do

We're not here to attack businesses. We're here to promote transparency.

## How It Works

The database is a simple JSON file that the Unwrap extension fetches. When you visit a listed site, the extension shows you the information we have on file.

```json
{
  "example.com": {
    "name": "Example AI",
    "category": "PDF Analysis",
    "base_model": "GPT-4",
    "price_text": "$20/mo",
    "alternative_name": "NotebookLM",
    "alternative_url": "https://notebooklm.google.com/",
    "reason": "Why users might consider this alternative",
    "system_prompt": "A prompt to try with the alternative",
    "confidence": 85,
    "contributor": "github-username"
  }
}
```

## Contributing

### Add a Site

Found a service you think should be listed? We welcome contributions from your personal experience.

**Option 1: Open an issue**
[Suggest a Site →](https://github.com/xcqtnr/unwrap-ai-db/issues/new?template=suggest-site.yml)

**Option 2: Submit a PR**
Add your entry directly to `database.json` following the schema above.

### Guidelines for Contributors

- **Be honest** — Only suggest sites you've personally used or researched
- **Provide evidence** — Include pricing info and why you believe an alternative exists
- **Stay neutral** — Describe, don't accuse
- **Include a working prompt** — Help users actually try the alternative

## Request Removal

If you represent a service listed in this database and believe the information is inaccurate or unfair, we want to hear from you.

**To request a review or removal:**

1. [Open an issue](https://github.com/xcqtnr/unwrap-ai-db/issues/new) with the subject "[Removal Request] Your Site Name"
2. Explain why you believe the listing is inaccurate
3. We'll review and respond within 7 days

We're not trying to harm businesses — we're trying to inform users. If your service adds genuine value beyond the alternatives we've listed, let us know and we'll update the entry.

## Database Fields

| Field | Required | Description |
|-------|----------|-------------|
| `name` | Yes | Display name of the service |
| `category` | Yes | Type (PDF Analysis, Writing, etc.) |
| `base_model` | No | Underlying AI model if known |
| `price_text` | Yes | Human-readable pricing |
| `savings_monthly` | Yes | Monthly cost in USD |
| `alternative_name` | Yes | Name of the free/cheaper alternative |
| `alternative_url` | Yes | Link to the alternative |
| `reason` | Yes | Why users might consider switching |
| `system_prompt` | Yes | A prompt to replicate functionality |
| `confidence` | Yes | Confidence score (0-100). Guidelines: High=90+, Medium=60-89, Low=40-59 |
| `last_updated` | Yes | Date of last verification |
| `contributor` | No | GitHub username of contributor |

## Disclaimer

This database contains community-sourced information and opinions. We do not guarantee accuracy and do not make definitive claims about any company's technology or business practices. Companies listed may provide genuine value beyond what alternatives offer. Users should conduct their own research.

## License

MIT — Use freely, contribute back.

---

*Part of the [Unwrap](https://github.com/xcqtnr/unwrap) project. Built to encourage transparency in the AI ecosystem.*
