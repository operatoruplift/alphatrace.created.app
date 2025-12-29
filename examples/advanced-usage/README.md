# Advanced Usage Example

This example showcases advanced features of AlphaTrace including distributed tracing, custom metrics, and complex event tracking.

## Overview

Learn how to:
- Implement distributed tracing across services
- Create custom metrics and dashboards
- Set up advanced event tracking
- Configure performance monitoring
- Integrate with existing observability tools

## Prerequisites

Before running this example, make sure you've completed the [basic setup](../basic-setup/) example.

## Getting Started

```bash
# Install dependencies
npm install

# Configure environment
cp .env.example .env
# Edit .env with your configuration

# Run the example
npm start
```

## Features Demonstrated

### Distributed Tracing
```javascript
const trace = tracer.startTrace('user-checkout-flow');
trace.addSpan('validate-cart');
trace.addSpan('process-payment');
trace.addSpan('send-confirmation');
trace.end();
```

### Custom Metrics
```javascript
tracer.metric('checkout_duration', {
  value: 1234,
  unit: 'milliseconds',
  tags: { user_tier: 'premium' }
});
```

## More Information

For detailed API documentation, see the [API Reference](../../docs/api-reference.md).