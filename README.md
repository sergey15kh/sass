# 🧱 SCSS Architecture — Clean & Scalable

A modular and scalable SCSS architecture for modern front-end projects.  
Organized with separation of concerns, performance, and developer experience in mind.

---

## 📁 Folder Structure

```bash
sass/
├── helpers/     # Variables, functions, mixins, breakpoints
├── base/        # Normalize, resets, typography
├── layout/      # Grids, wrappers, containers
├── components/  # Reusable UI (buttons, inputs, cards)
├── sections/    # Page sections (header, footer, hero)
├── vendors/     # 3rd-party styles (e.g. Swiper)
└── style.scss   # Main entry point

🚀 Setup and Usage
1. Install Dependencies
To get started, first install npm (Node Package Manager) if you haven't already.

Run the following commands to install necessary dependencies:

bash
Copy
npm init -y
npm install sass --save-dev
2. Add Scripts to package.json
Add the following scripts in your package.json to compile and watch SCSS files:

json
Copy
{
  "scripts": {
    "sass": "sass assets/sass/style.scss assets/css/style.css --no-source-map --style=compressed",
    "sass:watch": "sass --watch assets/sass/style.scss assets/css/style.css --no-source-map"
  }
}
3. Compile SCSS
To compile your SCSS into CSS, use the following command:

bash
Copy
npm run sass
This will compile your SCSS file located in assets/sass/style.scss to assets/css/style.css.

4. Watch SCSS Changes
To automatically recompile your SCSS when changes are made, use the watch command:

bash
Copy
npm run sass:watch
This will watch for any changes in your SCSS files and automatically compile them into CSS.
