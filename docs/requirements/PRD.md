# PRD: URL Shortener

## 1. Executive Summary
A minimal URL shortener service: users POST a long URL and get back a short code; GET /:code redirects to the original.

## 6. Scope & Features
- Create short link (POST /shorten)
- Redirect (GET /:code)
- Basic hit counter

## 7. Functional Requirements
- Short codes are unique, 6 chars.
- Redirect returns 301.
- Unknown code returns 404.

## 8. Non-Functional
- p95 < 100ms; 1k RPS.
