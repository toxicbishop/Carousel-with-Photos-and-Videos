# CSS & JavaScript Carousel

A lightweight, responsive media carousel built with pure HTML, CSS, and JavaScript. It supports both images and videos, features smooth scrolling with snap effects, and offers intuitive navigation via buttons, pagination dots, and keyboard controls.

![Carousel Preview](Title/Carousel.png)

## ✨ Features

- **Zero Dependencies**: Built with vanilla HTML, CSS, and JS. No frameworks or libraries.
- **Mixed Media**: Supports both `<img>` and `<video>` elements interchangeably.
- **Responsive Design**: Adapts fluidly to different screen sizes (Desktop, Tablet, Mobile).
- **Navigation**:
  - 🖱️ **Click**: Left/Right arrows and pagination dots.
  - ⌨️ **Keyboard**: Arrow Left/Right key support.
  - 👆 **Touch**: Native horizontal scroll with snap behavior.
- **Smooth Animations**: CSS transitions for hover effects and scrolling.
- **Modern Styling**: Uses CSS variables, gradients, and subtle glow effects.

## 🚀 Getting Started

Since this project uses no build tools, running it is extremely simple.

### Prerequisites
- A modern web browser (Chrome, Firefox, Edge, Safari).

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/carousel-project.git
   ```
2. Navigate to the project folder:
   ```bash
   cd carousel-project
   ```
3. Open `index.html` in your browser.

> **Note**: For video autoplay to work reliably in some browsers, you may need to serve the files via a local server (like Live Server in VS Code) rather than opening the file directly.

## 🛠️ Customization

### Adding Media
1. Place your images or videos in the `images/` folder.
2. Add a new `.Card` element to the `.carousel` container in `index.html`:

**For Images:**
```html
<div class="Card">
  <img src="images/your-image.jpg" alt="Description" />
</div>
```

**For Videos:**
```html
<div class="Card">
  <video src="images/your-video.mp4" autoplay muted loop></video>
</div>
```

*The pagination dots are automatically generated based on the number of cards found.*

### Changing Colors
All colors are defined as CSS variables in `:root` at the top of `style.css`. You can easily theme the carousel by changing these values:

```css
:root {
  --primary-color: #1a1a2e;      /* Card background */
  --background-color: #0e0e1a;   /* Page background */
  --button-color: #5c4cda;       /* Button gradient start */
  --accent-color: #7a6be6;       /* Hovers & accents */
  /* ... */
}
```

## 📁 Project Structure

```
├── index.html       # Main HTML structure & inline JavaScript
├── style.css        # All styling, animations, and responsive rules
├── images/          # Assets folder for carousel media
├── Title/           # Assets for favicon/metadata
└── README.md        # Project documentation
```

## 🤝 Contributing

Feel free to fork this project and submit pull requests. You can also open issues for bugs or feature suggestions.

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
