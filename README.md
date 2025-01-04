# TechtoGreen Project README

Welcome to the TechtoGreen project! This README is designed to help everyone contribute effectively, even if you're new to web development. Please read it carefully before making any changes.

## Project Structure

Here's a clear breakdown of the folder and file structure:

```
TechtoGreen/
├── index.html              # Main HTML file (uses partials for modular structure)
├── css/                    # Stylesheets
│   ├── index.css          # Custom CSS for the project
│   └── stylesheet.css     # Additional styles
├── images/                 # Image assets
│   └── ttgLogo.png        # Website favicon/logo
├── js/                     # JavaScript files
│   ├── theme.js           # Custom JS for the project
│   └── switcher.min.js    # Style switcher script
├── partials/               # HTML components for modular structure
│   ├── header.html        # Navbar and header section
│   ├── about.html         # About section
│   ├── services.html      # Services section
│   ├── portfolio.html     # Portfolio section
│   ├── contact.html       # Contact section
│   ├── footer.html        # Footer section
│   ├── disclaimer.html    # Disclaimer modal content
│   └── terms-policy.html  # Terms and policy modal content
```

## Editing Guidelines

Follow these steps to safely edit and update the project:

### 1. Editing Partials (HTML Components)

All modular HTML sections (like Header, About, Services, etc.) are stored in the `partials/` directory.

To edit a specific section, open the corresponding file in the `partials/` folder. For example:

- Want to edit the About section? Open `partials/about.html`.
- Want to update the Footer? Open `partials/footer.html`.

### 2. Editing CSS

The main CSS files are stored in the `css/` directory.

- Use `css/index.css` for specific customizations related to this project.
- Avoid directly modifying `css/stylesheet.css` unless necessary. It's better to add your styles to `index.css`.

### 3. Editing JavaScript

The main JavaScript logic resides in `js/theme.js`. Add any project-specific functionality here.

- Avoid modifying `js/switcher.min.js` unless you're confident. It's for style switching.

### 4. Adding/Editing Images

All images, including logos and icons, are in the `images/` folder.

- To update the favicon/logo, replace `images/ttgLogo.png` with your new file (ensure the file name is the same).

### 5. Working with Vendor Files

You can't.

### 6. Loading Components Dynamically

The `index.html` file dynamically loads partials using the `loadComponent()` function in `theme.js`.

#### Function Example:

```javascript
loadComponent('header', 'partials/header.html');
loadComponent('about', 'partials/about.html');
```

If you add new partials, make sure to include them in this script within `index.html`.

### 7. Testing Changes

After making edits, test your changes by opening `index.html` in a browser.

- For dynamic partials, ensure your changes are loading properly.

## Troubleshooting

### Issue: Changes not visible.

- Ensure you saved the file.
- Clear your browser cache.
- Check the file path for typos.

### Issue: CSS/JS not working.

- Confirm the correct file is linked in `index.html`.
- Check the browser console for errors (Right-click > Inspect > Console).

## General Tips

- Always back up files before making major changes: `git add .; git commit -m "some changes"`.
- Keep changes modular by editing the relevant partials or files.
- Communicate with the team about what you're working on to avoid conflicts.

If you have any questions or need help, don't hesitate to ask. Happy coding!
