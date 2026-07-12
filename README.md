# 🤖 Jmpy.me Official MCP Server

[![Status](https://img.shields.io/badge/System_Status-Online-green?style=for-the-badge)](https://jmpy.me/status)
[![MCP](https://img.shields.io/badge/MCP-Ready-blue?style=for-the-badge)](https://modelcontextprotocol.io)
[![Docs](https://img.shields.io/badge/Documentation-View_Docs-orange?style=for-the-badge)](https://jmpy.me/docs/mcp)

Unlock the power of **Jmpy.me** directly within your AI agents. This official **Model Context Protocol (MCP)** server provides a high-performance bridge for AI assistants (Claude, ChatGPT, Cursor) to manage branded links, dynamic QR codes, and deep marketing analytics using natural language.

---

## 🛠️ Performance-Grade Tools

Our MCP server exposes a rich suite of 72+ tools, optimized for AI discovery and execution:

### 🔗 Link Management
- `shortenUrl`: Create branded short links with custom aliases, password protection, and expiration.
- `updateUrl`: Change destination URLs in real-time without breaking existing short links.
- `listUrls`: Search and filter your link inventory with advanced pagination.
- `lookupUrl`: Detect existing short URLs for any destination to prevent duplicates.

### 🔳 Advanced QR Suite
- `generateQr`: Create dynamic, branded QR codes for URLs, WiFi, vCards, Text, and SMS.
- `listQrCodes`: Manage your entire library of visual assets.
- `customStyleQr`: (Coming Soon) Programmatic control over logo overlays and branding colors.

### 📊 Marketing Analytics
- `getStats`: Real-time performance metrics (clicks, uniqueness, growth rates).
- `getGeographicStats`: Deep-dive into traffic by country and city for precise targeting.
- `getDeviceAnalytics`: Analyze audience technographics (browser, OS, device type).
- `getOverviewStats`: Account-wide marketing health and performance summaries.

### 👥 Team & Campaigns
- `createCampaign`: Organize your marketing efforts into logical groups.
- `listCampaigns`: Track link performance at the campaign level.
- `createSubdomain`: Provision and verify custom subdomains (e.g., `brand.jmpy.me`).

---

## 🚀 Quick Setup

### 1. Obtain Your API Key
1. Sign in to [app.jmpy.me](https://app.jmpy.me).
2. Navigate to **Dashboard > API Keys**.
3. Create a key and ensure the **MCP Channel** is enabled.

### 2. Integration Guides

#### ☁️ Claude Desktop
Add this entry to your `claude_desktop_config.json`:

```json
{
  "mcpServers": {
    "jmpy": {
      "command": "npx",
      "args": [
        "-y",
        "jmpy-mcp-server"
      ],
      "env": {
        "JMPY_API_KEY": "your_api_key_here"
      }
    }
  }
}
```

#### 💻 Cursor / AI IDEs
Configure a **Remote SSE** connection in your IDE settings:
- **Type:** Server-Sent Events (SSE)
- **URL:** `https://jmpy.me/mcp/sse`
- **Auth Header:** `x-mcp-key: your_api_key`

---

## 💡 Example AI Prompts

- *"Shorten https://google.com/search?q=mcp-protocol with a custom alias 'mcp-guide' and make a QR code for it."*
- *"Check the analytics for my 'Summer Sale' campaign and tell me which city is clicking the most."*
- *"I need to redirect all links for jmpy.me/old-promo to a new destination: https://jmpy.me/new-landing."*

---

## 🛡️ Security & Reliability

- **Encrypted Transport:** All communication occurs over HTTPS with TLS 1.3.
- **Unified Auth:** Managed via the `x-mcp-key` header to ensure your account is only accessible by your authorized agents.
- **Bot Detection:** Integrated classification identifies and filters automated traffic for accurate marketing data.
- **Uptime Monitoring:** Real-time health checks available at [jmpy.me/status](https://jmpy.me/status).

---

## 📄 Resources
- **Organization Profile:** [github.com/jmpy-me](https://github.com/jmpy-me)
- **Technical Support:** [support@jmpy.me](mailto:support@jmpy.me)
- **Terms of Service:** [jmpy.me/terms](https://jmpy.me/terms)

Built with ❤️ for a better-connected web by the [Jmpy.me Team](https://jmpy.me).
