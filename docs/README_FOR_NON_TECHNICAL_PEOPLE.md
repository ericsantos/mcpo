ocs/README_FOR_NON_TECHNICAL_PEOPLE.md</path>
<content lines="1-100">
# Welcome to mcpo!

## What is mcpo?

mcpo is a simple tool that helps make complex computer programs easier to use. Think of it like a translator for computers - it takes special commands from one type of program and makes them available through regular web technology.

Imagine you have a powerful but complicated tool, and you want to let others use it without needing to understand all the technical details. mcpo acts as a bridge between these complex tools and everyday users or other programs that expect standard web connections.

## Why Use mcpo?

mcpo makes your computer tools more accessible in several ways:

- **Easier Integration**: It converts special commands into standard web requests, making it compatible with common software
- **Better Security**: It adds protection features like authentication and secure connections
- **Clear Documentation**: It automatically generates helpful guides for each tool
- **Simpler Setup**: You can get started quickly without complex configurations

## How to Use mpo

Using mcpo is straightforward. Here are the basic steps:

1. **Install mcpo**:
   - If you have Python installed, you can install it with: `pip install mcpo`
   - Or use a package manager like uv for faster installation: `uvx mcpo`

2. **Run Your Tool**:
   - Use the command format: `mcpo --port 8000 --api-key "your-secret-key" -- your_tool_command`
   - Replace "your-tool-command" with the actual command that runs your program

3. **Access the Documentation**:
   - Once running, you can see all available tools at: http://localhost:8000/docs
   - Each tool will have its own documentation page at: http://localhost:8000/tool_name/docs

4. **Connect to Your Tool**:
   - Other programs or users can now connect to your tool using standard web protocols
   - No need for special software or complex setup

## Examples

### Example 1: Basic Setup

If you have a tool called "time-server" that shows the current time, you would run:

```bash
mcpo --port 8000 --api-key "my-secret-key" -- your_time_server_command
```

Then visit http://localhost:8000/docs to see how to use it.

### Example 2: Using Docker

For a more robust setup, you can use Docker:

```bash
docker run -p 8000:8000 ghcr.io/open-webui/mcpo:main --api-key "my-secret-key" -- your_tool_command
```

This makes your tool available on the internet with all the benefits of containerization.

### Example 3: Multiple Tools

If you have multiple tools, you can organize them:

```bash
mcpo --config /path/to/config.json
```

Where config.json defines each tool and its settings.

## Getting Help

For more detailed information or troubleshooting, please visit:
- GitHub repository: https://github.com/open-webui/mcpo
- Documentation site: https://docs.openwebui.com/openapi-servers/open-webui/

If you have questions about using mcpo with specific tools, feel free to ask for help from the community.