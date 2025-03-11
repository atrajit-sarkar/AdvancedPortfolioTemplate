# Professional Portfolio Website Template

A modern, responsive portfolio website template that can be easily customized through text files and supports blog posts in PDF format. Perfect for hosting on GitHub Pages!

## Features

- 🎨 Modern and clean design
- 📱 Fully responsive layout
- 🌓 Dark/Light theme switcher
- ⚡ Fast loading and smooth animations
- 📝 Easy content management through text files
- 📚 Blog post system with PDF support
- 🔗 Social media integration
- 🎯 SEO friendly

## Getting Started

1. Clone or download this repository
2. Replace the content in the `data` folder with your personal information:
   - `hero.txt`: Your name and title (one per line)
   - `about.txt`: Your personal description
   - `skills.txt`: Your skills and expertise
   - `contact.txt`: Your contact information
   - `social.txt`: Your social media links (format: `platform|url`)
   - `footer.txt`: Your footer text

3. Add your profile picture:
   - Place your profile picture in the `data` folder
   - Name it `profile.jpg`

4. Set up your blog posts:
   - Place your PDF blog posts in the `blogs` folder
   - Update `blogs/index.html` with your blog post information:
   ```html
   {
       "title": "Your Blog Title",
       "file": "your-blog-file.pdf",
       "date": "March 15, 2024"
   }
   ```
   - Make sure the "file" field matches your PDF filename exactly
   - Add multiple blog entries following the same format

5. Deploy to GitHub Pages:
   - Create a new repository on GitHub
   - Push your code to the repository
   - Go to repository Settings > Pages
   - Under "Source", select "Deploy from a branch"
   - Select "main" branch and "/ (root)" folder
   - Click Save
   - Your site will be available at `https://yourusername.github.io/repository-name`

## File Structure
```
portfolio/
├── index.html          # Main HTML file
├── css/
│   └── style.css      # Stylesheet with modern design
├── js/
│   └── main.js        # JavaScript for dynamic content
├── data/              # Content management folder
│   ├── hero.txt       # Name and title
│   ├── about.txt      # Personal description
│   ├── skills.txt     # Skills and expertise
│   ├── contact.txt    # Contact information
│   ├── social.txt     # Social media links
│   ├── footer.txt     # Footer text
│   └── profile.jpg    # Your profile picture
└── blogs/             # Blog posts folder
    ├── index.html     # Blog posts listing
    └── *.pdf          # Your blog post PDFs
```

## Customization

### Content Files Format

1. `hero.txt`:
```
Your Name
Your Title/Role
```

2. `social.txt`:
```
github|https://github.com/yourusername
linkedin|https://linkedin.com/in/yourusername
twitter|https://twitter.com/yourusername
```

3. `blogs/index.html`:
```html
<div id="blog-list" style="display: none;">
    [
        {
            "title": "Your Blog Title",
            "file": "your-blog-file.pdf",
            "date": "March 15, 2024"
        }
    ]
</div>
```

### Colors
You can customize the website's color scheme by modifying the CSS variables in `css/style.css`:

```css
:root {
    --primary-color: #2563eb;
    --secondary-color: #1e40af;
    --text-color: #1f2937;
    --background: #ffffff;
    /* ... other color variables ... */
}
```

### Supported Social Media Platforms
- GitHub
- LinkedIn
- Twitter
- Instagram
- Facebook
- YouTube
- TikTok
- Twitch
- Discord
- Telegram
- Reddit
- Pinterest
- Snapchat
- WhatsApp
- Spotify
- Apple
- Google
- Microsoft
- Amazon

Add more platforms by updating the `getSocialIcon` function in `main.js`.

## Troubleshooting

1. **Blog posts not showing up:**
   - Make sure your PDFs are properly placed in the `blogs` folder
   - Verify that `blogs/index.html` is correctly formatted
   - Check that PDF filenames match exactly with what's listed in `index.html`

2. **Profile picture not loading:**
   - Ensure your image is named `profile.jpg`
   - Place it in the `data` folder
   - Try using a smaller image size if it loads slowly

3. **Social media icons not showing:**
   - Check that the platform name in `social.txt` matches the supported platforms
   - Verify the URL format is correct
   - Make sure there's no extra whitespace in the file

## Contributing

Feel free to submit issues and enhancement requests!

## License

This project is licensed under the MIT License - see the LICENSE file for details. 