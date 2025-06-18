# Landing Page Maintenance Guide

This guide will help you maintain and customize your business landing page. Follow these instructions carefully to make updates while preserving the design and functionality.

## Table of Contents
- [Updating Text and Styling](#updating-text-and-styling)
- [Managing Links](#managing-links)
- [Adding Privacy and Terms Pages](#adding-privacy-and-terms-pages)
- [Troubleshooting](#troubleshooting)

## Updating Text and Styling

### Header Section
The header contains your company name and navigation menu. To update:

1. **Company Name**: Find this line in the header:
```html
<div class="text-2xl font-bold text-gray-800">Lorem ipsum</div>
```
Replace "Lorem ipsum" with your company name.

2. **Navigation Menu Items**: Locate these lines in both desktop and mobile menus:
```html
<a href="#" class="text-gray-600 hover:text-gray-900 transition-colors duration-300">Home</a>
<a href="#" class="text-gray-600 hover:text-gray-900 transition-colors duration-300">About</a>
```
Update the text between `<a>` tags with your desired menu items.

### Hero Section
The main banner section contains your primary headline and call-to-action:

1. **Main Headline**: Find:
```html
<h1 class="text-4xl md:text-5xl lg:text-6xl font-bold leading-tight tracking-tight text-gray-900 mb-8">
    Transform Your Business with Modern Solutions
</h1>
```
Replace the text while keeping the surrounding tags intact.

2. **Subheading**: Update this paragraph:
```html
<p class="text-xl text-gray-600 mb-12 leading-relaxed">
    Elevate your brand with our professional services...
</p>
```

### Tailwind CSS Classes Explained
- `text-4xl`: Text size (increases with `md:text-5xl` on medium screens)
- `font-bold`: Text weight
- `text-gray-600`: Text color (600 is darker than 400)
- `mb-8`: Margin bottom spacing (1=0.25rem, 8=2rem)
- `hover:text-gray-900`: Color change on hover

## Managing Links

### Navigation Menu Links
1. Locate all `href="#"` attributes in the navigation:
```html
<a href="#" class="text-gray-600 hover:text-gray-900">Home</a>
```

2. Replace `#` with proper URLs:
- For internal pages: `href="about.html"`
- For external links: `href="https://example.com"`

### Footer Links
1. Find the Quick Links section:
```html
<ul class="space-y-2">
    <li><a href="#" class="text-gray-400 hover:text-white">About</a></li>
    <li><a href="#" class="text-gray-400 hover:text-white">Services</a></li>
</ul>
```

2. Update each `href="#"` with correct paths:
```html
<li><a href="about.html" class="text-gray-400 hover:text-white">About</a></li>
```

## Adding Privacy and Terms Pages

### Linking Privacy Policy
1. Locate this section in the footer:
```html
<li><a href="#" class="text-gray-400 hover:text-white">Privacy Policy</a></li>
```

2. Update the link:
```html
<li><a href="privacy.html" class="text-gray-400 hover:text-white">Privacy Policy</a></li>
```

### Linking Terms of Service
1. Find this line:
```html
<li><a href="#" class="text-gray-400 hover:text-white">Terms of Service</a></li>
```

2. Update to:
```html
<li><a href="terms.html" class="text-gray-400 hover:text-white">Terms of Service</a></li>
```

### Creating Consistent Styling
- Copy the existing link classes: `class="text-gray-400 hover:text-white transition-colors duration-300"`
- Use these classes for any new links you add to maintain visual consistency

## Troubleshooting

### Common Issues and Solutions

1. **Broken Layout After Text Changes**
- Ensure you haven't removed any closing tags
- Check that all classes remain intact
- Verify proper spacing in the markup

2. **Links Not Working**
- Confirm file names match exactly (case-sensitive)
- Verify files are in the correct directory
- Test paths using your local server

3. **Responsive Design Issues**
- Keep the responsive classes (md:, lg:) when updating
- Test on different screen sizes after changes
- Don't remove the viewport meta tag

### Need Help?
- Double-check your changes against the original code
- Use browser developer tools to inspect elements
- Maintain proper HTML structure and indentation
- Test all changes in multiple browsers

Remember to back up your files before making any changes, and test thoroughly after updates.