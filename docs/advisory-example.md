# Advisory Example — Workshop Demo

This document is the working example for our open-source supply-chain security workshop.

## Advisory Details

- **GHSA ID:** GHSA-673q-mjm6-r5xr
- **Title:** Next.js: Unauthenticated Remote Code Execution in `use cache` functions returning typed arrays
- **Severity:** critical
- **Affected Package:** `next` (npm)
- **Vulnerable Version Range:** >= 16.0.0, <= 16.4.0
- **First Patched Version:** 16.4.1
- **CWE:** CWE-502 (Deserialization of Untrusted Data)

## Summary

A vulnerability in applications using the App router with Cache Component can lead to remote code execution. The application needs to have a `use cache` function that returns multiple typed arrays. There is no known workaround for affected applications with such `use cache` functions — you should upgrade immediately even if your application does not have similar functions.

## Reference

- Advisory: https://github.com/advisories/GHSA-673q-mjm6-r5xr
- Upstream advisory: https://github.com/vercel/next.js/security/advisories/GHSA-673q-mjm6-r5xr
- Patched release: https://github.com/vercel/next.js/releases/tag/v16.4.1

---

*This is the example advisory we build the workshop demo around.*
