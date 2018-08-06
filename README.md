# sapper-template

The default [Sapper](https://github.com/sveltejs/sapper) template. To clone it and get started:

```bash
npx degit sveltejs/sapper-template my-app
cd my-app
npm install # or yarn!
npm run dev
```

Open up [localhost:3000](http://localhost:3000) and start clicking around.

## Reproduce bug

Seen in Chrome 67.0.3396.99, Firefox 61.0.1 & Safari 11.1.2 (12605.3.8.1)

> Navigation to an anchor link from another page doesn't work, and only takes you to the top of the page. However, navigation to an anchor link does work if you are already on the page.

1. I've set "home" in the top nav to link to /#link-183  Click on about. Then click back to home
1. You will see that it takes you to home, but to the top of the page and not to the anchored section of the page
1. Copy the url in the browser bar.
1. Paste the url and hit <kbd>return</kbd>. In Chrome, the link will now jump to the correct part of the page.
1. Now click on another anchor link, say 232
1. Scroll to the top of the page and hit "home." Now you should get taken to #link-183

![](screenshot.gif)
