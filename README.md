# Sample Playwright Setup

This repository demonstrates a simple setup for running Playwright tests with BrowserStack integration.

## Getting Started

1. **Install dependencies**
   ```sh
   npm install
   ```

2. **Install Playwright browsers**
   ```sh
   npx playwright install
   ```

3. **Run tests on BrowserStack**
   ```sh
   npx browserstack-node-sdk playwright test --config playwright.config.ts
   ```

## Authentication Setup

- The repo includes authentication tests.
- During setup (as defined in `browserstack.yml`), a `.auth` folder is created containing credentials.
- These credentials are used by other tests in the build.

## Folder Structure

```
.
├── .auth/           # Stores authentication credentials
├── tests/           # Playwright test files
├── playwright.config.ts
├── browserstack.yml
└── README.md
```

## Notes

- Ensure you have access to BrowserStack and have configured your credentials in `browserstack.yml`.
- The `.auth` folder is auto-generated during setup and should not be manually edited.

