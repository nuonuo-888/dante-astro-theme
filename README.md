# Dante - Astro & Tailwind CSS Theme by justgoodui.com

Dante is a single-author blog and portfolio theme for Astro.js. Featuring a minimal, slick, responsive and content-focused design. For more Astro.js themes please check [justgoodui.com](https://justgoodui.com/).

![Dante Astro.js Theme](public/dante-preview.jpg)

## Deploy

[![Deploy to Tencent EdgeOne Pages](https://img.shields.io/badge/Deploy-Tencent%20EdgeOne%20Pages-006EFF?style=for-the-badge&logo=tencentqq&logoColor=white)](https://edgeone.ai/pages/new?template=https%3A%2F%2Fgithub.com%2Fnuonuo-888%2Fdante-astro-theme&output-directory=dist%2Fclient&build-command=npm+run+build&install-command=npm+install&origin_from=childtom)

The one-click button above clones `nuonuo-888/dante-astro-theme`, installs dependencies with `npm`, runs `npm run build`, and serves the generated `dist/client/` folder automatically on Tencent EdgeOne Pages.

## 👁 Preview

[![Preview](https://img.shields.io/badge/Preview-4ECCA3?style=for-the-badge&logo=globe&logoColor=white)](https://dante-astro-theme.edgeone.app/)

Visit the preview link above to see a live demo of this theme.

## Theme Features:

- ✅ Dark and light color mode
- ✅ Hero section with bio
- ✅ Portfolio collection
- ✅ Pagination support
- ✅ Post tags support
- ✅ Subscription form
- ✅ View transitions
- ✅ Tailwind CSS
- ✅ Mobile-first responsive layout
- ✅ SEO-friendly with canonical URLs and OpenGraph data
- ✅ Sitemap support
- ✅ RSS Feed support
- ✅ Markdown & MDX support
- ✅ Optimized images using Astro’s `Image` component

## Template Integrations

- @astrojs/tailwind - https://docs.astro.build/en/guides/integrations-guide/tailwind/
- @astrojs/sitemap - https://docs.astro.build/en/guides/integrations-guide/sitemap/
- @astrojs/mdx - https://docs.astro.build/en/guides/markdown-content/
- @astrojs/rss - https://docs.astro.build/en/guides/rss/

## ⚙️ Configuration Notes

### `site-config.ts`

All site-wide data and theme options are stored in `src/data/site-config.ts`. It provides a single configuration object used throughout the theme for navigation, branding, hero content, social links, and more.

You can update this file to customize:

- Site identity — title, description, avatar, subtitle, and default social share image
- Navigation — header and footer navigation links
- Social links — URLs for supported platforms
- Hero section — title, text, image, and action buttons
- Newsletter subscription — form settings suitable for Mailchimp, Formspree, ConvertKit, or other form-based providers. The form supports a custom action URL, configurable email and hidden fields, and an optional honeypot field for spam protection.
- Pagination — posts per page for blog and projects listings

Images can be referenced either as imports from `src/assets/` (for optimized Astro images) or as string paths from the `public/` directory.

### Images

The theme uses a `CustomImage` component that automatically displays images using Astro’s optimized `<Image />` or a standard `<img>` tag depending on the source.

- Content collection images (used in posts or pages) must be stored in `src/assets/` since they use Astro’s `image()` schema.
- Site-config images (like the avatar, hero image, or social preview) can either be imported from `src/assets/` for optimization or referenced directly from `public/` if you prefer not to optimize them.

## Project Structure

Inside of Dante Astro theme, you'll see the following folders and files:

```text
├── public/
├── src/
│   ├── assets/
│   ├── components/
│   ├── content/
│   ├── data/
│   ├── icons/
│   ├── layouts/
│   ├── pages/
│   ├── styles/
│   ├── utils/
│   ├── content.config.ts
│   └── types.ts
├── astro.config.mjs
├── package.json
├── README.md
└── tsconfig.json
```

Astro looks for `.astro` or `.md` files in the `src/pages/` directory. Each page is exposed as a route based on its file name.

There's nothing special about `src/components/`, but that's where we like to put any Astro (`.astro`) components.

The `src/content/` directory contains "collections" of related Markdown and MDX documents. Use `getCollection()` to retrieve posts from `src/content/blog/`, and type-check your frontmatter using an optional schema. See [Astro's Content Collections docs](https://docs.astro.build/en/guides/content-collections/) to learn more.

Any static assets, like images, can be placed in the `public/` directory.

## Astro.js Commands

All commands are run from the root of the project, from a terminal:

| Command                   | Action                                           |
| :------------------------ | :----------------------------------------------- |
| `npm install`             | Installs dependencies                            |
| `npm run dev`             | Starts local dev server at `localhost:4321`      |
| `npm run build`           | Build your production site to `./dist/`          |
| `npm run preview`         | Preview your build locally, before deploying     |
| `npm run astro ...`       | Run CLI commands like `astro add`, `astro check` |
| `npm run astro -- --help` | Get help using the Astro CLI                     |

## Want to learn more about Astro.js?

Check out [our documentation](https://docs.astro.build) or jump into our [Discord server](https://astro.build/chat).

## Credits

- Demo content generate with [Chat GPT](https://chat.openai.com/)
- Images for demo content from [Unsplash](https://unsplash.com/)

## Astro Themes by Just Good UI

- [Ovidius](https://github.com/JustGoodUI/ovidius-astro-theme) is a free single author blog theme.

## License

Licensed under the [GPL-3.0](https://github.com/JustGoodUI/dante-astro-theme/blob/main/LICENSE) license.
