# SEO & tracking

## What the theme does automatically

- **Titles, descriptions and canonical URLs** use Shopify's native SEO fields
  (Online Store → Preferences, and the SEO section on each product / collection
  / page / article). The theme does not add its own competing title logic.
- **Structured data (JSON-LD)** for Organization, WebSite + SearchAction,
  WebPage, BreadcrumbList, Product with Offer, ItemList for collections,
  BlogPosting for articles, and Brand.
- **Open Graph and Twitter Card** tags, using the page's own image or the
  **Default social sharing image** from Theme settings.
- Shopify supplies `sitemap.xml`, `robots.txt`, and hreflang tags for
  multi-language stores.
- Responsive images with width/height, lazy loading below the fold, eager +
  high priority for the LCP image, and `decoding="async"`.

## Domain verification

**Theme settings → SEO and tracking** has token fields for:

- Google (Search Console)
- Microsoft Bing
- Pinterest
- Meta (Facebook) domain verification

Paste the token; the theme renders the correct `<meta>` tag.

## Google tag

**Theme settings → SEO and tracking → Google tag ID** adds an optional
storefront page-view tag. It:

- waits for the visitor's Shopify analytics consent,
- is disabled inside the theme editor,
- should be left blank if Google Analytics is already installed by the
  Google & YouTube app, Customer Events, or another app, to avoid duplicate
  data.

For checkout and conversion events (`checkout_completed` etc.), use Shopify
**custom pixels** or an app. Themes cannot script checkout.

## Custom storefront code

**Enable custom storefront code** unlocks two slots: before `</head>` and
before `</body>`. These are storefront-only (never checkout, never the
editor), intended for a single trusted provider. Incorrect code here can
affect performance or compatibility, so treat it as advanced.
