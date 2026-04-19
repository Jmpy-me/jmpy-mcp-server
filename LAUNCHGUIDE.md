# Jmpy.me MCP Server

## Tagline
Dynamic URL Shortener, QR Code generator, & Marketing Analytics for AI Agents.

## Description
Official JMPY.me MCP Server providing AI agents with powerful tools for digital marketing. Shorten URLs with custom aliases, generate branded QR codes, track deep analytics (geo, device, clicks), and manage marketing campaigns directly through natural language. Fully compatible with Claude Desktop, Cursor, ChatGPT (via plugins), and any MCP-compliant environment.

## Setup Requirements
- `JMPY_API_KEY` (required): Your Jmpy.me API key used to authorize tool execution. Generate your key at [app.jmpy.me/dashboard/api-keys](https://app.jmpy.me/dashboard/api-keys).

## Category
Marketing & Social

## Use Cases
Marketing Automation, Link Management, Analytics Reporting, Dynamic QR Design, Growth Hacking, Conversion Tracking, Omni-channel Attribution

## Features
- **Dynamic URL Shortening**: Create professional, short jmpy.me links. Change the destination URL at any time without changing the short link—perfect for fixing broken links or A/B testing.
- **Branded & Custom Domains**: Build trust with custom branded domains and subdomains. Create memorable aliases like `jmpy.me/your-brand` for higher click-through rates.
- **Enterprise-Grade Analytics**: Real-time tracking of total clicks, unique visitors, and conversion rates. Monitor growth rates and compare performance against previous periods.
- **Deep Geographic Insights**: Track traffic down to the country, region, and city level. Visualize geographic distributions to understand where your audience is located.
- **Technographic Details**: Analyze visitor browsers, operating systems, device types (mobile, desktop, tablet), and preferred languages for precise targeting.
- **Advanced Traffic Attribution**: identify referral sources and mediums. Full UTM parameter support to track campaign effectiveness across all digital channels.
- **Multi-Content QR Code Engine**: Generate high-resolution (PNG/SVG) QR codes for URLs, WiFi networks, vCards, Text, Email, SMS, WhatsApp, and 40+ other content types.
- **Dynamic & Customizable QR Codes**: Design branded QR codes with custom colors, gradients, corner styles, and pattern dots. Add your logo for a professional look.
- **Offline-to-Online Tracking**: Track every scan of your QR codes with the same deep analytics as your short links. Monitor scan counts and last-scanned timestamps.
- **Campaign & Link Management**: Organize your links into campaigns for holistic reporting. Use tags and custom names for easy searching and bulk management.
- **Security & Privacy**: Protect sensitive links with password protection. Set expiration dates for time-sensitive offers. Links are continuously scanned for safety.
- **Bulk Operations**: Shorten multiple links at once or generate batches of QR codes. Integrated RESTful API for developers to automate marketing workflows.

## Getting Started
- "Shorten this link and make a QR code for it: https://example.com"
- "Show me how my marketing links performed in the last 7 days"
- "What are the top cities or countries clicking on my links?"
- "Create a new marketing campaign called 'Summer Sale 2024'"
- Tool: `shortenUrl` — Create a shortened link with optional custom alias, password, and expiration.
- Tool: `listUrls` — List your shortened URLs with filtering, search, and pagination.
- Tool: `updateUrl` — Edit an existing short link (change destination, name, or settings).
- Tool: `deleteUrl` — Permanently remove a shortened URL.
- Tool: `generateQr` — Create branded QR codes for URLs, WiFi, vCards, Text, and more.
- Tool: `listQrCodes` — View and manage your collection of generated QR codes.
- Tool: `getStats` — Get detailed click counts and performance trends for any link.
- Tool: `getGeographicStats` — Analyze traffic by country and city for specific URLs.
- Tool: `getDeviceAnalytics` — See which browsers and devices your audience uses.
- Tool: `getOverviewStats` — Access account-wide performance summaries and growth metrics.
- Tool: `listCampaigns` — Manage your marketing campaigns and grouped links.
- Tool: `createCampaign` — Start a new campaign to organize related marketing assets.
- Tool: `createSubdomain` — Setup a jmpy.me subdomain (e.g., brand.jmpy.me) for branded linking.

## Tags
url-shortener, qr-code, analytics, marketing, growth-tools, link-management, branded-links, mcp-server, dynamic-qr-code, short-urls, bitly-alternative, marketing-automation, link-tracking

## Documentation URL
https://jmpy.me/docs/mcp

## Health Check URL
https://jmpy.me/mcp/health
