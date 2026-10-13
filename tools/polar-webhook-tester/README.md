# Test a payment notification signature

**Positioning:** Paste a webhook secret, payload, `webhook-id`, and `webhook-timestamp`, and get back the expected `webhook-signature`, or check one you received. Debug the "bad signature" error without logging secrets anywhere. It runs 100% in the browser via WebCrypto, and nothing is sent to a server.
**Audience:** developers wiring up Polar (or any Standard Webhooks provider), which is exactly who buys Product 1.
**Price:** free. CTA: "Skip the wiring → Starter Kit".
**Polar notes:** none at runtime. Checked against docs.polar.sh (Oct 2026): it computes both schemes. Standard Webhooks applies to secrets created on/after 2026-09-08 UTC, and legacy Polar HMAC (UTF-8 bytes of the full `whsec_` string) to older ones. It reports which one matches.
**Deploy:** static, only with approval.

## Support
Questions, license, or refund requests: steeleblueai@gmail.com
