# web-test-runner-manual-html
Basic example using @web/test-runner to demonstrate issue with manual invocation
of HTML test file.

This works: `yarn web-test-runner --puppeteer`

This doesn't when choosing the HTML test: `yarn web-test-runner --manual`

The problem appears to be that manual invocation is attempting to load the
HTML file as a Javascript module.
