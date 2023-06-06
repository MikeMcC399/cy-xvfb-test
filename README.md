# cy-xvfb-test
 Tests for xvfb running under Cypress

---

- Cypress issue https://github.com/cypress-io/cypress/issues/19868

## Current

Cypress starts `xvfb` when running Chrome headless.

## Desired

Cypress should not start `xvfb` when running Chrome headless. Refer to https://developer.chrome.com/blog/headless-chrome/#faq "Headless Chrome doesn't use a window so a display server like Xvfb is no longer needed. You can happily run your automated tests without it."

## Repro code

[chrome.yml](.github/workflows/chrome.yml)

---
