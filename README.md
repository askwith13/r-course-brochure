# Master R Programming - Course Brochure

A professional brochure website for R Programming courses, built with Python and static HTML/CSS/JavaScript. This website is designed to be hosted on GitHub Pages.

## 🚀 Features

- **Responsive Design**: Works seamlessly on desktop, tablet, and mobile devices
- **Modern UI**: Clean, professional design with smooth animations
- **Easy Navigation**: Smooth scrolling navigation between sections
- **All Course Information**: Complete details about the R Programming course curriculum

## 📁 Project Structure

```
.
├── generate_site.py    # Python script to generate the HTML
├── index.html          # Main HTML file (generated)
├── styles.css          # CSS stylesheet
├── script.js           # JavaScript for interactivity
├── images/             # Course images
│   ├── R-Programming-Course.jpg
│   ├── instructor1.jpg
│   └── Payment-links.jpg
└── README.md           # This file
```

## 🛠️ Setup Instructions

### Local Development

1. **Clone or download this repository**
   ```bash
   git clone <your-repo-url>
   cd "Landing page R course brochure"
   ```

2. **Generate the HTML file** (if needed)
   ```bash
   python3 generate_site.py
   ```

3. **Open in browser**
   - ⚠️ **Important**: Don't open `index.html` directly in your browser (file:// protocol won't load images)
   - Use a local server instead:
     ```bash
     python3 -m http.server 8000
     ```
     Then visit `http://localhost:8000` in your browser
   - Images will only load when served through HTTP, not when opening the file directly

### Hosting on GitHub Pages

1. **Create a GitHub repository**
   - Go to GitHub and create a new repository
   - Name it (e.g., `r-course-brochure`)

2. **Push your code to GitHub**
   ```bash
   git init
   git add .
   git commit -m "Initial commit: R Course Brochure website"
   git branch -M main
   git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git
   git push -u origin main
   ```

3. **Enable GitHub Pages**
   - Go to your repository on GitHub
   - Click on **Settings**
   - Scroll down to **Pages** section (in the left sidebar)
   - Under **Source**, select **Deploy from a branch**
   - Choose **main** branch and **/ (root)** folder
   - Click **Save**

4. **Access your website**
   - Your site will be available at:
     `https://YOUR_USERNAME.github.io/YOUR_REPO_NAME/`
   - It may take a few minutes for the site to be live

## 📝 Customization

### Updating Content

You can edit the content in two ways:

1. **Edit the Python script** (`generate_site.py`):
   - Modify the HTML content in the `generate_html()` function
   - Run `python3 generate_site.py` to regenerate `index.html`

2. **Edit HTML directly** (`index.html`):
   - Make changes directly to `index.html`
   - Note: Changes will be overwritten if you run `generate_site.py` again

### Updating Styles

- Edit `styles.css` to change colors, fonts, spacing, etc.
- The design uses a blue gradient theme (#1e3a8a to #3b82f6)

### Updating Images

- Replace images in the `images/` folder
- Keep the same filenames or update the paths in `index.html`

## 🔧 Requirements

- Python 3.x (for generating HTML)
- Modern web browser (Chrome, Firefox, Safari, Edge)
- Git (for version control and GitHub Pages)

## 📧 Contact Information

For course inquiries:
- Email: aswathkarunakaran@gmail.com
- Phone/WhatsApp: +91-9895973729

## 📄 License

This project is for educational purposes. All course content belongs to Dr. Aswath Karunakaran.

## 🙏 Acknowledgments

- Built with Bootstrap 5.3.0
- Original design inspired by Shiny R applications

