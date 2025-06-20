# Paul Osunero's Blog

A Hugo-powered static site blog hosted on GitHub Pages.

## 🚀 Quick Start

This blog is built with [Hugo](https://gohugo.io/) using the [PaperMod](https://github.com/adityatelange/hugo-PaperMod) theme.

### Prerequisites

- [Hugo Extended](https://gohugo.io/installation/) (latest version)
- [Git](https://git-scm.com/)

### Local Development

1. Clone the repository:
   ```bash
   git clone https://github.com/posunero/posunero.github.io.git
   cd posunero.github.io
   ```

2. Initialize and update the theme submodule:
   ```bash
   git submodule update --init --recursive
   ```

3. Start the development server:
   ```bash
   hugo server -D
   ```

4. Open your browser and navigate to `http://localhost:1313`

## 📝 Creating Content

### New Blog Post

```bash
hugo new content posts/my-new-post.md
```

### New Page

```bash
hugo new content my-new-page.md
```

### Content Structure

- `content/posts/` - Blog posts
- `content/about.md` - About page
- `static/` - Static files (images, favicon, etc.)

## 🛠️ Building for Production

```bash
hugo --gc --minify
```

This generates the static site in the `docs/` directory, which is configured for GitHub Pages deployment.

## 🔄 Deployment

This blog uses GitHub Actions for automatic deployment. Every push to the `main` branch triggers:

1. Building the Hugo site
2. Deploying to GitHub Pages

The workflow is defined in `.github/workflows/deploy.yml`.

## 📁 Project Structure

```
├── .github/workflows/    # GitHub Actions workflows
├── archetypes/           # Content templates
├── assets/               # Hugo Pipes assets
├── content/              # Content files
│   ├── posts/           # Blog posts
│   └── about.md         # About page
├── data/                 # Data files
├── docs/                 # Generated static site (GitHub Pages source)
├── i18n/                 # Internationalization files
├── layouts/              # Custom layout templates
├── static/               # Static files
├── themes/PaperMod/      # PaperMod theme (git submodule)
├── hugo.toml             # Hugo configuration
└── README.md             # This file
```

## ⚙️ Configuration

The main configuration is in `hugo.toml`. Key settings include:

- Site URL: `https://posunero.github.io/`
- Theme: PaperMod
- Publishing directory: `docs/` (for GitHub Pages)

## 🎨 Customization

### Theme Configuration

The PaperMod theme is highly customizable. Check the [theme documentation](https://github.com/adityatelange/hugo-PaperMod/wiki) for available options.

### Custom Styling

Add custom CSS in `assets/css/extended/` (this will be automatically included by the theme).

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🤝 Contributing

Feel free to open issues or submit pull requests if you find any bugs or have suggestions for improvements!

---

Built with ❤️ using [Hugo](https://gohugo.io/) and [PaperMod](https://github.com/adityatelange/hugo-PaperMod) 