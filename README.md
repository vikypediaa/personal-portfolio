# Vikas Malik &mdash; Executive Personal Portfolio

A sleek, responsive, executive-grade personal portfolio website tailored for **Vikas Malik** (Direct Scaled Acquisitions Lead &mdash; EMEA @ Google | Growth Marketing & Automation | Digital Transformation).

Built with semantic **HTML5**, **Vanilla CSS (Design Tokens, Glassmorphism, Responsive Grid)**, and **Vanilla JavaScript** &mdash; delivering instant page loads, zero build overhead, and maximum flexibility.

---

## 🌟 Key Features

- **Executive Dark/Light Mode**: Styled in deep obsidian slate with frosted glass panels, ambient cyan/blue gradients, and a live toggle with localStorage persistence.
- **Dynamic Hero Section**: Highlighting leadership role at Google, location, value propositions, and direct CTA actions.
- **Leadership Metrics Ribbon**: Showcases 9+ years at Google, EMEA scope, MBA credentials, and global brand impact.
- **Interactive Career Timeline**: Chronological career trajectory covering roles across Google EMEA, Google Ads, Google Cloud, BlackRock, and earlier leadership.
- **Categorized MarTech Arsenal**: Filterable skill matrix (Growth & Strategy, MarTech & Automation, Data & Analytics) covering Salesforce, Marketo, Tableau, GTM, etc.
- **Enterprise Campaigns Showcase**: Highlights major campaigns across Google Cloud, Google Ads, BlackRock, Volvo, and BP.
- **Credentials & Certifications**: Detailed breakdown of Strathclyde MBA, Salesforce Certified Administrator (SCA), AgilePM Practitioner, and Marketo Certified Associate.
- **Direct Connect Hub**: One-click email copy with visual toast confirmation, direct mailto link, and verified LinkedIn profile link.

---

## 📁 Directory Structure

```
.
├── index.html               # Main semantic HTML structure & SEO meta
├── css/
│   ├── variables.css        # Design tokens, color palettes & themes (Dark & Light)
│   ├── base.css             # CSS reset, typography, and utility classes
│   ├── components.css       # Nav, Hero, Timeline, Cards, Badges, Footer
│   └── responsive.css       # Breakpoints for mobile, tablet, and widescreen
├── js/
│   └── main.js              # Theme switcher, mobile menu, filters, copy toast
├── assets/
│   ├── images/
│   │   └── profile.jpg      # Executive headshot portrait
│   └── icons/               # SVG / branding assets
├── package.json             # Quick scripts for local development
└── README.md                # Documentation and deployment guide
```

---

## 🚀 Running Locally

You can preview the site immediately using any of the following methods:

### Option 1: Via npm (Recommended)
```bash
npm run dev
```
Then open [http://localhost:3000](http://localhost:3000) in your browser.

### Option 2: Via Python
```bash
python3 -m http.server 3000
```
Then open [http://localhost:3000](http://localhost:3000).

### Option 3: Direct File Open
Simply double-click `index.html` or open it in any web browser (Chrome, Safari, Edge, Firefox).

---

## 🛠️ How to Customize

- **Updating Profile Photo**: Replace `assets/images/profile.jpg` with your preferred high-resolution photo.
- **Editing Bio & Content**: Modify the text inside `index.html`. All sections have clear IDs (`#about`, `#experience`, `#competencies`, `#impact`, `#credentials`, `#contact`).
- **Colors & Accents**: Adjust brand accent colors in `css/variables.css` (e.g. `--brand-blue`, `--brand-cyan`, `--brand-emerald`).

---

## 🌐 Deploying to Vercel

The portfolio is pre-configured for **Vercel** with a custom [`vercel.json`](file:///Users/vikasmalik/Desktop/Life%20OS%20/Personal%20Portfolio%20/vercel.json) supporting:
- **Clean URLs** (no ugly `.html` extensions)
- **High-performance HTTP Cache-Control headers** for static assets, CSS, and JS
- **Enterprise security headers** (`X-Frame-Options`, `X-Content-Type-Options`, `Referrer-Policy`)
- **Zero build step required** (instant deploys)

### Method 1: Deploy via Vercel CLI (Fastest)

Run the following in your terminal:
```bash
# Preview deployment
npm run deploy

# Production deployment
npm run deploy:prod
```
The CLI will ask you to confirm the project settings (accept defaults: framework "Other", root directory `./`).

### Method 2: Deploy via GitHub Integration (Recommended for Continuous Deployment)

1. Initialize a git repository and push to GitHub:
   ```bash
   git init
   git add .
   git commit -m "Initial portfolio setup"
   git branch -M main
   git remote add origin https://github.com/<your-username>/<your-repo-name>.git
   git push -u origin main
   ```
2. Open the [Vercel Dashboard](https://vercel.com/new).
3. Click **"Add New Project"** > **"Import Git Repository"**.
4. Select your portfolio repo and click **Deploy**.
5. Any subsequent `git push` to your repository will automatically trigger an instant deployment.

### Custom Domain on Vercel
Once deployed on Vercel:
1. Go to your Project on Vercel > **Settings** > **Domains**.
2. Add your custom domain (e.g., `vikasmalik.com`).
3. Follow the DNS records shown (add the CNAME / A record in your domain registrar like Namecheap, GoDaddy, Google Domains / Squarespace). Vercel provisions free automatic SSL certificates!
