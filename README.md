# 🚀 Hover Effect Design_1.0

A smooth, modern, GSAP-powered hover animation effect that reveals fullscreen images when hovering over client names.  
This project showcases an interactive UI pattern often used in portfolios, agency websites, and high-end brand showcases.

---

## ✨ Features

- 🔥 **GSAP animations** with custom easing  
- 🎨 Fullscreen image reveal using CSS `clip-path`  
- 🖱️ Hover-driven dynamic transitions  
- 📁 Auto-display of images based on hovered list index  
- 💫 Smooth fade + scale animation

---

## 📂 Project Structure
```bash
project/
│── main.html
│── styling.css
│── animations.js
└── /images
```

### **main.html**  
Contains the markup for the clients section, fixed navigation, and footer.  
It also loads GSAP and the `animations.js` script.  
 [oai_citation:0‡main.html](sediment://file_0000000094c871fa99d89c9384fed690)

### **styling.css**  
Defines layout, typography, fullscreen background preview container, and hover underline animation.  
It also creates the clipped image wrapper effect.  
 [oai_citation:1‡styling.css](sediment://file_00000000fac47243974cf5019f983456)

### **animations.js**  
Handles dynamic image reveal on hover using GSAP.  
- Creates a custom ease curve  
- Sets image scale + opacity  
- Triggers animations on mouseover/mouseout  
 [oai_citation:2‡animations.js](sediment://file_0000000012c071f8ac5a068bcb3b4c77)

---

## 🛠️ Technologies Used

- **HTML5**
- **CSS3**
- **JavaScript (ES Modules)**
- **GSAP 3**
- **GSAP CustomEase**

---

## 🚀 Getting Started

### 1. Clone or Download the Project

```sh
git clone https://github.com/your-username/hover-effect-project.git
```
Or simply download the ZIP.

### 2. Folder Setup

Make sure you have an /images folder inside the project.
Images must follow this naming format:
```sh
img1.jpg
img2.jpg
img3.jpg
...
```

These are called dynamically via:
```sh
clientImg.src = `images/img${index + 1}.jpg`;
```

### 3. Open the Project

Just open main.html in your browser.


No build tools required.

---

## 🔧 How It Works

### Image Reveal Logic

When you hover over a client name:
	1.	A new .client-img-wrapper is created
	2.	The corresponding image is inserted (img1, img2, etc.)
	3.	GSAP animates:
	•	clip-path → from center to fullscreen
	•	opacity → fade in
	•	scale → zoom-in to natural size

When the mouse leaves, GSAP reverses the animation and removes the element from the DOM.

### Custom Ease

A smooth “hop” motion is created with:
```sh
CustomEase.create("hop", "M0, 0 C0.071,0.505 0.192,0.726 0.318,0.852 0.45,0.984 0.504, 1 1,1");
```

---

## 📸 Demo Preview

Just hover over any of the F1 team names (RedBull, Ferrari, McLaren, etc.) and the project’s hover effect reveals their respective image fullscreen.

---

## 👨‍💻 Developer

Designed & Developed by Yourajdeep





