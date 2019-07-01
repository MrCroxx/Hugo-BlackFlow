# BlackFlow Hugo Theme

BlackFlow is a clear, responsive dark style theme with timeline and charts.

*This theme is referenced from [blackburn](<https://github.com/yoshiharuyamashita/blackburn>) by [yoshiharuyamashita](https://github.com/yoshiharuyamashita).*

![screenshot](https://raw.githubusercontent.com/mrcroxx/hugo-blackflow/master/images/screenshot.png)

## Demo

You can reach a live [Demo](<https://hugo-blackflow.github.io>) here which contains official documents from [Hugo](<https://gohugo.io/>) and some other documents about this theme.

## Features

- A clear chart for counting posts and words on index page.
- A clear sidebar with category links and social links.
- Timeline organized posts and categories lists.
- Automatic code highlighting supported by [highlight.js](https://highlightjs.org/).
- Latex language supported by [KaTeX](<https://katex.org/>).
- Charting supported by [ChartJS](<https://www.chartjs.org/>).
- Comment system supported by [Gitalk](<https://github.com/gitalk/gitalk>).
- ...

## Getting Started

1. Clone this repository to your hugo theme directory.

```bash
cd /path/to/your/hugo/site/
git submodule add https://github.com/mrcroxx/hugo-blackflow.git themes/blackflow
```

2. Switch your theme to *BlackFlow* in your *config.toml*.

```toml
theme = "blackflow"
```

3. Customize your site.

For more information read [Site Configuration](<#site-configuration>).

## Site Configuration<a name="site-configuration"></a>

Take a look in the `exampleSite` folder first.

### Length of the summary

When using a language other than English (like Chinese), make sure of adding the config below to make the length of summaries right.

```toml
summaryLength = 40
hasCJKLanguage = true
```

### Menu

Take a look at the `config.toml` file in the `exampleSite` folder.

The icon of menu items can be customized by parameter `pre` with [Font-Awesome](https://fontawesome.com/).

### Social Link

See `layouts/partials/social.html` for more information. 

### Site Parameters

```toml
[params]
    brand = "BlackFlow" # Showed at the top of the sidebar.
    subtitle = "A brief black style Hugo theme."
    dateformat = "2006-01-02 15:04"
    math = true # Turn KaTeX support on.
    max_taxonomy_terms = 3 # Limit posts showed below tags or topics.
    highlightjs = "androidstudio" # Customize the theme of highlightjs.
    highlightjs_extra_languages = ["yaml","kotlin"] # Add extra languages support.
    comment_system = "gitalk" # Turn Gitalk support on.
    comment_system_client_id = "xxx" 
    comment_system_client_secret = "xxx"
    comment_system_owner = "xxx"
    comment_system_repo = "xxx"
```

## Use ChartJS in Posts

The post page does not load `ChartJS` by default. You can turn it on by adding `"ChartJS"` to the `include` parameter of the markdown file.

```toml
+++
title = "xxx"
# ... ...
include = ["ChartJS"]
+++
```

## Content Suggestions

- Keep blog posts in `content/posts` directory.
- Use `tags` and `topics` as taxonomies.

## More Screenshots



