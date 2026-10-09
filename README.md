# One Message · Donate

The public payment-details page for **One Message**, the Ramadan Sehri app for students.

It shows the UPI ID and QR code. People pay from their own UPI app, then go back to the One Message app to submit the amount and a screenshot, which a super admin verifies. This page processes no payments.

The app opens this page in the phone's browser instead of showing payment details itself, because a fundraiser that is not an approved nonprofit may only collect funds outside the app (App Store Review Guideline 3.2.2(iv)).

## Hosting

Served by GitHub Pages from the `main` branch root. It is plain HTML with no build step:

- `index.html`: the donation page
- `privacy.html`: the app's privacy policy (linked from the app and both store listings)
- `delete-account.html`: how to delete an account without the app (Google Play requirement)
- `site.css`: styles for the two policy pages
- `qr.jpeg`: the UPI QR code
- `.nojekyll`: serve the files as they are

To change the UPI ID, edit it in `index.html` in three places: the visible ID, the `upi://` link and the copy script. Replace `qr.jpeg` to match.
