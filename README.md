# Nexus API Documentation

<p align="center">
  <img src="https://cdn.nexus.dev/logo.svg" width="120" alt="Nexus API">
</p>

<p align="center">
  <strong>The modern API for building scalable, intelligent applications</strong>
</p>

<p align="center">
  <a href="https://docs.nexus.dev">Documentation</a> •
  <a href="https://app.nexus.dev">Dashboard</a> •
  <a href="https://discord.gg/nexus">Discord</a>
</p>

---

## Quick Start

```bash
# Install the SDK
pip install nexus-sdk

# Make your first API call
from nexus import Client

client = Client(api_key="nx_live_xxxxxxxxxxxx")
user = client.users.me()
print(f"Logged in as: {user.email}")
```

## Features

- 🚀 **Lightning Fast** - Sub-50ms response times globally
- 🔒 **Enterprise Ready** - SOC 2 Type II certified, GDPR compliant
- 📚 **Comprehensive** - Full API reference with examples
- 🤖 **AI Agent Ready** - Optimized for AI coding tools
- 💻 **Multi-Language SDKs** - Python, Node.js, Go

## Documentation Structure

| Section | Description |
|---------|-------------|
| [Getting Started](/quickstart) | Quick start guide |
| [Authentication](/essentials/auth) | API key authentication |
| [API Reference](/api-reference/users/list) | Complete API documentation |
| [SDKs](/snippets/python) | Multi-language SDK examples |

## Installation

### Python

```bash
pip install nexus-sdk
```

### Node.js

```bash
npm install @nexus/sdk
```

### Go

```bash
go get github.com/nexus/sdk-go
```

## Example: Create a User

<Tabs>
  <Tab value="python" label="Python">
    ```python
    from nexus import Client
    
    client = Client(api_key="nx_live_xxxxxxxxxxxx")
    
    user = client.users.create(
        email="new@example.com",
        name="New User"
    )
    print(f"Created: {user.id}")
    ```
  </Tab>
  <Tab value="node" label="Node.js">
    ```javascript
    import { NexusClient } from '@nexus/sdk';
    
    const client = new NexusClient({ apiKey: 'nx_live_xxxxxxxxxxxx' });
    
    const user = await client.users.create({
      email: 'new@example.com',
      name: 'New User'
    });
    console.log(`Created: ${user.id}`);
    ```
  </Tab>
  <Tab value="curl" label="cURL">
    ```bash
    curl -X POST "https://api.nexus.dev/v1/users" \
      -H "Authorization: Bearer nx_live_xxxxxxxxxxxx" \
      -H "Content-Type: application/json" \
      -d '{"email": "new@example.com", "name": "New User"}'
    ```
  </Tab>
</Tabs>

## API Endpoints

| Resource | Endpoints |
|----------|-----------|
| Users | List, Get, Create, Update, Delete |
| Projects | List, Get, Create, Update, Delete |
| Analytics | Overview, Events, Metrics |
| Webhooks | Subscribe, Unsubscribe |

## Contributing

Contributions are welcome! Please read our [contributing guidelines](CONTRIBUTING.md) before submitting PRs.

## License

MIT License - see [LICENSE](LICENSE) for details.

---

Built with ❤️ by the Nexus team