# Personal Portfolio Website

A modern and responsive portfolio website showcasing my skills, experience, and projects as a Data Analyst. Built with HTML, CSS, and JavaScript.

![Portfolio Preview](images/portfolio/portfolio-1.jpg)

## 🚀 Live Demo
[View Portfolio](https://your-portfolio-url.com)

## ✨ Features

- 📱 **Fully Responsive Design**
  - Mobile-first approach
  - Breakpoints at 1199px, 991px, and 767px
  - Smooth transitions and animations

- 🎨 **Theme Customization**
  - 5 different color themes
  - Dark/Light mode toggle
  - Custom CSS variables for easy styling

- 💼 **Professional Sections**
  - Dynamic typing effect for job titles
  - Skills progress bars with percentages
  - Interactive portfolio gallery
  - Working contact form

## Sections

### 1. Home
- Professional introduction
- Hero image
- Quick about me
- Call-to-action buttons

### 2. About
- Detailed personal information
- Professional skills with progress bars
- Educational timeline
- Experience timeline 
- Downloadable CV

### 3. Services
- Web Design
- SQL Querying & Database Management
- Data Visualization
- Data Cleaning & Preprocessing
- Predictive Analytics & Machine Learning Models

### 4. Portfolio
- Project gallery with 6 showcase items
- Project images with hover effects
- Shadow effects for visual appeal

### 5. Contact
- Contact information
- Location details
- Email form
- Social media links

## 🛠️ Technical Stack

- **Frontend:**
  - HTML5
  - CSS3 (Custom properties, Flexbox, Grid)
  - JavaScript (ES6+)
  - [Typed.js](https://github.com/mattboldt/typed.js/) for typing animation

- **External Libraries:**
  - Font Awesome 6.7.2
  - Google Fonts (Poppins, Caveat)

## 📂 Project Structure

```
Portfolio/
├── CSS/
│   ├── style.css          # Main styles
│   ├── color.css          # Default theme
│   ├── color1.css         # Theme variation 1
│   ├── color2.css         # Theme variation 2
│   ├── color3.css         # Theme variation 3
│   ├── color4.css         # Theme variation 4
│   ├── color5.css         # Theme variation 5
│   └── style-switcher.css # Theme switcher styles
├── JS/
│   ├── script.js          # Main functionality
│   └── switcher.js        # Theme switching logic
├── images/
│   ├── hero.jpg
│   └── portfolio/
│       ├── Logo.png
│       └── portfolio-1.jpg to portfolio-6.jpg
├── index.html             # Main HTML file
└── README.md             # Documentation
```

## 🎯 Core Components

### 1. Theme Switcher
```javascript
const setActiveStyle = (color) => {
    alternateStyles.forEach((style) => {
        if(color === style.getAttribute("title")) {
            style.removeAttribute("disabled");
        } else {
            style.setAttribute("disabled","true");
        }
    })
}
```

### 2. Dynamic Typing Effect
```javascript
var typed = new Typed(".typing", {
    strings: ["", "Web-developer", "Data-analyst", "Python-developer"],
    typeSpeed: 100,
    BackSpeed: 60,
    loop: true
});
```

### 3. Responsive Navigation
```javascript
const navTogglerBtn = document.querySelector(".nav-toggle");
navTogglerBtn.addEventListener("click", () => {
    aside.classList.toggle("open");
});
```

## 🚀 Getting Started

1. **Clone the repository:**
```bash
git clone https://github.com/yourusername/portfolio.git
```

2. **Navigate to project directory:**
```bash
cd portfolio
```

3. **Open in browser:**
- Double click `index.html` or use Live Server in VS Code

## 📱 Responsive Design

- **Desktop (>1199px)**: Full sidebar navigation
- **Tablet (991px-1199px)**: Collapsible sidebar
- **Mobile (<767px)**: 
  - Stack layout
  - Full-width sections
  - Touch-friendly navigation

## 🎨 Color Themes

| Theme | Primary Color | Active Color |
|-------|--------------|--------------|
| Default | #B82132 | #DE3163 |
| Theme 1 | #362222 | #4A3131 |
| Theme 2 | #EB8317 | #F49B2E |
| Theme 3 | #48CFCB | #5FE7E3 |
| Theme 4 | #8F43EE | #A35EFF |
| Theme 5 | #FF597B | #FF7C97 |

## 🔧 Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Brave (latest)

## 📄 License

This project is open source and available under the MIT License.

## 📞 Contact

- Email: ronitprasad48@gmail.com
- LinkedIn: [Ronit Prasad](https://www.linkedin.com/in/ronit-prasad-aaa0122a2/)
- Website: www.domain.com

## 🔄 Future Updates

- [ ] Add blog section
- [ ] Implement dark mode persistence
- [ ] Add project filtering
- [ ] Integrate with a backend for contact form
- [ ] Add animation on scroll effects
