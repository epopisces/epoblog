# epoblog

So this is/was an attempt to get markdown+mermaid working in an online blog, as hosted (initially) by GitHub pages.  

As I did my research, it became fairly clear that as of 2022.03 you can have one of the two, but not both:
* Vue 3 blog supporting markdown
* Vue 2 blog supporting markdown + mermaid

I struggle-bused for a bit with Vue 3, and have a working markdown blog, but couldn't get the mermaid part working; the tooling available didn't support mermaid out of the box([vue3-markdown-it](https://github.com/JanGuillermo/vue3-markdown-it), [vuepress](https://www.npmjs.com/package/vuepress-plugin-mermaidjs)) or wasn't ported to Vue3 yet (vue-markdown-it, [gridsome](https://github.com/gridsome), [vuepress-next](https://github.com/vuepress/vuepress-next)).

But also I realized in the course of this research: I don't want to design a blog site from the ground up (at least not at this point, maybe in the future).  So I am going to fall back on Vue 2 with a full-blown framework for blogging.  I'm going to try [gridsome](https://github.com/gridsome), inspired by posts like these:
* [Building a blog with vue and markdown using gridsome](https://www.telerik.com/blogs/building-a-blog-with-vue-and-markdown-using-gridsome)

It is my great hope that gridsome isn't a dead project and will be upgraded to Vue 3.  We shall see!

## Project setup
```
npm install
```

### Compiles and hot-reloads for development
```
npm run serve
```

### Compiles and minifies for production
```
npm run build
```

### Lints and fixes files
```
npm run lint
```

### Project deploy to Github Pages
```
npm run deploy
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).
