# Spectravella

A beautiful, animated color gradient visualizer that creates smoky, flowing spectrum effects for your web projects.

![Spectravella](https://img.shields.io/badge/version-1.0.0-purple) ![License](https://img.shields.io/badge/license-MIT-green)

## ✨ Features

- **Animated Gradients** - Smooth, flowing color transitions with a smoky aesthetic
- **Customizable Colors** - 4 gradient colors + background color
- **Zero Dependencies** - Three.js is bundled, just drop in and go
- **Lightweight** - Single JS file, easy to integrate
- **Responsive** - Adapts to any container size

## 🚀 Quick Start

### 1. Include the Script

Add `spectravella.js` in the `<head>` of your HTML file:

```html
<head>
  <script src="spectravella.js"></script>
</head>
```

### 2. Add the Container

Create a container element with the class `sprectravella-container`:

```html
<div class="sprectravella-container"></div>
```

### 3. Style the Container

Set dimensions for your container:

```css
.sprectravella-container {
  width: 100%;
  height: 500px;
  overflow: hidden;
}
```

That's it! The visualizer will automatically initialize and start animating.

## 🎨 Customizing Colors

### Using Color Inputs

Add color input elements with specific IDs to let users customize the palette:

```html
<!-- Gradient Colors -->
<input type="color" id="spectravella-color1" value="#E06FBB" />
<input type="color" id="spectravella-color2" value="#8D28F6" />
<input type="color" id="spectravella-color3" value="#8FCBE7" />
<input type="color" id="spectravella-color4" value="#F2B077" />

<!-- Background Color -->
<input type="color" id="spectravella-background-color" value="#000000" />

<!-- Update Button -->
<button id="spectravella-updateColors">Update Colors</button>
```

### Default Colors

| Color      | Hex Code  | Description |
| ---------- | --------- | ----------- |
| Color 1    | `#E06FBB` | Pink        |
| Color 2    | `#8D28F6` | Purple      |
| Color 3    | `#8FCBE7` | Light Blue  |
| Color 4    | `#F2B077` | Orange      |
| Background | `#000000` | Black       |

## 📥 Download Feature

Add a download button to let users save the current visualization:

```html
<button id="spectravella-downloadButton">Download</button>
```

## 📁 Project Structure

```
spectravella/
├── index.html          # Demo page with color picker UI
├── spectravella.js     # Main library (includes Three.js)
├── styles.css          # Basic container styles
├── perlinImage/        # Noise textures for effects
│   └── *.png
└── README.md           # This file
```

## 🔧 Integration Examples

### Basic Implementation

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>My Spectravella Page</title>
    <script src="spectravella.js"></script>
    <style>
      body {
        margin: 0;
      }
      .sprectravella-container {
        width: 100%;
        height: 100vh;
      }
    </style>
  </head>
  <body>
    <div class="sprectravella-container"></div>
  </body>
</html>
```

### As a Hero Section

```html
<header class="hero">
  <div class="sprectravella-container"></div>
  <div class="hero-content">
    <h1>Welcome to My Site</h1>
    <p>Beautiful animated backgrounds</p>
  </div>
</header>

<style>
  .hero {
    position: relative;
    height: 100vh;
  }
  .sprectravella-container {
    position: absolute;
    inset: 0;
    z-index: 0;
  }
  .hero-content {
    position: relative;
    z-index: 1;
    color: white;
    text-align: center;
    padding-top: 40vh;
  }
</style>
```

### With Custom Initial Colors

Simply change the `value` attributes on the color inputs to set your preferred starting palette:

```html
<input type="color" id="spectravella-color1" value="#FF6B6B" />
<input type="color" id="spectravella-color2" value="#4ECDC4" />
<input type="color" id="spectravella-color3" value="#45B7D1" />
<input type="color" id="spectravella-color4" value="#96CEB4" />
<input type="color" id="spectravella-background-color" value="#1a1a2e" />
```

## 🎯 Use Cases

- **Landing Pages** - Eye-catching hero sections
- **Portfolio Sites** - Creative backgrounds
- **Music Visualizers** - Ambient visual effects
- **Presentations** - Dynamic slide backgrounds
- **Loading Screens** - Beautiful wait experiences

## ⚠️ Important Notes

1. **Script Placement** - Always include `spectravella.js` in the `<head>` section
2. **Container Class** - Use exactly `sprectravella-container` (note the spelling)
3. **Container Sizing** - The container needs explicit dimensions to render properly
4. **Performance** - Uses WebGL via Three.js; ensure target browsers support it

## 📄 License

MIT License - Copyright 2023 Chris Bedian

Feel free to use in personal and commercial projects.

---

Made with 💜 by [Chris Bedian](https://github.com/chrisbedian)
