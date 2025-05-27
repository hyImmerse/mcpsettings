# MCP Settings Repository

This repository contains Model Context Protocol (MCP) configuration files for different IDEs and environments.

## Repository Structure

```
mcpsettings/
├── cursor/
│   ├── normal/          # Cursor IDE settings for normal environments
│   └── wsl/             # Cursor IDE settings for WSL environments
└── vscode/
    ├── normal/          # VSCode settings for normal environments
    └── wsl/             # VSCode settings for WSL environments
```

## Available Configurations

### Cursor IDE
- **Normal Environment**: Standard desktop installation
- **WSL Environment**: Windows Subsystem for Linux optimized settings

### VSCode
- **Normal Environment**: Standard desktop installation  
- **WSL Environment**: Windows Subsystem for Linux optimized settings

## Usage

1. Navigate to the appropriate folder for your IDE and environment
2. Copy the template file to your IDE's configuration directory
3. Replace placeholder values with your actual API keys
4. Restart your IDE to load the new MCP configuration

## Security

⚠️ **Important**: All files in this repository are templates with placeholder values. Never commit actual API keys to version control.

## Contributing

Feel free to submit pull requests to add new MCP server configurations or improve existing ones.