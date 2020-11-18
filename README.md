# shortcodes

Rich text editor short codes that work with the We Are Underground Shopify themes. Based off of the Advanced Rich Text Editing formatting for the [Mr. Parker](https://support.weareunderground.com/article/269-20-mr-parker-theme-advanced-rich-text-editor-formatting) and [Vantage](https://support.weareunderground.com/article/246-20-vantage-theme-advanced-rich-text-editor-formatting) themes. Inspired by the [Shopify Shortcodes](https://github.com/culturekings/shopify-shortcodes).

## Installation

### Activating shortcodes

Go to the Shopify Admin > Themes > Actions drop down > Edit Code.

Add the [`shortcode.liquid`](https://raw.githubusercontent.com/culturekings/shopify-shortcodes/master/shortcode.liquid) and [`shortcode-render.liquid`](https://raw.githubusercontent.com/culturekings/shopify-shortcodes/master/shortcode-render.liquid) to the __Snippets__ folder.

Open the `page-templates.liquid` file in the __Sections__ folder.

Change `{{ page.content }}` to `{% include 'shortcode' load: page.content %}` and click Save.

### Add the modules 

Add the following to the __Snippets__ folder:

- [`shortcode-button.liquid`](./shortcode-button.liquid)
- [`shortcode-row.liquid`](./shortcode-row.liquid)
- [`shortcode-column.liquid`](./shortcode-column.liquid)

Open the __Assets__ folder find the `stylesheet.css.liquid` file and add the [`styles.css`](./styles.css) to the bottom of the file.
