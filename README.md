# Mega Shop — 3D Print Cost Calculator

<p align="center">
  <img src="logo.jpg" alt="Mega Shop Logo" width="110">
</p>

<p align="center">
  <strong>A clean, modern and lightweight 3D printing cost calculator.</strong>
</p>

<p align="center">
  Calculate material cost, machine time, multi-part prints and final pricing directly in your browser.
</p>

---

## ✨ Features

- **Multi-part print support** — add as many printed parts as needed.
- **Weight calculation** — enter the weight of every part in grams.
- **Time calculation** — enter hours and minutes for every part.
- **Automatic totals** — all part weights and printing times are combined automatically.
- **Material pricing** — calculated from the total weight.
- **Machine pricing** — calculated from the total printing time.
- **Editable rates** — change the material and machine rates from the **Rates** modal.
- **Persistent settings** — custom rates are saved in the browser using `localStorage`.
- **Responsive design** — works on desktop, tablet and mobile.
- **No backend required** — everything runs locally in the browser.
- **GitHub Pages ready** — deploy it as a static website with no build step.

---

## 🧮 How It Works

The calculator uses two pricing rates:

| Rate | Default |
|---|---:|
| Material | `5,000 Toman / gram` |
| Machine time | `135,000 Toman / hour` |

### Material Cost

```text
Material Cost = Total Weight × Material Rate
```

### Machine Cost

```text
Machine Cost = Total Printing Time × Machine Rate
```

Minutes are converted into a fraction of an hour automatically.

For example:

```text
30 minutes = 0.5 hour
45 minutes = 0.75 hour
90 minutes = 1.5 hours
```

### Final Price

```text
Final Price = Material Cost + Machine Cost
```

---

## 🧩 Multi-Part Products

Some 3D printed products consist of multiple separate pieces.

For example:

| Part | Weight | Time |
|---|---:|---:|
| Part 1 | 120 g | 2h 30m |
| Part 2 | 80 g | 1h 20m |
| Part 3 | 45 g | 50m |

The calculator automatically combines them:

```text
Total Weight = 245 g
Total Time   = 4h 40m
```

Then it calculates the final price using the configured rates.

Use **+ Add Part** to add another piece and the `×` button to remove a piece.

---

## ⚙️ Changing Pricing Rates

Click the **Rates** button in the top-right corner.

You can change:

- Material rate per gram
- Machine rate per hour

After clicking **Save Rates**, the new values are immediately used by the calculator.

Your custom rates are stored in the browser, so they remain available when you return to the page on the same browser/device.

---

## 📁 Project Structure

```text
mega-shop-print-calculator/
├── index.html
├── logo.jpg
└── README.md
```

The project intentionally has no framework, package manager or build process.

---

## 🚀 Run Locally

No installation is required.

Simply open:

```text
index.html
```

in a modern web browser.

For local development, you can also use any static server.

For example with VS Code, the **Live Server** extension can be used.

---

## 🌐 Deploy on GitHub Pages

### 1. Create a repository

Create a new GitHub repository, for example:

```text
mega-shop-print-calculator
```

### 2. Upload the project

Upload:

```text
index.html
logo.jpg
README.md
```

### 3. Enable GitHub Pages

Go to:

```text
Repository → Settings → Pages
```

Under **Build and deployment**, select:

```text
Source: Deploy from a branch
Branch: main
Folder: / (root)
```

Save the settings.

GitHub will provide your public website URL after deployment.

---

## 🎨 Design

The interface follows the Mega Shop visual direction:

- Deep black background
- Vivid red accent
- Minimalist layout
- Rounded modern cards
- Soft cinematic gradients
- Subtle borders and shadows
- Responsive typography
- Clean product-oriented aesthetic

The primary accent color is:

```text
#E01B1B
```

---

## 🔒 Privacy

This calculator does not send calculation data to a server.

All calculations happen locally in the browser.

The only persistent data is the pricing configuration stored in:

```text
localStorage
```

---

## 🛠️ Technology

Built with:

- HTML5
- CSS3
- Vanilla JavaScript
- Browser LocalStorage

No external dependencies are required.

---

## 📄 License

This project is intended for **Mega Shop** use.

You can modify the source code and pricing logic to match your own 3D printing workflow.

---

<p align="center">
  <strong>Mega Shop</strong><br>
  3D Printing Cost Calculator
</p>
