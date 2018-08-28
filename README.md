# AngularJS Migration Guide
A (style) guide to migrating from AngularJS to Angular.

This is an **_opinionated_** guide for of a few of the things I have learned on the path to migrating an AngularJS codebase to Angular. Pull Requests are welcome.

There are some core concepts and technologies that you will want to be sure you want to incorporate when following this guide.
- TypeScript - this really isn't optional. Angular is built in TypeScript. Yes its possible to do a lot of things without it, but it's **far** more difficult and you won't find documentation. Besides, you can make TypeScript pretty lax in a lot of cases.
- ES2015/ESNext - Use modern JavaScript/ECMAScript features. You have them available, so why not?
- Babel - You will be migrating your code iteratively from `.js` to `.ts` files. If you still want to use modern features (as described above) and you still need to support legacy browsers (like IE11 🤮 ) You will want Babel.
- Webpack - Webpack is the glue that ties this all together. You *will* want a bundler. Angular is designed to work well with Webpack. (the angular CLI `ng` uses Webpack under the hood)

If these sound alright with you, then great! This guide might be right for you. 😄