# sails generate new

Generate the files and directory structure for a new Sails app using webpack and vue.js.

Edit or create a `.sailsrc` file in the current directory.

Add this to the JSON object

```json
{
  "generators": {
    "modules": {
      "new": "sails-generate-new-webpack-vue"
    }
  }
}

```

```sh
sails new sweet-app
```
