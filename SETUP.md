# Set up ShelterPact public support on GitHub

## 1. Create an independent public repository

1. Sign in at https://github.com/new under the account or organization that owns ShelterPact.
2. Name it `ShelterPact-Support`.
3. Select **Public**. This must be a **new empty repository** — never change the visibility of the private application repository.
4. Initialize with a README if uploading files individually in the browser, or leave it empty for the command-line upload below.
5. Never fork, mirror, or copy application source files into it.

## 2. Upload this package

For an empty repository, unzip this archive on your computer and run from inside the extracted `ShelterPact-Support` directory:

```bash
git init
git branch -M main
git add .
git commit -m "Initialize public ShelterPact support community"
git remote add origin https://github.com/YOUR_USERNAME/ShelterPact-Support.git
git push -u origin main
```

Replace YOUR_USERNAME with the actual repository owner. Sign into GitHub when prompted; do not put a password or token in a command.

If you initialized the repository with a README on GitHub, upload the files through **Add file > Upload files** instead, replacing README.md deliberately.

## 3. Enable Discussions

In your new `ShelterPact-Support` repository: **Settings > General > Features > Discussions**. Check **Discussions**. Open the new Discussions tab and use **Categories > Edit** to create/rename categories.

Suggested categories and formats:

| Category | Format |
| --- | --- |
| Announcements | Announcement (maintainers only) |
| Help & Questions | Question / Answer |
| Animal Operations | Question / Answer |
| Municipal & Compliance | Question / Answer |
| Feature Requests | Open-ended discussion |
| Bug Reports | Question / Answer |
| Tips & Best Practices | Open-ended discussion |
| General Discussion | Open-ended discussion |

You can remove default categories you do not want. GitHub might require creating categories before the discussion form templates appear or associate with them.

## 4. Publish a welcome discussion

In **Announcements**, create and pin a discussion with this text:

**Title:** Welcome to the ShelterPact Community!

Welcome! This is a place for animal shelter, rescue, and municipal animal services professionals to ask questions, share ideas, and help improve ShelterPact. Please choose the appropriate category, search for similar topics, and keep discussions courteous and constructive. Never share citizen or animal-owner records, confidential case information, credentials, or unredacted screenshots. For private assistance, contact support@shelterpact.com. Explore ShelterPact at https://shelterpact.com.

## 5. Link from your website

Use the public URL `https://github.com/YOUR_USERNAME/ShelterPact-Support/discussions` behind a **Community Forum** or **Ask the Community** link. Consider adding it under Support and in the site footer. No changes to your VPS are required for GitHub-hosted Discussions.

## 6. Safety check

- Confirm the original application repository still says **Private**.
- Confirm the public repository contains *only* these community files (not app code, `.env` files, secrets, database exports, or internal documents).
- Open the Discussions URL in a signed-out/private browser session to verify public visibility.
- Verify your account has notifications enabled for new discussion activity.
