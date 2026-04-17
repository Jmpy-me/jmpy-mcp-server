# Jmpy.me Official MCP Server

Power your AI agents with 70+ advanced marketing tools from Jmpy.me. This Model Context Protocol (MCP) server allows your assistant to manage your entire marketing stack through natural language.

## 🚀 Key Capabilities

- **Dynamic Short URLs**: Branded link management with custom aliases and real-time updates.
- **QR Code Suite**: Generate and manage diverse, high-quality dynamic QR codes.
- **Deep Analytics**: Real-time click data tracking geography, device types, and traffic sources.
- **Landing Pages**: Deploy and manage marketing landing pages with AI-driven workflows.
- **Marketing Ecosystem**: Full access to 70+ specialized tools for campaigns and domains.
...


## 🛠️ Quick Setup

### 1. Get an API Key
Log in to your [Jmpy.me Dashboard](https://jmpy.me/dashboard/api-keys) and create a new API key with **MCP Channel** access.

### 2. Configure Your Client

#### For Claude Desktop
Add this to your `claude_desktop_config.json`:

```json
{
  "mcpServers": {
    "jmpy": {
      "command": "node",
      "args": [
        "-e",
        "const http=require('https');const req=http.request({hostname:'jmpy.me',port:443,path:'/mcp',method:'POST',headers:{'Content-Type':'application/json','x-mcp-key':process.env.JMPY_API_KEY}},(res)=>{res.pipe(process.stdout);});process.stdin.pipe(req);"
      ],
      "env": {
        "JMPY_API_KEY": "your_api_key_here"
      }
    }
  }
}
```

#### For Cursor / VS Code
Create a `.cursor/mcp.json` in your project and paste the same configuration as above.

## 🌐 Remote API
- **SSE Transport**: `https://jmpy.me/mcp/sse`
- **JSON-RPC Endpoint**: `https://jmpy.me/mcp`

## 📄 Documentation
For the full tool list and documentation, visit [jmpy.me/docs/mcp](https://jmpy.me/docs/mcp).
