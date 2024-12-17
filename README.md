# Sparkle ID Common Package

[![NPM Version](https://img.shields.io/npm/v/@sparkleid/common)](https://www.npmjs.com/package/@sparkleid/common)
[![GitHub Repository](https://img.shields.io/github/stars/Sparkle-ID/common?style=social)](https://github.com/Sparkle-ID/common)

## Overview
The `@sparkleid/common` package provides shared utilities, constants, and type definitions used across Sparkle ID services and applications. It streamlines development by centralizing common logic into a single, reusable module.

## Installation

```bash
npm install @sparkleid/common
```

## Features
- **Middleware:** Pre-built middleware functions for consistent request handling.
- **Error Handling:** Standardized error classes for streamlined API error management.
- **Type Definitions:** Centralized TypeScript interfaces and types.
- **Constants:** Global constants used across the Sparkle ID ecosystem.
- **Utility Functions:** Common helper functions for data processing and validation.

## Usage

### Middleware
Use the built-in middleware functions to manage request validation, authentication, and response formatting.

```typescript
import { middleware } from '@sparkleid/common';

// Example: Request validation middleware
app.use(middleware.validateRequest);

// Example: Authentication middleware
app.use(middleware.authenticate);
```

### Error Handling
The package includes standard error classes for clean and consistent error management.

```typescript
import { errors } from '@sparkleid/common';

// Throwing an authentication error
throw new errors.AuthenticationError('Invalid token');

// Throwing a validation error
throw new errors.ValidationError('Missing required field');
```

## Modules

### Constants
Shared application constants.
```typescript
import { constants } from '@sparkleid/common';
console.log(constants.APP_VERSION);
```

### Types
TypeScript interfaces and type definitions.
```typescript
import { types } from '@sparkleid/common';
const user: types.User = {
  id: '1',
  name: 'Jane Doe'
};
```

### Utils
Helper functions for data processing and validation.
```typescript
import { utils } from '@sparkleid/common';
const isValid = utils.validateEmail('test@example.com');
```

## Contributing
We welcome contributions! Please check the [GitHub repository](https://github.com/Sparkle-ID/common) for guidelines on how to get involved.

## License
This project is licensed under the MIT License. See the [LICENSE](https://github.com/Sparkle-ID/common/blob/main/LICENSE) file for details.

---
For more information, check out the [NPM Package Page](https://www.npmjs.com/package/@sparkleid/common) and the [GitHub Repository](https://github.com/Sparkle-ID/common).

