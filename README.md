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

## 🌐 Deploying to GoDaddy (cPanel / Web Hosting)

Because your portfolio is built with pure semantic **HTML5, Vanilla CSS, and JavaScript**, it is **100% compatible with GoDaddy Web Hosting** (or any cPanel Linux/Apache hosting). No Node.js server, build tools, or databases are needed on the server!

We have also created a pre-configured [`.htaccess`](file:///Users/vikasmalik/Desktop/Life%20OS%20/Personal%20Portfolio%20/.htaccess) file with:
- Automatic **HTTPS redirection**
- **Gzip compression** for instant page loading
- **Long-term browser caching** for images, fonts, CSS, and JS
- **Security headers** (`X-Frame-Options`, `X-Content-Type-Options`)

---

### Step-by-Step GoDaddy cPanel Upload (Fastest & Easiest)

1. **Generate or use the ready zip package**:
   In your project root, run:
   ```bash
   npm run package:godaddy
   ```
   *(A pre-packaged file [`godaddy-portfolio.zip`](file:///Users/vikasmalik/Desktop/Life%20OS%20/Personal%20Portfolio%20/godaddy-portfolio.zip) has already been created for you!)*

2. **Log in to GoDaddy**:
   - Go to your [GoDaddy Account](https://account.godaddy.com/).
   - Under **Web Hosting**, find your hosting plan and click **Manage** or **cPanel Admin**.

3. **Open File Manager**:
   - In cPanel, open **File Manager** (under *Files*).
   - In the left sidebar, click on **`public_html`** (this is your root website directory).
   - *Note: If you have a default `index.html` or GoDaddy placeholder page in `public_html`, delete or backup that file.*

4. **Upload & Extract**:
   - Click the **Upload** button in the top toolbar.
   - Select or drag-and-drop `godaddy-portfolio.zip`.
   - Once upload reaches 100%, return to `public_html`.
   - Right-click `godaddy-portfolio.zip` and select **Extract** (extract directly into `public_html`).
   - You can then delete the `.zip` file from the server.

5. **Ensure Hidden Files Are Visible (`.htaccess`)**:
   - In File Manager, click **Settings** (top right gear icon).
   - Check **"Show Hidden Files (dotfiles)"** and click **Save**.
   - Verify that `.htaccess` is present in `public_html`.

6. **Done!**:
   - Visit your domain (e.g. `yourdomain.com`). Your sleek dark executive portfolio is now live!

---

### Alternative: Deploy via FTP / SFTP (FileZilla or Cyberduck)

If you prefer uploading directly via an FTP client:
1. In GoDaddy cPanel, find your **FTP Accounts** or use your cPanel username & password.
2. Connect to your host with host name `ftp.yourdomain.com` (or your server IP).
3. Navigate to the `/public_html/` folder.
4. Drag and drop the following files/folders into `/public_html/`:
   - `index.html`
   - `css/`
   - `js/`
   - `assets/`
   - `.htaccess`
