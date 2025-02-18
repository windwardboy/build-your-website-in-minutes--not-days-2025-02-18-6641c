# Landing Page Maintenance Guide

This guide will help you customize and maintain your AI Website Builder landing page. Whether you're new to web development or just getting started, follow these instructions to make updates while maintaining the page's professional appearance.

## Table of Contents
1. [Updating Text and Styling](#updating-text-and-styling)
2. [Managing Links](#managing-links)
3. [Adding Privacy and Terms Pages](#adding-privacy-and-terms-pages)
4. [Troubleshooting](#troubleshooting)

## Updating Text and Styling

### Header Section
The header contains your brand name and navigation menu. To update:

1. Change the brand name:
```html
<!-- Find this line in the header section -->
<a href="/" class="text-2xl font-bold text-white">WebComedia</a>
```
Simply replace "WebComedia" with your brand name.

### Hero Section
The hero section is your main banner area. To modify:

1. Update the main heading:
```html
<h1 class="text-4xl md:text-6xl font-bold mb-6 leading-tight">
    Build Your Website in Minutes, <br class="hidden md:block">Not Days
</h1>
```
Replace the text while keeping the `<br>` tag for proper mobile responsiveness.

2. Update the subheading:
```html
<p class="text-xl md:text-2xl text-gray-300 mb-12 max-w-3xl mx-auto">
    Best AI Website Builder, No Code Required
</p>
```

### Understanding Tailwind Classes
Common classes used in this template:

- Text sizes: `text-xl`, `text-2xl`, `text-4xl`
- Colors: `text-gray-300`, `bg-gray-900`
- Spacing: `mb-6` (margin bottom), `px-6` (padding left/right)
- Responsive design: `md:text-6xl` (applies at medium screens and up)

To modify styling:
1. Find the element you want to change
2. Locate its class attribute
3. Modify existing classes or add new ones
4. Test on both mobile and desktop views

## Managing Links

### Navigation Menu Links
Current navigation links are found in the header:

```html
<div class="hidden md:flex space-x-8">
    <a href="#features" class="text-gray-300 hover:text-white transition-colors duration-300">Features</a>
    <a href="#benefits" class="text-gray-300 hover:text-white transition-colors duration-300">Benefits</a>
    <a href="#video" class="text-gray-300 hover:text-white transition-colors duration-300">Demo</a>
    <a href="#faq" class="text-gray-300 hover:text-white transition-colors duration-300">FAQ</a>
</div>
```

To update:
1. Locate the `href` attribute
2. Replace with your new link
   - For internal sections, use `#section-id`
   - For external links, use full URLs (e.g., `https://example.com`)

### Call-to-Action Buttons
Update the "Get Started" buttons:

```html
<a href="https://webcomedia.net" class="px-6 py-2 bg-gradient-to-r from-purple-600 to-blue-600 text-white font-semibold rounded-lg hover:scale-105 transition-transform duration-300">
    Get Started
</a>
```

Replace `https://webcomedia.net` with your actual signup or product page URL.

## Adding Privacy and Terms Pages

### Footer Link Updates
Locate the footer links section:

```html
<div>
    <h4 class="text-xl font-bold mb-4">Links</h4>
    <ul class="space-y-2 text-gray-400">
        <li><a href="#" class="hover:text-white transition-colors duration-300">Privacy Policy</a></li>
        <li><a href="#" class="hover:text-white transition-colors duration-300">Terms of Service</a></li>
    </ul>
</div>
```

To add proper links:
1. Create your privacy.html and terms.html files
2. Update the href attributes:
```html
<li><a href="privacy.html" class="hover:text-white transition-colors duration-300">Privacy Policy</a></li>
<li><a href="terms.html" class="hover:text-white transition-colors duration-300">Terms of Service</a></li>
```

## Troubleshooting

Common issues and solutions:

1. **Broken Internal Links**
   - Ensure section IDs match href attributes
   - Check for typos in IDs
   - IDs are case-sensitive

2. **Responsive Design Issues**
   - Test on multiple screen sizes
   - Don't remove `md:` prefixed classes
   - Maintain the existing responsive structure

3. **Style Inconsistencies**
   - Keep gradient colors consistent (`from-purple-600 to-blue-600`)
   - Maintain padding and margin patterns
   - Use existing color schemes (`text-gray-300`, `bg-gray-900`)

For additional help:
- Reference [Tailwind CSS documentation](https://tailwindcss.com/docs)
- Use browser developer tools to inspect elements
- Test all changes across different devices and browsers

Remember to always backup your code before making significant changes!