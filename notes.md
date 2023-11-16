#### To install Playwright
npm init playwright@latest

#### Run tests
npx playwright test

#### Show test report
npx playwright show-report

#### Execute on specific browser
npx playwright test --project=firefox

#### Run test in headed mode (default is headless)
npx playwright test --project=firefox --headed

#### Execute a specific test case
npx playwright test spec_file_name --project=chrome

#### Execute a specific test by specifying its name
npx playwright test -g "test name" --project=chromium

#### Selectively running or excluding tests (test.skip or test.only)
test.skip('test desc')
test.only('test desc')

#### Running tests via playwright UI
npx playwright test --ui

Using the UI runner we have features like watch a test case, that runs if any change is made to the test case
Also, the screenshot and steps where the test case exactly failed is also available for easier debugging

#### Trace mode
npx playwright test --project=chromium --trace on

#### Debug mode
npx playwright test --project=chromium --debug