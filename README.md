# AryanShekar.com — Render-ready static site

This package contains the existing AryanShekar.com homepage plus complete Money Quest Kids
Privacy Policy and Support pages, styled to match the homepage.

## File structure

```text
index.html
404.html
render.yaml
moneyquest/
  privacy/
    index.html
  support/
    index.html
```

## Public URLs after deployment

- Homepage: `https://aryanshekar.com/`
- Privacy Policy: `https://aryanshekar.com/moneyquest/privacy/`
- Support: `https://aryanshekar.com/moneyquest/support/`

## App Store Connect

Use:

```text
Privacy Policy URL:
https://aryanshekar.com/moneyquest/privacy/

Support URL:
https://aryanshekar.com/moneyquest/support/
```

## Deploy on Render — existing Static Site

1. Put all files and folders from this package in the root of the GitHub repository used by
   the existing AryanShekar.com Render Static Site.
2. Commit and push the changes.
3. In Render, open the existing Static Site.
4. Set the Publish Directory to `.` if it is not already set.
5. Leave the Build Command blank, or use `echo "No build required"`.
6. Deploy the latest commit.
7. Open both public URLs in a private browser window before entering them in App Store Connect.

The included `render.yaml` is optional for an existing Render service. It is mainly useful
when creating a new Render Blueprint from the repository.

## Important email check

Both pages use:

```text
support@aryanshekar.com
```

Create that mailbox or forwarding address before publishing. Otherwise, replace every
occurrence in both legal-page HTML files with a working public support email.

## Privacy accuracy check before publication

The current policy says that profile names, the parental PIN and progress are stored locally
and are not transmitted to EqualEd. It also says the app has no third-party advertising.

Before publishing, update the policy if the app uses any service that sends information
off the device, including Firebase Analytics, Crashlytics, cloud sync, remote user accounts,
push-notification identifiers, advertising SDKs or other analytics/diagnostic services.
