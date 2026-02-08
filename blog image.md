# Image Classes Guide for Blog Posts

## How to Use Image Classes in Your JSON

When adding images to your blog posts in the `posts.json` file, you can control their size, alignment, and style using CSS classes.

## SIZE Classes

### img-small
Small images (max 300px width, centered)
```html
<img src="screenshot.png" class="img-small" alt="Screenshot">
```

### img-medium
Medium images (max 600px width, centered)
```html
<img src="diagram.png" class="img-medium" alt="Diagram">
```

### img-large
Large images (max 100% width, full container)
```html
<img src="banner.jpg" class="img-large" alt="Banner">
```

### img-full
Full-width images (always 100% width)
```html
<img src="hero.jpg" class="img-full" alt="Hero">
```

## ALIGNMENT Classes

### img-left
Float image to the left, text wraps around
```html
<img src="profile.jpg" class="img-left" alt="Profile">
```

### img-right
Float image to the right, text wraps around
```html
<img src="logo.png" class="img-right" alt="Logo">
```

### img-center
Center the image (works with any size)
```html
<img src="chart.png" class="img-medium img-center" alt="Chart">
```

## STYLE Classes

### img-rounded
More rounded corners (12px radius)
```html
<img src="card.png" class="img-medium img-rounded" alt="Card">
```

### img-circle
Circular image (great for profile photos)
```html
<img src="avatar.jpg" class="img-small img-circle" alt="Avatar">
```

### img-shadow
Adds shadow effect
```html
<img src="screenshot.png" class="img-medium img-shadow" alt="Screenshot">
```

### img-border
Adds border with padding
```html
<img src="photo.jpg" class="img-medium img-border" alt="Photo">
```

## COMBINING Classes

You can combine multiple classes for custom effects:

```html
<!-- Small, centered, rounded image with shadow -->
<img src="icon.png" class="img-small img-center img-rounded img-shadow" alt="Icon">

<!-- Medium, left-aligned image with border -->
<img src="diagram.png" class="img-medium img-left img-border" alt="Diagram">

<!-- Full-width image with shadow -->
<img src="banner.jpg" class="img-full img-shadow" alt="Banner">

<!-- Circular profile picture, small and centered -->
<img src="profile.jpg" class="img-small img-circle img-center" alt="Profile">
```

## Example JSON Entry

```json
{
  "slug": "my-awesome-post",
  "title": "My Awesome Post",
  "excerpt": "This is an example post with images",
  "date": "2026-02-07",
  "category": "Tutorial",
  "tags": ["example", "images"],
  "image": "hero.jpg",
  "content": "<h2>Introduction</h2><p>Here's my post with various images:</p><img src='hero.jpg' class='img-full img-shadow' alt='Hero Image'><h2>Section 1</h2><p>Here's a small centered image:</p><img src='icon.png' class='img-small img-center img-rounded' alt='Icon'><h2>Section 2</h2><img src='diagram.png' class='img-left img-medium' alt='Diagram'><p>This text will wrap around the left-aligned image. Lorem ipsum dolor sit amet...</p>"
}
```

## Default Behavior (No Classes)

If you don't add any classes, images will:
- Be max 100% width (responsive)
- Have slight border radius (4px)
- Have 30px top and bottom margin
- Be left-aligned

## Tips

1. **For screenshots**: Use `img-medium img-shadow img-center`
2. **For profile photos**: Use `img-small img-circle img-center`
3. **For hero images**: Use `img-full img-shadow`
4. **For diagrams**: Use `img-medium img-center`
5. **For inline images**: Use `img-small img-left` or `img-small img-right`

## Mobile Responsive

On mobile (screens < 768px):
- Left and right floating images automatically become full-width
- All images stack vertically for better readability

## baisc html tags 
<h2></h2>
<p></p>
<h2></h2>
<pre><code class='language-javascript'></code></pre>
<blockquote></blockquote>