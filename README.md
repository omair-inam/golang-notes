# Website
This is a template repo for using [Docusaurus 2](https://docusaurus.io/) to generate a docs-only website.

### Installation

```
$ yarn
```

### Setup
* Search for all instances of `UpdateMe` in the codebase and replace with a suitable value for your project.

### Local Development

```
$ yarn start
```

This command starts a local development server and opens up a browser window. Most changes are reflected live without having to restart the server.

### Build

```
$ yarn build
```

This command generates static content into the `build` directory and can be served using any static contents hosting service.

### Deployment

Using SSH:

```
$ USE_SSH=true yarn deploy
```

Not using SSH:

```
$ GIT_USER=<Your GitHub username> yarn deploy
```

If you are using GitHub pages for hosting, this command is a convenient way to build the website and push to the `gh-pages` branch.
