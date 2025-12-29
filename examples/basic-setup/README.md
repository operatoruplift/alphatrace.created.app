# Basic Setup Example

This example demonstrates the basic setup and initialization of AlphaTrace.

## Overview

Learn how to:
- Install AlphaTrace
- Configure the client
- Track your first event
- View analytics data

## Getting Started

```bash
# Install dependencies
npm install

# Run the example
npm start
```

## Code Example

```javascript
import { AlphaTrace } from '@alphatrace/core';

// Initialize AlphaTrace
const tracer = new AlphaTrace({
  apiKey: 'your-api-key',
  environment: 'development'
});

// Track an event
tracer.track('user_action', {
  action: 'button_click',
  component: 'homepage'
});
```

## Next Steps

Once you've completed this basic setup, check out the [advanced usage](../advanced-usage/) examples for more sophisticated integrations.