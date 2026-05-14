# AI Agent Instructions

<!-- This file provides instructions for AI agents working with this documentation repository. -->

## Project Overview

This is the **Nexus API** documentation site, built with [Mintlify](https://mintlify.com). It contains comprehensive API documentation for developers integrating with Nexus.

## Repository Structure

```
docs/
├── index.mdx              # Home page
├── quickstart.mdx        # Quick start guide
├── development.mdx       # Development environment setup
├── essentials/           # Core concepts and guides
│   ├── auth.mdx          # Authentication
│   ├── api-keys.mdx      # API key management
│   ├── models.mdx        # Data models
│   ├── endpoints.mdx     # API endpoints
│   ├── rate-limits.mdx   # Rate limiting
│   ├── pagination.mdx    # Pagination
│   ├── errors.mdx        # Error handling
│   └── webhooks.mdx      # Webhooks
├── api-reference/        # Detailed API reference
│   ├── users/            # User API endpoints
│   ├── projects/         # Project API endpoints
│   └── analytics/        # Analytics API endpoints
├── snippets/             # SDK examples
│   ├── python.mdx        # Python SDK
│   ├── javascript.mdx    # JavaScript SDK
│   └── curl.mdx          # cURL examples
├── agent-ready/          # AI agent integration features
│   ├── prompt.mdx        # Prompt component
│   ├── visibility.mdx   # Content visibility control
│   └── contextual.mdx    # Contextual menu
└── docs.json             # Mintlify configuration
```

## For AI Agents

### Understanding the API

- **Base URL**: `https://api.nexus.dev/v1`
- **Sandbox URL**: `https://api-sandbox.nexus.dev/v1`
- **Authentication**: Bearer token (API key starting with `nx_live_` or `nx_test_`)

### Key Data Types

| Type | ID Format | Description |
|------|-----------|-------------|
| User | `usr_xxxx` | User account |
| Project | `prj_xxxx` | Project container |
| Event | `evt_xxxx` | Analytics event |
| API Key | `nx_xxxx` | API authentication |

### Common Operations

1. **List resources**: `GET /v1/{resource}`
2. **Get single**: `GET /v1/{resource}/{id}`
3. **Create**: `POST /v1/{resource}`
4. **Update**: `PATCH /v1/{resource}/{id}`
5. **Delete**: `DELETE /v1/{resource}/{id}`

### Pagination

All list endpoints support cursor-based pagination:
- `limit`: Number of items (default: 20, max: 500)
- `cursor`: Pagination cursor for next page

### Error Handling

Standard HTTP status codes with JSON error responses:
- `400`: Validation error
- `401`: Authentication failed
- `403`: Insufficient permissions
- `404`: Resource not found
- `429`: Rate limit exceeded
- `500`: Server error

## Development Commands

```bash
# Preview locally
mint dev

# Check for broken links
mint broken-links

# Update Mintlify CLI
mint update
```

## Adding New Documentation

1. Create the `.mdx` file in the appropriate folder
2. Add frontmatter with `title` and `description`
3. Add the page to `docs.json` navigation
4. Test with `mint dev`

## Content Guidelines

- Use active voice and second person ("you")
- Keep sentences concise
- Use code formatting for technical terms
- Include code examples for all endpoints
- Add error handling examples
- Reference related documentation pages

## Style Preferences

- Sentence case for headings
- Bold for UI elements: Click **Settings**
- Code formatting for paths, commands, and technical terms
- Tables for structured data
- Tabs for multi-language examples