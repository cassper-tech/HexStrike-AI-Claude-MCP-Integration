# HexStrike-AI-Claude-MCP-Integration
HexStrike-AI-Claude-MCP-Integration

**Overview**

This project documents the integration of HexStrike AI v6.0 with Claude Desktop through the Model Context Protocol (MCP), using Kali Linux as the security-tool execution environment.
The integration establishes an AI-assisted security testing workflow in which Claude Desktop communicates with the HexStrike MCP server, which connects to the HexStrike AI API and authorized security tools available on Kali Linux.
Integration Architecture
```text
Claude Desktop
      │
      │ MCP
      ▼
HexStrike MCP Server
      │
      ▼
HexStrike AI API
      │
      ▼
Kali Linux
      │
      ├── Nmap
      ├── Burp Suite
      ├── Nikto
      ├── SQLMap
      └── Other Authorized Security Tools
```

**Objectives**

Integrate HexStrike AI with Claude Desktop through MCP.
Configure Kali Linux as the security-tool execution environment.
Establish communication between Claude Desktop and HexStrike.
Verify HexStrike API health and MCP connectivity.
Validate controlled security-tool command execution.
Document the architecture, configuration, and validation process.
Demonstrate practical application of AI-assisted cybersecurity automation.

**Technologies**

Technology	Purpose

Claude Desktop	AI agent / MCP client
Model Context Protocol (MCP)	Communication layer
HexStrike AI v6.0	Security automation and tool orchestration
Kali Linux	Security testing environment
Python	HexStrike server and MCP components
SSH Port Forwarding	Secure connectivity between environments
Nmap	Command execution validation

**Environment**

AI Client: Claude Desktop
Security Platform: Kali Linux
HexStrike AI: v6.0
MCP: HexStrike MCP integration
API Port: 8888
Testing Scope: Authorized laboratory environment

**Implementation**

The integration was implemented using the following logical workflow:
Configure and run the HexStrike AI server on Kali Linux.
Expose the HexStrike API through the configured port.
Configure the HexStrike MCP client for Claude Desktop.
Establish connectivity between the client and HexStrike API.
Verify server health and version information.
Confirm that Claude Desktop reports the HexStrike MCP server as running.
Execute a controlled validation command.
Verify successful command completion and output.

**Validation**

The integration was successfully validated through:
HexStrike API health status: `healthy`
HexStrike version: `6.0.0`
Claude Desktop MCP server status: `Running`
Controlled command execution through HexStrike
Validation command: `which nmap`
Returned executable path: `/usr/bin/nmap`
Exit code: `0`

These results demonstrate that the MCP integration was operational and that HexStrike could successfully execute an authorized security-tool environment command.

**Screenshots**

Claude Desktop — HexStrike MCP Running
![Claude Desktop HexStrike MCP](Screenshots/01-claude-desktop-mcp-running.png)
HexStrike MCP Client Connection
![HexStrike MCP Client](Screenshots/02-hexstrike-mcp-client-connected.png)
HexStrike AI Server
![HexStrike AI Server](Screenshots/03-hexstrike-ai-server-running.png)
API Health Validation
![HexStrike API Health](Screenshots/04-hexstrike-api-health.png)
Security Tool Execution Validation
![Nmap Execution Validation](Screenshots/05-nmap-command-validation.png)
> If your existing screenshot filenames differ, rename the files to the names above or update the image paths accordingly.

Documentation
Architecture
Setup Guide
Validation
Security and Legal Notice

This project is intended strictly for authorized cybersecurity research, education, testing, and laboratory environments.
HexStrike and the integrated security tools can provide powerful system and network security capabilities. They must only be used against systems, applications, networks, accounts, or data for which the operator has explicit authorization.

Do not use this configuration to perform unauthorized scanning, exploitation, credential attacks, persistence, data collection, or other intrusive activity.
For public documentation:

Do not publish passwords, API keys, authentication tokens, SSH private keys, session cookies, or other secrets.
Redact public/private IP addresses where disclosure is unnecessary.

Do not publish real customer data, credentials, proprietary information, or sensitive evidence.

Use intentionally vulnerable applications and isolated laboratory systems for demonstrations.

Review screenshots and command output before committing them to a public repository.

The author assumes no responsibility for misuse of the techniques, software, or configuration documented in this repository.

**Skills Demonstrated**

AI-assisted cybersecurity automation
Model Context Protocol (MCP)
Security tool integration
Kali Linux
Linux administration
Python-based security tooling
Network security testing
Vulnerability assessment
Security automation
Technical documentation
Secure laboratory configuration
Validation and troubleshooting

**References**

HexStrike AI — Official Repository
Model Context Protocol

**Author**

Mudassar Ali Zaman

Cybersecurity | Vulnerability Assessment | Digital Forensics | GRC | Security Research
