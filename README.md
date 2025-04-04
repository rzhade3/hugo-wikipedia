# Hugo Wikipedia Theme

A Wikipedia-inspired theme for Hugo that mimics the look and feel of Wikipedia. This theme is perfect for knowledge bases, wikis, documentation sites, and any content-heavy website.

## Features

- Wikipedia-like design and layout
- Responsive design for mobile and desktop
- Table of contents for long articles
- Category system similar to Wikipedia
- Citation and references support
- Infobox shortcode for Wikipedia-style info boxes
- Sidebar navigation

## Installation

1. In your Hugo site directory, run:
   ```
   git submodule add https://github.com/rzhade3/hugo-wikipedia themes/hugo-wikipedia
   ```

2. Update your site's configuration file (`config.toml`) to use the theme:
   ```
   theme = "hugo-wikipedia"
   ```

## Configuration

Example configuration in `config.toml`:

```toml
baseURL = "https://example.org/"
languageCode = "en-us"
title = "My Wiki"
theme = "hugo-wikipedia"

[params]
  description = "A knowledge base built with Hugo and the Wikipedia theme"
  favicon = "favicon.ico"
  license = "Creative Commons Attribution-ShareAlike License"
  license_url = "https://creativecommons.org/licenses/by-sa/4.0/"
  # logo = "images/logo.png"  # Uncomment to use a custom logo
  github = "https://github.com/rzhade3/your-wiki"  # Link to your GitHub repo

[menu]
  [[menu.main]]
    name = "Getting Started"
    url = "/getting-started/"
    weight = 1
  [[menu.main]]
    name = "Documentation"
    url = "/docs/"
    weight = 2
  [[menu.main]]
    name = "About"
    url = "/about/"
    weight = 3
```

## Shortcodes

### Infobox

```
{{< infobox title="Title Here" >}}
Content of the infobox goes here.
{{< /infobox >}}
```

### Citation Reference

```
{{< ref "1" >}}
```

## License

This theme is released under the MIT license.
