# Gastby Starter Ghost

A starter template to build lightning fast websites with [Ghost](https://ghost.org) & [Gatsby](https://gatsbyjs.org)

**Demo:** https://gatsby.ghost.org

&nbsp;

![gatsby-starter-ghost](https://user-images.githubusercontent.com/120485/50913567-8ab8e380-142c-11e9-9e78-de02ded12fc6.jpg)

&nbsp;


# Installing

```bash
# With Gatsby CLI
gatsby new gatsby-starter-ghost https://github.com/TryGhost/gatsby-starter-ghost.git
```

```bash
# From Source
git clone git@github.com:TryGhost/gatsby-starter-ghost.git
cd gatsby-starter-ghost
```

Then install dependencies

```bash
yarn
```

&nbsp;

# Running

Start the development server. You now have a Gatsby site pulling content from headless Ghost.

```bash
gatsby develop
```

By default, the starter will populate content from a default Ghost install located at https://gatsby.ghost.io.

To use your own install, edit the `.ghost.json` config file with your credentials. You can find or your `contentApiKey` in the "Integrations" screen in Ghost Admin.

&nbsp;

# Deploying with Netlify

The starter contains three config files specifically for deploying with Netlify. A `netlify.toml` file for build settings, a `/static/_headers` file with default security headers set for all routes, and `/static/_redirects` to set Netlify custom domain redirects.

To deploy to your Netlify account, hit the button below.

[![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/)

Content API Keys are generally not considered to be sensitive information, they exist so that they can be changed in the event of abuse so most people commit it directly to their `ghost.json` config file. If you prefer to keep this information out of your repository you can remove this config and set [Netlify ENV variables](https://www.netlify.com/docs/continuous-deployment/#build-environment-variables) for production builds instead.

Once deployed, you can set up a [Ghost + Netlify Integration](https://docs.ghost.org/integrations/netlify/) to use deploy hooks from Ghost to trigger Netlify rebuilds. That way, any time data changes in Ghost, your site will rebuild on Netlify.

&nbsp;

# Optimising

You can disable the default Ghost Handlebars Theme front-end by enabling the `Make this site private` flag within your Ghost settings. This enables password protection in front of the Ghost install and sets `<meta name="robots" content="noindex" />` so your Gatsby front-end becomes the source of truth for SEO.

&nbsp;

# Extra options

```bash
# Run a production build, locally
gatsby build

# Serve a production build, locally
gatsby serve
```

Gatsby `develop` uses the `dev` config in `ghost.json` - while Gatsby `serve` uses the `production` config.

&nbsp;

# Copyright & License

Copyright (c) 2013-2019 Ghost Foundation - Released under the [MIT license](LICENSE).
# gatsby-ghost-blog-demo
