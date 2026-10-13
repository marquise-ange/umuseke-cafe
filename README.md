# Umuseke Café 

Umuseke Café is a responsive café website built with HTML and CSS, featuring two versions: Plain CSS and Tailwind CSS. The project demonstrates modern web design and compares two approaches to styling a website.

##  Live Website

[Visit Umuseke Café] https://umuseke-cafe.netlify.app/

##  Features

- Responsive café website design
- Two versions of the website: Plain CSS and Tailwind CSS
- Modern layout and styling
- Practice with frontend development and responsive design
- Built with Vite for development and production builds
- Deployed using Netlify

##  Technologies Used

- HTML5
- CSS3
- Tailwind CSS v4
- Vite
- Git and GitHub
- Netlify


*Note: `public/` and `dist/` may not exist until you create the deployment files and run a production build.*

##  Website Versions

### 1. Plain CSS

The Plain CSS version uses standard CSS rules written in a stylesheet. It helps demonstrate how layouts, colors, spacing, typography, and responsive behavior can be controlled directly with CSS.

### 2. Tailwind CSS

The Tailwind CSS version uses utility classes to style HTML elements. Instead of writing a separate CSS rule for every component, utility classes can be combined directly in the HTML.

##  Understanding `public/` and `dist/`

These folders have different purposes.

### `public/` — Files to include in the build

Vite copies files from the root `public/` folder into the production output folder. In this project, we used it to include the Plain CSS and Tailwind CSS pages so they could be accessed after deployment.

The original files in `plain-css/` and `Tailwind-css/` are where the website pages are maintained. If you manually copy those files into `public/`, remember to copy any changes you make later.

### `dist/` — Production website

The `dist/` folder is generated when you run the build command:


npm run build


It contains the files that Netlify publishes. You normally do not edit files inside `dist/` directly because the next build can replace them.

**Important:** Having duplicate files in `public/` and the original folders can make the project harder to maintain. A better long-term setup is to keep one authoritative copy of each page and configure the build process to publish both versions automatically.

##  Run the Project Locally

### 1. Clone the repository


git clone https://github.com/marquise-ange/umuseke-cafe.git

### 2. Enter the project folder


cd umuseke-cafe


### 3. Install dependencies


npm install


### 4. Start the development server


npm run dev


Open the local URL shown in your terminal.

### 5. Build for production


npm run build


Vite generates the production files in `dist/`.

##  Deployment

The website is deployed through Netlify, connected to the GitHub repository.

Recommended build settings:

- **Build command:** `npm run build`
- **Publish directory:** `dist`

After pushing changes to the connected GitHub branch, Netlify can automatically build and deploy the updated website.

##  Project Goal

The goal of Umuseke Café is to strengthen frontend development skills by building a responsive website and comparing traditional CSS styling with Tailwind CSS.

