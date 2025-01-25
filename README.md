# NinjaSEO Landing Page - Maintenance Guide

This guide will help you maintain and customize the NinjaSEO landing page. Whether you're new to HTML and CSS or just getting started, follow these detailed instructions to make updates while preserving the design integrity.

## Table of Contents
1. [Updating Text and Styling](#updating-text-and-styling)
2. [Managing Links](#managing-links)
3. [Adding Privacy and Terms Pages](#adding-privacy-and-terms-pages)
4. [Troubleshooting](#troubleshooting)

## Updating Text and Styling

### Header Section
The header contains the logo and navigation menu. To modify:

```html
<!-- Logo Text -->
<div class="text-2xl font-bold text-gray-800">
    Ninja<span class="text-indigo-600">SEO</span>
</div>
```
- To change the logo text, simply replace "Ninja" and "SEO"
- The `text-indigo-600` class colors "SEO" in purple

### Hero Section
Located at the top of the page:

```html
<h1 class="text-5xl md:text-6xl font-bold text-gray-900 mb-8 leading-tight">
    10X Online Traffic With Online Ninja 🥷
</h1>
```
- Replace the heading text while keeping the emoji (🥷)
- `text-5xl` sets mobile size, `md:text-6xl` sets desktop size
- Don't remove `leading-tight` as it maintains proper line spacing

### Tailwind CSS Tips
Common classes used throughout:
- `text-gray-900`: Dark text
- `text-gray-600`: Secondary text
- `mb-8`: Margin bottom (spacing)
- `py-24`: Vertical padding
- `container mx-auto`: Centers content
- `px-6`: Horizontal padding

## Managing Links

### Navigation Menu Links
```html
<div class="hidden md:flex space-x-8">
    <a href="#features" class="text-gray-600 hover:text-indigo-600">Features</a>
    <a href="#benefits" class="text-gray-600 hover:text-indigo-600">Benefits</a>
    <a href="#faq" class="text-gray-600 hover:text-indigo-600">FAQ</a>
    <a href="#contact" class="text-gray-600 hover:text-indigo-600">Contact</a>
</div>
```
To update:
1. Locate the `href` attribute
2. Replace `#section-name` with your desired link
3. For internal links (same page), use `#section-id`
4. For external links, use full URL (e.g., `https://example.com`)

### Call-to-Action Links
Current CTA buttons point to `https://ninja200.online`. To change:
```html
<a href="https://ninja200.online" class="inline-block bg-indigo-600...">
    Start Your SEO Journey
</a>
```
1. Replace `https://ninja200.online` with your destination URL
2. Update button text between `<a>` tags
3. Maintain all classes to preserve styling

## Adding Privacy and Terms Pages

### Footer Links Setup
Current placeholder links in footer:
```html
<ul class="space-y-2">
    <li><a href="#" class="hover:text-white transition-colors duration-300">Privacy Policy</a></li>
    <li><a href="#" class="hover:text-white transition-colors duration-300">Terms of Service</a></li>
</ul>
```

To link proper pages:
1. Create `privacy.html` and `terms.html` in your root directory
2. Update the href attributes:
```html
<li><a href="privacy.html" class="hover:text-white transition-colors duration-300">Privacy Policy</a></li>
<li><a href="terms.html" class="hover:text-white transition-colors duration-300">Terms of Service</a></li>
```

## Troubleshooting

### Common Issues

1. **Broken Layout**
- Check that you haven't removed any essential Tailwind classes
- Verify container divs are properly closed
- Ensure responsive classes (md:, lg:) remain intact

2. **Links Not Working**
- Confirm file paths are correct
- Check for typos in URLs
- Verify file names match exactly (case-sensitive)

3. **Styling Issues**
- Don't remove `transition-` classes - they ensure smooth animations
- Keep `hover:` classes for interactive elements
- Maintain responsive classes starting with `md:` for proper mobile display

### Need Help?
- Double-check the HTML structure
- Compare against the original code
- Use browser developer tools (F12) to inspect elements
- Keep backups before making major changes

Remember: Always test your changes across different screen sizes using browser developer tools to ensure responsive design remains intact.

[Back to Top](#table-of-contents)