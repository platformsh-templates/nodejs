> [!WARNING]
> **This repository is no longer maintained by our internal teams.**  
> The template is provided *as is* and will not receive updates, bug fixes, or new features.  
> You are welcome to contribute on it or fork the repository and modify it for your own use.
> To deploy this template on [Upsun](https://www.upsun.com), you can use the command [upsun project:convert](https://docs.upsun.com/administration/cli/reference.html#projectconvert)
> on this codebase to convert the existing `.platform.app.yaml` configuration file to the [Upsun Flex format](https://docs.upsun.com/create-apps/app-reference/single-runtime-image.html).

# Node.js for Platform.sh

This template builds a simple application using the Node.js built-in `http` web server. It includes a minimalist application skeleton that demonstrates how to connect to the included MariaDB server, but you are free to alter it as needed.

Node.js is an open-source JavaScript runtime built on Chrome's V8 JavaScript engine.

## Features

* Node.js 14
* MariaDB 10.4
* Automatic TLS certificates
* npm-based build

## Customizations

The following files and additions make the framework work.  If using this project as a reference for your own existing project, replicate the changes below to your project.

* The `.platform.app.yaml`, `.platform/services.yaml`, and `.platform/routes.yaml` files have been added.  These provide Platform.sh-specific configuration and are present in all projects on Platform.sh.  You may customize them as you see fit.
* An additional module, [`config-reader-nodejs`](https://github.com/platformsh/config-reader-nodejs), has been added.  It provides convenience wrappers for accessing the Platform.sh environment variables.

## References

* [Node.js http](https://nodejs.org/api/http.html#http_http)
* [Node.js on Platform.sh](https://docs.platform.sh/languages/nodejs.html)
