# Al Mutlaq Furniture Landing Page - Maintenance Guide

This guide provides detailed instructions for maintaining and customizing the Al Mutlaq Furniture landing page. Whether you're new to web development or need a quick reference, follow these step-by-step instructions.

## 1. Updating Text and Tailwind CSS Classes

### Text Content Updates

#### Hero Section
```html
<!-- Located in the main hero section -->
<h1 class="text-4xl md:text-5xl lg:text-7xl font-bold leading-tight mb-8">
    Experience Excellence in Furniture Since 1954
</h1>
```
To modify:
1. Locate the `<h1>` tag in the hero section
2. Replace the text between the opening and closing tags
3. Maintain the existing classes to preserve styling

#### Features Section
Each feature card follows this structure:
```html
<div class="bg-gray-800/50 rounded-2xl p-8">
    <h3 class="text-xl font-semibold mb-4">Offices</h3>
    <p class="text-gray-400">Professional workspace solutions...</p>
</div>
```
To update:
1. Find the feature cards in the `#features` section
2. Modify the `<h3>` title and `<p>` description
3. Keep the existing classes for consistent styling

### Tailwind CSS Classes Explained

#### Responsive Design Classes
- `md:` - Applies styles on medium screens (768px and up)
- `lg:` - Applies styles on large screens (1024px and up)

Example:
```html
<h1 class="text-4xl md:text-5xl lg:text-7xl">
<!-- text-4xl (mobile) → text-5xl (tablet) → text-7xl (desktop) -->
```

#### Common Class Combinations
```html
<!-- Card styling -->
<div class="bg-gray-800/50 rounded-2xl p-8 hover:bg-gray-800 transition duration-300">
```
- `bg-gray-800/50`: Semi-transparent background
- `rounded-2xl`: Rounded corners
- `p-8`: Padding on all sides
- `hover:bg-gray-800`: Background color on hover
- `transition duration-300`: Smooth transition effect

## 2. Fixing Broken Links

### Navigation Menu Links
Current structure:
```html
<div class="hidden md:flex space-x-8">
    <a href="#features">Solutions</a>
    <a href="#benefits">Services</a>
    <a href="#faq">FAQ</a>
    <a href="#contact">Contact</a>
</div>
```

To update internal links:
1. Locate the `<a>` tags in the navigation
2. Modify the `href` attribute to point to the correct section ID
3. Ensure section IDs match exactly (case-sensitive)

### External Links
For the main CTA button:
```html
<a href="https://almutlaqfurniture.com" class="inline-block bg-gradient-to-r...">
    Explore Our Collection
</a>
```
To update:
1. Replace the `href` value with your desired URL
2. Ensure URLs include `https://` or `http://`
3. Test links before deploying

## 3. Linking Privacy and Terms Pages

### Footer Links Section
Current structure:
```html
<div class="flex space-x-6 mt-4 md:mt-0">
    <a href="#" class="text-gray-400 hover:text-white transition-colors duration-300">Privacy Policy</a>
    <a href="#" class="text-gray-400 hover:text-white transition-colors duration-300">Terms of Service</a>
</div>
```

To add privacy and terms pages:
1. Create `privacy.html` and `terms.html` in your root directory
2. Update the href attributes:
```html
<a href="privacy.html" class="text-gray-400 hover:text-white transition-colors duration-300">Privacy Policy</a>
<a href="terms.html" class="text-gray-400 hover:text-white transition-colors duration-300">Terms of Service</a>
```

## Troubleshooting Tips

### Common Issues and Solutions

1. **Broken Internal Links**
   - Ensure section IDs match exactly
   - Check for spaces or special characters in IDs
   - Example: `href="#features"` must match `id="features"`

2. **Responsive Design Issues**
   - Test on multiple screen sizes
   - Use browser dev tools to check breakpoints
   - Verify media query classes (md:, lg:) are correct

3. **Styling Inconsistencies**
   - Copy existing class combinations for new elements
   - Maintain the gradient theme: `from-purple-500 to-pink-500`
   - Keep consistent spacing using provided utility classes

### Best Practices

1. Always backup before making changes
2. Test all links after updates
3. Maintain consistent styling across new elements
4. Use browser dev tools to preview changes
5. Validate external URLs before linking

## Need Help?

If you encounter issues:
1. Check the HTML structure matches exactly
2. Verify all classes are spelled correctly
3. Test on multiple browsers
4. Ensure all files are in the correct directory
5. Double-check all closing tags

Remember to maintain the existing color scheme and responsive design patterns when making updates to preserve the site's professional appearance.