# sails generate new

Generate the files and directory structure for a new Sails app using webpack and vue.js.

## installation
```
npm install sails-generate-new-webpack-vue
```

Then edit or create a `.sailsrc` file in the current directory and add the following part to the JSON object to configure sails to use this module as the *new* generator.

```json
{
  "generators": {
    "modules": {
      "new": "sails-generate-new-webpack-vue"
    }
  }
}
```

Finally you can generate a new sails application as usual.
```sh
sails new sweet-app
```

The generator will install a standard sails backend, then download the [vuejs webpack template](https://github.com/vuejs-templates/webpack) and install it, prompting for features. The webpack project will be installed in `<project-directory>/webpack`. Then it will install a customized version of [sails-hook-webpack2](https://github.com/Tarrask/sails-hook-webpack2) to enable the webpack hot modules reloading directly from sails server.

## Usage
You can lift the sails server as usual:
```
sails lift
```

or for production:
```
NODE_ENV=production sails lift
```
