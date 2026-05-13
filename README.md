# Nexus API Documentation

Welcome to the official Nexus API documentation.

## 🌐 Live Site

**https://bhedanikhilkumar-code.github.io/docs/**

## Quick Start

```javascript
import { NexusClient } from '@nexusapi/sdk';

const nexus = new NexusClient({
  apiKey: process.env.NEXUS_API_KEY
});

const user = await nexus.users.me();
```

## API Base URL

```
https://api.nexusapi.dev/v1
```

## Authentication

All API requests require a Bearer token:

```
Authorization: Bearer YOUR_API_KEY
```

## SDKs

- **TypeScript/JavaScript**: `npm install @nexusapi/sdk`
- **Python**: `pip install nexusapi`
- **Go**: `go get github.com/nexusapi/nexus-go`

## Resources

- [API Reference](https://bhedanikhilkumar-code.github.io/docs/)
- [GitHub Repository](https://github.com/bhedanikhilkumar-code/docs)
- [Dashboard](https://dashboard.nexusapi.dev)

## Contributing

Contributions welcome! Please open an issue or pull request.

## License

MIT © 2024 bhedanikhilkumar-code
