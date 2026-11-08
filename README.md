# Tiny Kitchen — privacy policy website

A static, English privacy-policy page for self-hosting. No build tools, JavaScript, external fonts, cookies, forms or analytics are included in this website. No Unity files are changed.

## Before hosting / submitting to Meta

This is a draft, not a completed privacy certification. In `index.html`:

1. Replace every `Muhammad Benny Fathurrahman` and `bennyfathurr@gmail.com`. Use the responsible person's legal name for the unincorporated Skyfog Labs team.
2. Complete the highlighted retention and deletion-practice fields based on what you actually implement. The current game has no implemented online deletion workflow; do not promise one until you have a working administrative process.
3. Review development logging, any added SDKs/providers, backups and actual storage practices. The policy intentionally acknowledges local development logs rather than claiming tracking data is never recorded.
4. Implement and verify the mixed-age API/feature handling in the game, then rewrite section 06 to describe the actual behavior. The current age-check functionality is not implemented and is not presented as completed here.
5. Confirm privacy contact availability and a response process. Update the draft date to the actual reviewed effective date.
6. Remove the yellow draft notice and the `<meta name="robots" content="noindex, nofollow">` line once ready. Remove all highlighted owner-review placeholders and their review labels. Search for `[` and `Owner review` to find the remaining fields.

## Preview locally

Open `index.html` in a browser, or run from this folder:

```sh
python3 -m http.server 8788
```

Then open `http://localhost:8788/`.

## Host

Upload **both** `index.html` and `styles.css` to the same public folder on your static host (for example `/privacy/`). No server code or environment variables are needed. Keep the CSS filename and link intact. The final page must be readable over HTTPS without login; submit that public page URL to Meta, not a local path or ZIP link. The local preview URL is not a public policy URL.

Check the hosted page on desktop and mobile and verify the contact/deletion instructions before submission. The anchors work without JavaScript; the page also has a print stylesheet.

Meta references:
- https://developers.meta.com/vr/policy/privacy-policy/
- https://developers.meta.com/vr/resources/vrc-quest-privacy-4/

The presence of this website does not establish that game behavior meets Meta's mixed-age or data-use requirements.
