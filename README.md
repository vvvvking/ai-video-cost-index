# AI video cost index — list price per minute (2026)

[![Seedance 2.5 price](https://aiapi-pro.com/badge/seedance-2-5.svg?v=2)](https://aiapi-pro.com/chinese-ai-api-pricing)

`/badge` serves a one-line SVG for any of the 111 models — [embed one](https://aiapi-pro.com/badge).

**Full table:** all 111 Chinese models with list prices in one page — [Chinese AI API pricing comparison](https://aiapi-pro.com/chinese-ai-api-pricing)

Thirteen video models normalised to one unit: **USD per minute of finished output**. Per-second rates are not comparable across providers, because resolution and native audio change the billing tier.

List prices checked **2026-10-30**. Every row links to the provider's own pricing page.

| Model | Resolution | Per second | 1 minute | 8 seconds | Source |
|---|---|---|---|---|---|
| Kling 2.6 | 720p | $0.042 | **$2.52** | $0.34 | [Kling](https://kling.ai/document-api/pricing/base/video.md) |
| Wan 3 | 480p | $0.050 | $3.00 | $0.40 | [Runway](https://docs.dev.runwayml.com/guides/pricing.md) |
| Runway Gen-4 Turbo | — | $0.050 | $3.00 | $0.40 | [Runway](https://docs.dev.runwayml.com/guides/pricing.md) |
| Kling 3.0 | 720p | $0.084 | $5.04 | $0.67 | [Kling](https://kling.ai/document-api/pricing/base/video.md) |
| Hailuo 3 | 768p | $0.100 | $6.00 | $0.80 | [Runway](https://docs.dev.runwayml.com/guides/pricing.md) |
| Kling 3.0 | 1080p | $0.112 | $6.72 | $0.90 | [Kling](https://kling.ai/document-api/pricing/base/video.md) |
| Runway Gen-4.5 | — | $0.120 | $7.20 | $0.96 | [Runway](https://docs.dev.runwayml.com/guides/pricing.md) |
| Kling 3.0 + native audio | 1080p | $0.168 | $10.08 | $1.34 | [Kling](https://kling.ai/document-api/pricing/base/video.md) |
| Veo 3.1 | no audio | $0.200 | $12.00 | $1.60 | [Runway](https://docs.dev.runwayml.com/guides/pricing.md) |
| Seedance 2.5 | 720p | $0.300 | $18.00 | $2.40 | [Runway](https://docs.dev.runwayml.com/guides/pricing.md) |
| Veo 3.1 | with audio | $0.400 | $24.00 | $3.20 | [Runway](https://docs.dev.runwayml.com/guides/pricing.md) |
| Kling 3.0 | 4K | $0.420 | $25.20 | $3.36 | [Kling](https://kling.ai/document-api/pricing/base/video.md) |
| Seedance 2.5 | 1080p | $0.680 | **$40.80** | $5.44 | [Runway](https://docs.dev.runwayml.com/guides/pricing.md) |

## Three things the rate card hides

1. **The resolution step is not linear.** Kling 3.0 is $0.112/s at 1080p and $0.42/s at 4K — 3.75x the price for 4x the pixels. If a shot only ships at 1080p, rendering at 4K "to be safe" is the most expensive habit in the table.
2. **Native audio is a flat +50%.** Same model, same resolution: $0.112/s silent, $0.168/s with audio. It never appears in comparison tables.
3. **Retries double everything.** These are first-take prices. At a 1-in-2 hit rate, 300 clips of 8 seconds is 4,800 generated seconds: about **$202** on the cheapest tier and **$3,264** on the most expensive.

## Why this exists

Most "AI video pricing" pages quote a per-second rate at one configuration and call it comparable. Normalising to output minutes — and counting the takes that do not ship — is the only way the number matches an actual invoice.

Rows sourced to Runway are the prices Runway publishes for those resold models; Kling rows are Kuaishou's own published rates. Spread across resellers for the same model is typically 0–7%, so the model choice dominates, not the reseller.

## Tools

- Interactive batch calculator: https://aiapi-pro.com/video-cost-calculator
- Image batch calculator: https://aiapi-pro.com/image-cost-calculator
- Sourced per-minute table (HTML): https://aiapi-pro.com/video-cost-2026
- Japanese / Portuguese / Spanish versions: `/ja/`, `/pt/`, `/es/` under the same path

Maintained by [NovAI](https://aiapi-pro.com), an OpenAI-compatible gateway for Chinese AI models at provider list price, 0% platform fee.

_No affiliate links. Prices belong to their respective providers._

Companion repos: [live price feed for 111 Chinese models](https://github.com/vvvvking/chinese-ai-api-prices) · [interactive calculator](https://vvvvking.github.io/novai-cost-index/).

Companion index: [AI image generation cost per image](https://github.com/vvvvking/ai-image-cost-index).
