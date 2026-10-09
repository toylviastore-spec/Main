# Shopify theme additions

## Curved banner (`snippets/tlv-curved-banner.liquid`)

A banner in the traced curved shape. It goes under the "Just dropped" and "Best sellers of October" banners, and its width, height and corner radius match theirs at desktop, tablet and mobile sizes.

**Install on the theme "lior's theme for toylvia":**

1. In Shopify admin, go to **Online Store → Themes → … → Edit code**.
2. Under **Snippets**, add a snippet named `tlv-curved-banner` and paste in the contents of `snippets/tlv-curved-banner.liquid`.
3. Open `layout/theme.liquid` and find the `#tlv-best-sellers-banner` div near the top of `<main id="MainContent">`. It ends with `alt="Best sellers of October"></div>`. Right after that closing `</div>`, add:

   ```liquid
   {% render 'tlv-curved-banner' %}
   ```

4. Save.

The title, text, button label and link are set at the top of the snippet. The link defaults to the `new-arrivals` collection.

`tlv-curved-banner-preview.png` shows the banner under stand-ins for the two existing banners at 1440px, 900px and 390px wide.
