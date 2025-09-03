
npm install
npx playwright install

npx browserstack-node-sdk playwright test --config playwright.config.ts

The repo has some auth tests that are mentioned under setup flag in browserstack.yml which creates a .auth folder with all the credentials that can be used by other tests in the build.
