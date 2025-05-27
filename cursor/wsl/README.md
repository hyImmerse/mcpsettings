# Cursor MCP Settings for WSL

This folder contains MCP configuration for Cursor IDE optimized for WSL (Windows Subsystem for Linux) environment.

## Files

- `mcp.json.template` - Template configuration file with placeholder values

## Installation

1. Copy the template file to your Cursor configuration directory:
   ```bash
   cp mcp.json.template ~/.cursor/mcp.json
   ```

2. Edit the `~/.cursor/mcp.json` file and replace the placeholder values:
   - `YOUR_ANTHROPIC_API_KEY_HERE`: Your Anthropic API key for Claude
   - `YOUR_GOOGLE_API_KEY_HERE`: Your Google API key
   - `YOUR_GITHUB_MCP_KEY_HERE`: Your GitHub MCP key
   - `YOUR_GITHUB_MCP_PROFILE_HERE`: Your GitHub MCP profile

3. Restart Cursor IDE to load the new MCP configuration.

## MCP Servers Included

### 1. TaskMaster AI
- **Purpose**: AI-powered task management and project organization
- **Package**: `task-master-ai`
- **Requirements**: Anthropic API key, Google API key

### 2. GitHub
- **Purpose**: GitHub repository management and operations
- **Service**: Smithery AI GitHub integration
- **Requirements**: GitHub MCP key and profile

### 3. Puppeteer
- **Purpose**: Web automation and browser control
- **Runtime**: Node.js with Puppeteer
- **WSL Optimized**: Configured with sandbox disabled for WSL compatibility

## WSL Specific Optimizations

- Puppeteer configured with `--no-sandbox` and related flags
- Chrome executable path set to standard WSL installation location
- Node.js paths configured for NVM installation in WSL

## Troubleshooting

### Chrome Installation in WSL
```bash
sudo apt update
sudo apt install google-chrome-stable
```

### Node.js Path Issues
Verify your Node.js installation path:
```bash
which node
```
Update the path in the configuration if different.

### Permission Issues
```bash
chmod 600 ~/.cursor/mcp.json
```