<!-- omit in toc -->
# ✨ MiniMCP Servers

![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)
![Python](https://img.shields.io/badge/python-3.10%2B-blue)
[![PyPI version](https://img.shields.io/pypi/v/minimcp-servers.svg)](https://pypi.org/project/minimcp-servers/)

MCP servers built with MiniMCP to expose Python’s standard library modules.

## Claude Desktop

Claude desktop can be configured to use the Math server as follows.

```json
{
    "mcpServers":
    {
        "math-server":
        {
            "command": "uvx",
            "args":
            [
                "--from",
                "minimcp-servers",
                "math-server"
            ],
            "env":
            {
                "MCP_SERVER_LOG_FILE": "/tmp/math_mcp_server.log"
            }
        }
    }
}
```
