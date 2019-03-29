# hugo-loremipsum

<!-- [![Awesome](https://awesome.re/badge.svg)](https://github.com/budparr/awesome-hugo) -->

## About

This is not a standalone theme. It is a [Hugo](https://gohugo.io) theme component providing a shortcode: `loremipsum` to generate greek text paragraphs.

It starts off with a standard "Lorem ipsum …" text, then randomises the sentence order on each subsequent paragraph.

## Usage

1. Add the `hugo-loremipsum` as a submodule to be able to get upstream changes later `git submodule add https://github.com/martignoni/hugo-loremipsum.git themes/hugo-loremipsum`
2. Add `hugo-loremipsum` as the left-most element of the `theme` list variable in your site's or theme's configuration file `config.yaml` or `config.toml`. Example, with `config.yaml`:
    ```yaml
    theme: ["hugo-loremipsum", "my-theme"]
    ```
    or, with `config.toml`,
    ```toml
    theme = ["hugo-loremipsum", "my-theme"]
    ```
3. In your site, use the shortcode, e.g. to generate 3 paragraphs of Lorem ipsum greek text :
    ```go
    {{< loremipsum 3 >}}
    ```
    or simply, for just one paragraph
    ```go
    {{< loremipsum >}}
    ```

### Credits

Copyright © 2019 onwards, Nicolas Martignoni nicolas@martignoni.net.

This theme component was possible because of the code published by Chris Allmark in [this Hugo forum post](https://discourse.gohugo.io/t/lorem-ipsum-shortcode-for-hugo/15604/5), with his friendly permission.
