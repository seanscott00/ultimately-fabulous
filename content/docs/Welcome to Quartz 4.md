---
title: Welcome to Quartz 4
---

Quartz is a fast, batteries-included static-site generator that transforms Markdown content into fully functional websites. Thousands of students, developers, and teachers are [[./Quartz Showcase|already using Quartz]] to publish personal notes, websites, and [digital gardens](https://jzhao.xyz/posts/networked-thought) to the web.

## 🪴 Get Started

Quartz requires **at least [Node](https://nodejs.org/) v20** and `npm` v9.3.1 to function correctly. Ensure you have this installed on your machine before continuing.

Then, in your terminal of choice, enter the following commands line by line:

```shell
git clone https://github.com/jackyzha0/quartz.git
cd quartz
npm i
npx quartz create
```

This will guide you through initializing your Quartz with content. Once you've done so, see how to:

1. [[./Authoring Content|Writing content]] in Quartz
2. [[./Configuration|Configure]] Quartz's behaviour
3. Change Quartz's [[./Layout|Layout]]
4. [[./Building your Quartz|Build and preview]] Quartz
5. Sync your changes with [[./Setting up your GitHub repository|GitHub]]
6. [[./Hosting|Host]] Quartz online

If you prefer instructions in a video format you can try following Nicole van der Hoeven's
[video guide on how to set up Quartz!](https://www.youtube.com/watch?v=6s6DT1yN4dw&t=227s)

## 🔧 Features

- [[./features/Obsidian Compatibility|Obsidian Compatibility]], [[./features/Full-text Search|Full-text Search]], [[./features/Graph View|Graph View]], note transclusion, [[./features/Wikilinks|Wikilinks]], [[./features/Backlinks|Backlinks]], [[./features/LaTeX|Latex]], [[./features/Syntax Highlighting|Syntax Highlighting]], [[./features/Popover Previews|Popover Previews]], [[./features/Docker Support|Docker Support]], [[./features/Internationalization|internationalization]], [[./features/Comments|Comments]] and [many more](./features) right out of the box
- Hot-reload for both configuration and content
- Simple JSX layouts and [[./advanced/Creating your own Quartz components|page components]]
- [[./features/SPA Routing|Ridiculously fast page loads]] and tiny bundle sizes
- Fully-customizable parsing, filtering, and page generation through [[./advanced/Making your own plugins|plugins]]

For a comprehensive list of features, visit the [features page](/features). You can read more about the _why_ behind these features on the [[./Philosophy of Quartz|Philosophy of Quartz]] page and a technical overview on the [[./advanced/Architecture|Architecture]] page.

### 🚧 Troubleshooting + Updating

Having trouble with Quartz? Try searching for your issue using the search feature. If you haven't already, [[./Upgrading Quartz|upgrade]] to the newest version of Quartz to see if this fixes your issue.

If you're still having trouble, feel free to [submit an issue](https://github.com/jackyzha0/quartz/issues) if you feel you found a bug or ask for help in our [Discord Community](https://discord.gg/cRFFHYye7t).
