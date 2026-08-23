# Contributing

Awesome Userscripts is a curated list, so not every submission will be accepted. Entries should be useful, maintained, safe to install, and meaningfully different from scripts already listed.

## Before submitting

- Search the README, open issues, and open pull requests for duplicates.
- Confirm the userscript still works with a current browser and userscript manager.
- Use a stable, direct installation URL. Do not link to shortened or temporary URLs.
- Check that documentation and bug-report links are public and current.
- Submit one userscript per pull request. Category-wide improvements may be grouped when they form one focused change.

## Entry requirements

Each submission should include:

- Script name and a short, factual description ending with a period.
- Project, documentation, or catalogue page describing the script.
- Direct userscript installation link.
- Public bug tracker or support page when available.
- Screenshot or demo image when it helps explain visible behavior.
- Browser and userscript-manager combinations used for testing.

Descriptions should explain what the script does without promotional language, download counts, or unsupported claims. New entries must be placed alphabetically within the best matching category.

## Entry format

Match surrounding README markup. Use these link labels consistently:

- 💾 `Install` for a direct userscript installation link.
- 📖 `Readme` for documentation.
- 📢 `Discuss` for a discussion or community page.
- 🐛 `Report bug` for an issue tracker.

Omit unavailable optional links instead of changing a label's meaning.

```html
<details> <!-- Script Name -->
    <summary><a href="PROJECT_URL">Script Name</a> - Short, factual description.</summary><br>
    <blockquote>
        <a href="PROJECT_URL">
            <img width=511 src="SCREENSHOT_URL"></a>
    </blockquote>
    <blockquote>
        💾 <a href="INSTALL_URL">
            Install</a> /
        📖 <a href="README_URL">
            Readme</a> /
        📢 <a href="DISCUSSION_URL">
            Discuss</a> /
        🐛 <a href="ISSUES_URL">
            Report bug</a>
    </blockquote>
</details>
```

## Validate changes

Use Node.js 24, matching CI:

```sh
npm ci --ignore-scripts
npm run lint
```

Also open every added or changed link and verify that the install link serves the intended userscript.

## Pull request checklist

- Change is focused on one script or one related improvement.
- Entry is alphabetized and follows surrounding markup.
- Description is concise, factual, and ends with a period.
- Install, documentation, image, and support links work.
- Script was tested, with browser and userscript manager named in the pull request.
- `npm run lint` passes.
