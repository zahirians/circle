# Circle - Zahirians Management System

This is the **deployment repository** for the Circle application.

🚀 **Live App:** https://zahirians.github.io/circle/app/

## About This Repository

This repository contains only the **built/compiled files** for GitHub Pages deployment. The source code is maintained in a separate private repository.

## Automatic Deployment

This repository is automatically updated via GitHub Actions when changes are pushed to the source repository.

**Source Repository:** Private repository containing the source code  
**Deployment:** Automatic via GitHub Actions workflow

## Manual Deployment

If you need to deploy manually:

1. Build the application in the source repository
2. Copy all files from the `build/` folder to the `app/` folder in this repository
3. Ensure `.nojekyll` file is present in the `app/` folder
4. Commit and push changes

## Repository Structure

```
circle/
└── app/              # Deployed application files
    ├── index.html
    ├── .nojekyll     # Required for GitHub Pages
    ├── static/       # CSS, JS, and media files
    └── ...
```

## Important Files

- **`.nojekyll`**: Prevents Jekyll processing (required for React apps on GitHub Pages)
- **`app/index.html`**: Main application entry point
- **`app/static/`**: All static assets (CSS, JavaScript, images)

## Troubleshooting

### 404 Errors

If you see 404 errors for static assets:
1. Verify `.nojekyll` exists in the `app/` folder
2. Check that all files from `build/static/` are in `app/static/`
3. Wait 1-2 minutes for GitHub Pages to rebuild
4. Clear browser cache

### Deployment Issues

- Check the source repository's Actions tab for deployment logs
- Verify GitHub Actions has write access to this repository
- Ensure the workflow is running successfully

---

Built with ❤️ for Zahirians Circle

