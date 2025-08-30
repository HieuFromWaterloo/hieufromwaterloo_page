# HieuFromWaterloo Academic Portfolio

[![Screenshot](./preview.png)](https://hieufromwaterloo.netlify.app/)

**Hieu Quoc Nguyen's** academic and professional portfolio website built with Hugo Academic Theme. This site showcases my journey as a Full Stack Data Scientist with expertise in machine learning, deep learning, and data engineering.

**Live Site**: [hieufromwaterloo.ca](https://hieufromwaterloo.ca/) or [hieufromwaterloo.netlify.app](https://hieufromwaterloo.netlify.app/)

## Local Development Setup

### Prerequisites

Before you begin, ensure you have the following installed on your system:

#### 1. Install Hugo Extended

Hugo Extended is required for SCSS processing and the Academic theme.

**For Windows (WSL/Linux):**
```bash
# Download Hugo Extended v0.119.0 (same version as production)
wget https://github.com/gohugoio/hugo/releases/download/v0.119.0/hugo_extended_0.119.0_linux-amd64.deb
sudo dpkg -i hugo_extended_0.119.0_linux-amd64.deb
rm hugo_extended_0.119.0_linux-amd64.deb

# Verify installation
hugo version
```

**For macOS:**
```bash
brew install hugo
```

**For Windows (Chocolatey):**
```bash
choco install hugo-extended
```

#### 2. Install Go

Go is required for Hugo modules to work properly.

**For Linux/WSL:**
```bash
# Download and install Go
wget https://go.dev/dl/go1.21.0.linux-amd64.tar.gz
sudo tar -C /usr/local -xzf go1.21.0.linux-amd64.tar.gz
rm go1.21.0.linux-amd64.tar.gz

# Add to PATH (add this to your ~/.bashrc or ~/.zshrc)
export PATH=$PATH:/usr/local/go/bin

# Verify installation
go version
```

**For macOS:**
```bash
brew install go
```

### Building the Site

1. **Clone the repository:**
```bash
git clone https://github.com/HieuFromWaterloo/hieufromwaterloo.github.io.git
cd hieufromwaterloo.github.io
```

2. **Download Hugo modules:**
```bash
# Ensure Go is in your PATH
export PATH=$PATH:/usr/local/go/bin

# Download and organize Hugo modules
hugo mod tidy
```

3. **Start the development server:**
```bash
# Start server with draft content
hugo server -D

# Or bind to all interfaces (useful for WSL)
hugo server -D --bind 0.0.0.0 --port 1313
```

4. **Access your site:**
   - Open your browser and go to: http://localhost:1313/
   - The site will automatically reload when you make changes

### Development Commands

| Command | Description |
|---------|-------------|
| `hugo server -D` | Start development server with drafts |
| `hugo server --disableFastRender` | Full rebuilds on change |
| `hugo --gc --minify` | Build for production |
| `hugo --gc --minify --buildFuture` | Build with future-dated posts |
| `hugo mod get -u` | Update Hugo modules |
| `hugo mod tidy` | Clean up module dependencies |

### Project Structure

```
├── config/_default/     # Site configuration
│   ├── config.yaml     # Main Hugo config
│   ├── params.yaml     # Theme parameters
│   ├── menus.yaml      # Navigation menus
│   └── languages.yaml  # Language settings
├── content/            # Site content
│   ├── authors/        # Author profiles
│   ├── project/        # Research projects
│   ├── publication/    # Academic publications
│   └── post/          # Blog posts
├── static/            # Static files (images, PDFs, etc.)
├── assets/            # Assets for processing
└── public/            # Generated site (after build)
```

### Features

This academic portfolio includes:

- **Interactive Project Portfolio** - Showcasing ML/AI projects with filtering
- **Professional Experience Timeline** - Career progression and achievements  
- **Certificates & Education** - Academic credentials and certifications
- **Publications & Research** - Academic papers and research work
- **Technical Skills Display** - Technology stack and competencies
- **Responsive Design** - Optimized for all device sizes
- **SEO Optimized** - Enhanced search engine visibility

### Troubleshooting

**Common Issues:**

1. **"binary with name 'go' not found"**
   ```bash
   # Make sure Go is in your PATH
   export PATH=$PATH:/usr/local/go/bin
   # Add this line to your ~/.bashrc or ~/.zshrc for permanent setup
   ```

2. **Hugo modules not downloading**
   ```bash
   # Clear module cache and retry
   hugo mod clean
   hugo mod tidy
   ```

3. **Permission denied on Linux/WSL**
   ```bash
   # Make sure you have proper permissions for /usr/local
   sudo chown -R $USER:$USER /usr/local/go
   ```

4. **WSL networking issues**
   ```bash
   # Use bind to all interfaces
   hugo server -D --bind 0.0.0.0 --port 1313
   ```

### Content Management

**Adding New Projects:**
1. Create a new folder in `content/project/your-project-name/`
2. Add `index.md` with project metadata and description
3. Include a `featured.png` image for the project thumbnail

**Editing Your Profile:**
- Main profile: `content/authors/admin/_index.md`
- Avatar image: `content/authors/admin/avatar_hqn_270px.jpg`

**Updating Experience:**
- Edit the experience section in `content/_index.md`

**Adding Certificates:**
- Update the accomplishments section in `content/_index.md`
- Add certificate PDFs to `static/uploads/certs/`

### Deployment

This site is configured for **Netlify** deployment:

- **Production URL**: https://hieufromwaterloo.netlify.app/
- **Auto-deployment**: Triggered on Git push to main branch
- **Build command**: `hugo --gc --minify -b $URL`
- **Hugo version**: v0.119.0 (specified in `netlify.toml`)

### About

This is **Hieu Quoc Nguyen's** academic and professional portfolio website. The Hugo **Academic Resumé Template** empowers you to easily create your job-winning online resumé, showcase your academic publications, and create online courses or knowledge bases to grow your audience.

---

## Additional Resources

[![Get Started](https://img.shields.io/badge/-Get%20started-ff4655?style=for-the-badge)](https://wowchemy.com/hugo-themes/)
[![Discord](https://img.shields.io/discord/722225264733716590?style=for-the-badge)](https://discord.com/channels/722225264733716590/742892432458252370/742895548159492138)  
[![Twitter Follow](https://img.shields.io/twitter/follow/wowchemy?label=Follow%20on%20Twitter)](https://twitter.com/wowchemy)

️**Trusted by 250,000+ researchers, educators, and students.** Highly customizable via the integrated **no-code, widget-based Wowchemy page builder**, making every site truly personalized ⭐⭐⭐⭐⭐

Easily write technical content with plain text Markdown, LaTeX math, diagrams, RMarkdown, or Jupyter, and import publications from BibTeX.

[Check out the latest demo](https://academic-demo.netlify.app/) of what you'll get in less than 10 minutes, or [get inspired by our academics and research groups](https://wowchemy.com/creators/).

The integrated [**Wowchemy**](https://wowchemy.com) website builder and CMS makes it easy to create a beautiful website for free. Edit your site in the CMS (or your favorite editor), generate it with [Hugo](https://github.com/gohugoio/hugo), and deploy with GitHub or Netlify. Customize anything on your site with widgets, light/dark themes, and language packs.

- 👉 [**Get Started**](https://wowchemy.com/hugo-themes/)
- 📚 [View the **documentation**](https://wowchemy.com/docs/)
- 💬 [Chat with the **Wowchemy research community**](https://discord.gg/z8wNYzb) or [**Hugo community**](https://discourse.gohugo.io)
- 🐦 Twitter: [@wowchemy](https://twitter.com/wowchemy) [@GeorgeCushen](https://twitter.com/GeorgeCushen) [#MadeWithWowchemy](https://twitter.com/search?q=%23MadeWithWowchemy&src=typed_query)
- ⬇️ **Automatically import your publications from BibTeX** with the [Hugo Academic CLI](https://github.com/wowchemy/hugo-academic-cli)
- 💡 [Suggest an improvement](https://github.com/wowchemy/wowchemy-hugo-themes/issues)
- ⬆️ **Updating?** View the [Update Guide](https://wowchemy.com/docs/hugo-tutorials/update/) and [Release Notes](https://github.com/wowchemy/wowchemy-hugo-themes/releases)

## We ask you, humbly, to support this open source movement

Today we ask you to defend the open source independence of the Wowchemy website builder and themes 🐧

We're an open source movement that depends on your support to stay online and thriving, but 99.9% of our creators don't give; they simply look the other way.

### [❤️ Click here to become a GitHub Sponsor, unlocking awesome perks such as _exclusive academic templates and widgets_](https://github.com/sponsors/gcushen)

<p align="center"><a href="https://wowchemy.com/templates/" target="_blank" rel="noopener"><img src="https://wowchemy.com/uploads/readmes/academic_logo_200px.png" alt="Hugo Academic Theme for Wowchemy Website Builder"></a></p>

## Demo image credits

- [Open book](https://unsplash.com/photos/J4kK8b9Fgj8)
- [Course](https://unsplash.com/photos/JKUTrJ4vK00)

## Latest news

<!--START_SECTION:news-->
* [Easily make an academic CV website to get more cites and grow your audience 🚀](https:&#x2F;&#x2F;wowchemy.com&#x2F;blog&#x2F;easily-make-academic-website&#x2F;)
* [What&#39;s new in v5.2?](https:&#x2F;&#x2F;wowchemy.com&#x2F;blog&#x2F;whats-new-in-v5.2&#x2F;)
* [What&#39;s new in v5.1?](https:&#x2F;&#x2F;wowchemy.com&#x2F;blog&#x2F;whats-new-in-v5.1&#x2F;)
* [Version 5.0 (February 2021)](https:&#x2F;&#x2F;wowchemy.com&#x2F;blog&#x2F;version-5.0-february-2021&#x2F;)
* [Version 5.0 Beta 3 (February 2021)](https:&#x2F;&#x2F;wowchemy.com&#x2F;blog&#x2F;version-5.0-beta-3-february-2021&#x2F;)
<!--END_SECTION:news-->
