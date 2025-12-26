# Tech Blog Hub - Hugo Site

A beautiful Hugo site that showcases links to top tech companies' engineering blogs and includes an embedded YouTube tutorial on how to use Hugo.

![Site Preview](https://github.com/user-attachments/assets/f10953f0-5679-4ad7-9b41-2b3a6772014b)

## Features

✨ **Beautiful Design**: Modern, responsive design with gradient backgrounds and smooth animations  
🚀 **Top Tech Blogs**: Links to 12 leading tech companies' engineering blogs:
- Google Engineering
- Meta Engineering  
- Netflix Tech Blog
- Airbnb Engineering
- Uber Engineering
- Amazon AWS Blog
- Microsoft Developer
- LinkedIn Engineering
- Spotify Engineering
- GitHub Blog
- Twitter Engineering
- Stripe Engineering

🎥 **Hugo Tutorial**: Embedded YouTube video tutorial on how to use Hugo

## Prerequisites

- Hugo (v0.121.0 or higher)

## Installation

1. Clone this repository:
```bash
git clone https://github.com/priyanshu1998/hello-hugo.git
cd hello-hugo
```

2. Install Hugo (if not already installed):
```bash
wget https://github.com/gohugoio/hugo/releases/download/v0.121.0/hugo_0.121.0_Linux-64bit.tar.gz
tar -xzf hugo_0.121.0_Linux-64bit.tar.gz
sudo mv hugo /usr/local/bin/
```

## Usage

### Build the site
```bash
hugo
```

The built site will be in the `public/` directory.

### Run development server
```bash
hugo server -D
```

Then open your browser and navigate to `http://localhost:1313/hello-hugo/`

### Build for production
```bash
hugo --minify
```

## Project Structure

```
.
├── archetypes/          # Content templates
├── content/             # Site content
│   └── _index.md       # Homepage content with YouTube embed
├── layouts/             # HTML templates
│   ├── index.html      # Homepage layout
│   └── shortcodes/     # Custom shortcodes
│       └── youtube.html # YouTube embed shortcode
├── hugo.toml            # Site configuration
└── README.md            # This file
```

## Customization

### Change the site title
Edit `hugo.toml` and modify the `title` parameter.

### Change the YouTube video
Edit `content/_index.md` and replace the video ID in the YouTube shortcode:
```markdown
{{< youtube "VIDEO_ID_HERE" >}}
```

### Add more tech blogs
Edit `layouts/index.html` and add new blog cards in the `.blog-grid` section.

## Deployment

This site can be deployed to:
- GitHub Pages
- Netlify
- Vercel
- Any static hosting service

For GitHub Pages, push the `public/` directory to the `gh-pages` branch.

## Built With

- [Hugo](https://gohugo.io/) - The world's fastest framework for building websites
