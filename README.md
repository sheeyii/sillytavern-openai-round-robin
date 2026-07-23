# SillyTavern OpenAI Round-Robin Proxy

A proxy server that implements round-robin load balancing for OpenAI API requests in SillyTavern.

## Features

- Round-robin load balancing across multiple API keys
- Configuration management
- Test suite included
- Standalone executable

## Installation

```bash
npm install
```

## Configuration

Copy `config.example.json` to `config.json` and update with your API keys:

```json
{
  "port": 3000,
  "host": "localhost",
  "apiKeys": ["key1", "key2", "key3"],
  "proxySettings": {
    "timeout": 30000,
    "retries": 3
  }
}
```

## Usage

### As a module
```javascript
const proxyServer = require('./index');
```

### Standalone
```bash
node standalone.js
```

## Testing

```bash
npm test
```

## License

MIT