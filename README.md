# Vivario Public Pages

Static bilingual (English / Brazilian Portuguese) public-information pages for Vivario.

## Structure

- `index.html` — public information landing page
- `privacy/index.html` — Privacy Policy
- `terms/index.html` — Terms of Service
- `support/index.html` — Support
- `delete-account/index.html` — Account Deletion
- `assets/style.css` — shared visual styles

The pages use the visual direction from the supplied WildDex brand/UI guide:
- Forest green: `#0F3D2E`
- Leaf green: `#4CAF50`
- Warm cream: `#E8E1D6`
- Charcoal: `#1F1F1F`
- Gray: `#6B6B6B`
- Poppins or a similar sans-serif font

## IMPORTANT: review before publication

These pages are deliberately marked as a working draft. Do not submit them to Google Play or the App Store until the following are resolved:

1. Replace every `[INSERT ...]` / `[INFORMAR ...]` legal-operator placeholder with the actual full legal name and official address.
2. Confirm which legal person/entity is the data controller and service operator. The contact email alone does not establish this.
3. Verify the actual production data flows and providers (Firebase Authentication, Google Cloud services, Gemini, Firebase Cloud Messaging, taxonomy source and any analytics/crash tools).
4. Define exact retention periods or criteria for account data, photos/media, observations, logs, backups and provider-side AI requests.
5. Confirm the age rating/minimum age and any parental-consent process.
6. Confirm whether location is requested, collected, stored or attached to observations in the released app.
7. Confirm the account-deletion flow end-to-end, including deletion of profile, observations and media, third-party data where applicable, backup lifecycle and legally retained records.
8. Implement and test the in-app account deletion path where required by the app stores. This static email link is not a substitute for a working product flow if the store requires one.
9. Confirm that the public pages and support mailbox are monitored.
10. Have the final Privacy Policy and Terms reviewed by a qualified lawyer familiar with Brazilian LGPD and the other launch markets.

## Important engineering note

The source project README available when these drafts were prepared described AI identification as a development integration, disabled in staging/production pending launch gates. It also described Firebase Authentication, a FastAPI backend, PostgreSQL and Google Cloud infrastructure. Re-check all of this against the deployed production configuration before publishing.

The drafts avoid promising specific provider retention periods, guaranteed support response times, or immediate deletion from backups because those details were not established in the supplied project documentation.

## Contact

`nautilus@nautilustl.com`
