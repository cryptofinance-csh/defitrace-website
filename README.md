# DeFiTrace Website

Official website for the DeFiTrace project - a research initiative led by Complexity Science Hub Vienna.

## Prerequisites

Before you begin, ensure you have the following installed on your system:

### 1. Node.js

Install Node.js 20.x (LTS) using NodeSource repository:

```bash
# For Node.js 20.x (LTS)
curl -fsSL https://deb.nodesource.com/setup_20.x | sudo -E bash -
sudo apt-get install -y nodejs
```

Verify installation:
```bash
node --version  # Should show v20.x.x
npm --version   # Should show 10.x.x
```

### 2. pnpm

Install pnpm package manager:

```bash
curl -fsSL https://get.pnpm.io/install.sh | sh -
```

After installation, you may need to restart your terminal or run:
```bash
source ~/.bashrc
```

Verify installation:
```bash
pnpm --version
```

## Installation

### 1. Clone the repository

```bash
git clone <repository-url>
cd defitrace-website
```

### 2. Install Dependencies

```bash
pnpm install
```

This will install all required dependencies including:
- Astro
- TailwindCSS
- MDX support
- Sharp (for image optimization)
- And other necessary packages

### 3. Start Development Server

```bash
pnpm run dev
```

The site will be available at `http://localhost:4321`

### 4. Build for Production

```bash
pnpm run build
```

The built files will be in the `dist/` directory.

### 5. Preview Production Build

```bash
pnpm run preview
```

## Cleaning the Project

To remove build artifacts and start fresh:

```bash
rm -rf .astro dist node_modules
pnpm install
pnpm run build
```

## Project Structure

```
/
├── public/          # Static assets (images, fonts, etc.)
├── src/
│   ├── components/  # Reusable Astro components
│   ├── layouts/     # Page layouts
│   └── pages/       # Page routes
│       ├── index.astro      # Homepage
│       ├── contact.astro    # Contact page
│       ├── consortium.astro # Consortium page
│       ├── results.astro    # Results page
│       └── 404.astro        # 404 error page
├── astro.config.mjs
├── tailwind.config.cjs
└── package.json
```

## Technologies Used

- **Astro 4.16.14** - Static Site Generator
- **TailwindCSS 3.4.18** - Utility-first CSS framework
- **MDX** - Markdown with JSX support
- **Sharp** - Image optimization
- **Astro Icon** - Icon system

## Contact Information

**Complexity Science Hub Vienna**  
Metternichgasse 8  
1030 Vienna, Austria

Email: contact@defitrace.info  
Phone: +43 1 59991 600

## License

GPL-2.0

## Credits

This website is built with Astro and TailwindCSS, based on the Astroship template.
