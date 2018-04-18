# A Qooxdoo Theme for OSparc

> These instructions assume that you are using the new [qooxdoo-comiler](https://github.com/qooxdoo/qooxdoo-compiler)
> for building your application.

## Using the Theme in your Application

To use the OSparc Theme in your application, go into the application root directory
and install the theme into your project:

```console
$ qx contrib update
$ qx contrib list
$ qx contrib install ITISFoundation/qx-osparc-theme
```

now you just have to modify your `Manifest.json` to enable the theme:

```json5
"applications": [
  {
    ...
    "theme": "osparc.theme.OSparcDark",
    ...
  }
],
```

## Running the Demo App

This contrib also comes with a demo application. To make it really simple to test
it comes with 'docker-batteries' included.

The setup is prepared for runnig with docker. You don't
need a local qooxdoo install or anyting to get started. Just install docker
and give this a whirl.

* build the docker image
  ```console
  $ docker-compose build
  ```

* run the demo server
   ```console
   $ docker-compose up
   ```

If you want to run a different qx command, you can do this too

```console
$ docker-compose run qx lint
```
