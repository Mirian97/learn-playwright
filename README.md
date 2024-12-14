<img src="./docs/playwright.jpg" alt="Playwright Logo" style="background-color: #FFF; padding: 10px; margin: 0 auto;" />

# Playwright Project

This repository contains automated tests written using [Playwright](https://playwright.dev/).
Playwright is considered one of the best solutions for end-to-end (E2E) testing due to the following key features:

- **Cross-Browser Testing**:
  Playwright supports all major browsers, including Chromium, Firefox, and WebKit. This ensures your application works seamlessly across different environments.

- **Automatic Waiting**:
  Playwright automatically waits for elements to be ready before performing actions, reducing the need for complex and flaky manual wait logic.

- **Multi-Language Support**:
  While built in Node.js, Playwright offers bindings for Python, Java, and C#, making it accessible to developers across different tech stacks.

- **Fast and Reliable**:
  Playwright runs tests quickly and efficiently, with parallel execution and reduced flakiness, even for dynamic web applications.

- **Headless and Headed Execution**:
  Tests can be run in headless mode for CI pipelines or headed mode for debugging and observation.

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/learn-playwright.git
   cd learn-playwright
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

## Running Tests

To run all tests, execute the following command:

```bash
npx playwright test
```

### Show Report Test

After run the tests, you can see the detailed report with:

```bash
npx playwright show-report
```

### Running Specific Tests

You can run a specific test file by specifying its path:

```bash
npx playwright test tests/example.spec.js
```

### Headless Mode

By default, Playwright runs tests in headless mode. To run tests with a visible browser:

```bash
npx playwright test --headed
```

### Running Tests to Specific Browser

If you would like to run in specific browser

```bash
npx playwright test --project chromium
```

### Debugging

To debug tests, use the following command:

```bash
npx playwright test --debug
```

## Folder Structure

- **tests/**: Contains test files written in JavaScript/TypeScript.
- **playwright.config.js**: Configuration file for Playwright.

## Documentation

- Official Playwright Documentation: [https://playwright.dev/docs/intro](https://playwright.dev/docs/intro)
