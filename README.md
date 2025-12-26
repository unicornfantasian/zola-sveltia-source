# Zola Sveltia Source

![](https://raw.githubusercontent.com/unicornfantasian/zola-sveltia-source/refs/heads/main/Untitled%20Design_1-42.png)

Zola Sveltia Source is a Zola SSG project that uses Sveltia as its CMS and a ported version of the default Ghost CMS theme adapted for Zola & Sveltia.

## Requirements

You only need to download the Zola binary and configure the Sveltia CMS backend.  
You can deploy this project on Cloudflare Pages or Cloudflare Workers.

## Get Started

Run the following command for development:

`zola serve --extra-watch-path settings`

You can use Lightning CSS to minify, bundle, and target browsers (last 2 versions).

```json
{
  "devDependencies": {
    "lightningcss-cli": "^1.30.2"
  },
  "scripts": {
      "build": "lightningcss --minify --bundle --targets \">= 0.25%\" static/css/screen.css -o public/css/screen.css"
  }
}
```
`zola build && npm run build`

