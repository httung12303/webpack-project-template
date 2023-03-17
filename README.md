# Webpack Project Template
This project was created as a pain killer for setting up projects that use webpack. To apply this set up to your work, simply copy the dependencies in [here]() to your `package.json` and run 


```
npm install
```

If you followed [Webpack stater guide](https://webpack.js.org/guides/getting-started/), remember that they process images with Asset Modules which changes the name of the images in `dist`, meaning you cant do some thing like:

```Javascript
imgArray.forEach((img, index) => img.src = `img-${index}.png`);
```

In my setup, I instead use `copy-webpack-plugin` to retain the names.

I also included dependencies for using `eslint` with `Prettier`, so if you don't need them, make sure to remove them in `dependencies.json`. Also, I use this repos to save some resources like images and fonts that I see myself use repeatedly, they're not really important so I put them on the `others` branch.