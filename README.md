hello world from lah.
gatsby starter built in `gatsby + typescript + mdx`

# 💨 Quick start

Use the Gatsby CLI (install instructions) to create a new site, specifying the default starter.

1. Create a Gatsby site

```
npx gatsby new your-blog-name https://github.com/leahincom/gatsby-starter-lah
```

Instead of using npx, use the Gatsby CLI (install instructions) to create a new site, specifying the default starter.

```
npm install -g gatsby-cli
gatsby new your-blog-name https://github.com/leahincom/gatsby-starter-lah
```

2. Start developing

before you go, you should setup `.env`. This is provided in `.env.example`.

```
// required
GITHUB_PERSONAL_ACCESS_TOKEN=""

// preferred
GTM_CONTAINER_ID=""
MONGODB_REPLICA_SET=""
MONGODB_ADDRESS=""
MONGODB_USERNAME=""
MONGODB_PASSWORD=""
MONGODB_NAME=""
MONGODB_COLLECTION_NAME=""
```

```
cd your-blog-name/
yarn develop // gatsby develop
```

There you go!
Open localhost:8000 and ya'll see something's going on.

3. Add your posts 🌈

No more hard works for simple posts!
Write your posts in md, mdx by putting the content inside `/posts` folder.

Your own category can be made in enum in `gatsby-node.ts`.

4. 🚀 Quick start (Gatsby Cloud)

Deploy this starter with one click on Gatsby Cloud:
[<img src="https://www.gatsbyjs.com/deploynow.svg" alt="Deploy to Gatsby Cloud">](https://www.gatsbyjs.com/dashboard/deploynow?url=https://github.com/gatsbyjs/gatsby-starter-default)

or whatever you like :)

# 💝 Customize

### Gatsby config

/
├── gatsby-browser.ts // css, wrapPageElement, ...
├── wrapPageElement.tsx
├── gatsby-ssr.tsx // same as gatsby-browser.ts with more ssr settings for stitches
├── gatsby-config.ts // default config, plugins, ...
└── gatsby-node.ts // create types and configure page props for mdx settings

### Structure

src
├── assets
├── components // individual components needed for default page styling
├── hooks
├── layouts // default layout used in pages
├── pages // routing for basic pages except for posts (which are served from `/posts`)
├── styles
│ ├── global.ts // global style with stitches
│ ├── text.ts // custom text styles
│ ├── normlize.css
│ └── stitches.config.ts // custom media setting
├── templates // used for posts styling
├── types
├── utils
└── constants.ts
