# Multi-source docs

This example shows how multiple teams can publish to the same custom domain from independent repositories using Fern's [multi-source docs](https://buildwithfern.com/learn/docs/preview-publish/multi-source-docs) feature.

## Structure

In production, each folder would be its own repository. They are grouped here for demonstration:

```
multi-source/
├── homepage/     # Root of the domain — landing page with cards linking to each team
├── seeds/        # /seeds sub-path — seed catalog and planting guides
├── greenhouses/  # /greenhouses sub-path — climate control and monitoring
└── nursery/      # /nursery sub-path — plant care and propagation
```

Each folder contains a standalone `fern/` project with its own `docs.yml` and content. All four projects:

- Target the same base domain (`multi-source.docs.buildwithfern.com`)
- Set `multi-source: true` on their instance
- Share the same colors and logo (in production, use a [global theme](https://buildwithfern.com/learn/docs/customization/global-themes) instead of duplicating branding)

## Publishing

Each project publishes independently:

```bash
cd homepage && fern generate --docs
cd seeds && fern generate --docs
cd greenhouses && fern generate --docs
cd nursery && fern generate --docs
```

Updating one sub-path has no effect on the others.

## Learn more

See the [multi-source docs guide](https://buildwithfern.com/learn/docs/preview-publish/multi-source-docs) for the full setup instructions, including global themes and Dashboard configuration.
