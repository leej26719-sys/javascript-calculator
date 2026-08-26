# 🧮 Enhanced JavaScript Calculator

A feature-rich, fully functional calculator built with vanilla HTML, CSS, and JavaScript. Includes scientific functions, keyboard support, memory operations, and calculation history.

## 🌐 Live Demo

**[View Live Calculator](https://leej26719-sys.github.io/javascript-calculator/)**

## ✨ Features

### Basic Calculator
- ✅ Addition, subtraction, multiplication, division, and modulo operations
- ✅ Real-time display updates
- ✅ Clear (C) and backspace (⌫) functions
- ✅ Toggle positive/negative sign (±)

### Keyboard Support
- **Number Keys**: Press `0-9` to input numbers
- **Decimal**: Press `.` to add decimal point
- **Operators**: Press `+`, `-`, `*`, `/` for operations
- **Calculate**: Press `Enter` or `=` to compute result
- **Delete**: Press `Backspace` to remove last character
- **Clear**: Press `C` to clear display
- **Parentheses**: Press `(` and `)` for grouped calculations

### Memory Functions
- **MC** (Memory Clear): Clear stored value
- **MR** (Memory Recall): Retrieve stored value
- **M+** (Memory Add): Add current value to memory
- **M−** (Memory Subtract): Subtract current value from memory
- Memory display shows saved value
- Persistent storage using localStorage

### Scientific Calculator
Accessible via the "Scientific" mode button:
- **Trigonometric**: sin, cos, tan (in degrees)
- **Inverse Trigonometric**: sin⁻¹, cos⁻¹, tan⁻¹
- **Logarithmic**: log (base 10), ln (natural log)
- **Power & Root**: x^y (exponentiation), √ (square root)
- **Constants**: π (pi), e (Euler's number)
- **Other Functions**: Absolute value (|x|), Factorial (n!)
- **Parentheses**: Full support for grouped expressions

### Advanced Features
- 📋 **Calculation History**: Keeps track of last 20 calculations
- 💾 **Persistent Storage**: History and memory saved to browser localStorage
- 🎨 **Beautiful UI**: Modern gradient background, smooth animations, and hover effects
- 📱 **Responsive Design**: Works perfectly on desktop, tablet, and mobile
- ⌨️ **Keyboard Visual Feedback**: Buttons animate when pressed

## 🎮 How to Use

### Basic Operations
1. Click number buttons or press keys to input numbers
2. Click operator buttons or press `+`, `-`, `*`, `/`
3. Click `=` or press `Enter` to calculate
4. Click `C` or press `C` to clear

### Using Memory
1. Enter a number
2. Click **M+** to add to memory or **M−** to subtract from memory
3. Click **MR** to recall the stored value
4. Click **MC** to clear memory
5. Memory value displays at the top of the calculator

### Using Scientific Mode
1. Click the **Scientific** button to expand scientific functions
2. Use buttons for advanced mathematical operations
3. Trigonometric functions use degrees by default
4. Close parentheses automatically tracked

### Viewing History
- Calculation history appears in the right panel
- Click any history item to load that result into the display
- Click **Clear History** to remove all history entries

## 📁 Project Structure

```
javascript-calculator/
├── index.html          # Main calculator application
├── README.md           # This file
└── .nojekyll           # GitHub Pages configuration (auto-generated)
```

## 🚀 Deployment to GitHub Pages

This repository is configured for automatic GitHub Pages deployment:

### Enable GitHub Pages
1. Go to your repository settings
2. Navigate to **Settings** → **Pages**
3. Under "Build and deployment", select:
   - **Source**: Deploy from a branch
   - **Branch**: `main`
   - **Folder**: `/ (root)`
4. Click **Save**

Your calculator will be live at: `https://YOUR_USERNAME.github.io/javascript-calculator/`

### Local Testing
To test locally, simply open `index.html` in your web browser or use a local server:

```bash
# Using Python 3
python -m http.server 8000

# Using Node.js (with http-server)
npm install -g http-server
http-server
```

Then navigate to `http://localhost:8000` in your browser.

## 💾 Data Persistence

The calculator uses browser `localStorage` to save:
- **Calculation History**: Last 20 calculations (key: `calculatorHistory`)
- **Memory Value**: Current memory value (key: `calculatorMemory`)

Data persists across browser sessions until manually cleared.

## 🎨 Customization

### Color Scheme
Modify the CSS gradient in `body` style:
```css
background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
```

### Button Colors
- **Operators**: Change `.operator` background color
- **Numbers**: Change `.number` background color
- **Memory**: Change `.memory` background color
- **Scientific**: Change `.scientific button` background color

### Button Size
Adjust `.buttons grid-template-columns` for different grid layouts:
```css
grid-template-columns: repeat(4, 1fr);  /* Change 4 for different columns */
```

## 🔧 Browser Compatibility

- ✅ Chrome/Edge (latest)
- ✅ Firefox (latest)
- ✅ Safari (latest)
- ✅ Mobile browsers (iOS Safari, Chrome Mobile)

## ⚠️ Known Limitations

- Trigonometric functions use degrees (not radians)
- Very large numbers may display in scientific notation
- Complex expressions require proper parentheses placement
- Some advanced mathematical operations may have floating-point precision issues

## 📝 License

This project is open source and available under the MIT License.

## 🤝 Contributing

Feel free to fork this repository and submit pull requests for any improvements!

## 📧 Contact

For questions or suggestions, please open an issue on the GitHub repository.

---

**Built with ❤️ using HTML, CSS, and JavaScript**
