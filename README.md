Demonstration of how to use [wordpress-shortcode-webpack-plugin](https://github.com/studio-lagier/wordpress-shortcode-webpack-plugin) with [Create React App](https://reactjs.org/docs/create-a-new-react-app.html), using [react-app-rewired](https://github.com/timarney/react-app-rewired/) to extend the CRA webpack config.

How I got here:

1. `npx create-react-app my-plugin`
2. `cd my-plugin`
3. `yarn add -D react-app-rewired wordpress-shortcode-webpack-plugin`
4. Created `config-overrides.js` adding the webpack plugin.
5. Updated `package.json` to use `react-app-rewired` instead of `react-scripts`.
6. (Bonus) Updated base URL to be correctly pathed for Wordpress by setting `"homepage": "/wp-content/plugins/my-plugin/assets/"` in `package.json`.
7. Run `yarn build`. Done!
