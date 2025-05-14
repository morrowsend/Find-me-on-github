# Find-me-on-github
Bookmarklet that takes you to github.com repo page form any github.io page

# GitHub Pages → Repository Bookmarklet

This bookmarklet lets you quickly jump from a `github.io` project site to the corresponding GitHub repository.

## How it works

If you're on a page like:

https://username.github.io/repo-name/

css
Copy
Edit

Clicking the bookmarklet takes you to:

https://github.com/username/repo-name

less
Copy
Edit

## How to Install

1. Drag the link below to your bookmarks bar, or right-click and save as a bookmark:

**[Go to GitHub Repo](javascript:(function(){const host=location.hostname;const path=location.pathname.split('/').filter(Boolean);if(host.endsWith('github.io')&&path.length>0){const user=host.split('.')[0];const repo=path[0];window.location.href=`https://github.com/${user}/${repo}`;}else{alert('Not a github.io project page or missing repo name.');}})**
)

2. Visit a GitHub Pages project (e.g., `https://username.github.io/project`).
3. Click the bookmarklet.

## Limitations

- Works only for `username.github.io/repo` style URLs.
- Doesn’t support custom domains (like `mycoolproject.com`).

## License

MIT
