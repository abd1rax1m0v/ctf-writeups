# XSS on daryo.uz search endpoint

## Target:
`https://daryo.uz/search?q=test`

## Vulnerability:
Reflected Cross Site Scripting (XSS)

## Tools Used:
- XSStrike
- Google Chrome DevTools
- View-source

## Steps to Reproduce:
1. Visit the URL and inject:
2. Script executes, confirming XSS.

## Impact:
Attacker can run arbitrary JS in user’s browser.

## Recommendation:
- Escape user input
- Validate query params
- Implement CSP headers
