# TWIN Workspace

This repo contains all the other relevant repos as submodules.

To clone the repo and all it's submodules use the following command:

```shell
git clone --recursive https://github.com/twinfoundation/workspace.git
```

It should be noted the submodules will not be linked to one another, and will all have their own independent dependencies.

## Submodules

You have update all the submodules using the following command:

```shell
git submodule update --recursive
```

If you want to pull all the latest changes for the submodules use the following command:

```shell
git pull --recurse-submodules
```

To add a new module to the repository use the following command:

```shell
git submodule add https://github.com/twinfoundation/<name>.git
```

## Cross module commands

The following commands are available across all the modules.

### Install

You can run the following command to perform an npm install across all the submodules:

```shell
npm run submodule:install
```

### Dist

You can run the following command to perform the full distribution build across all the submodules:

```shell
npm run submodule:dist
```

### Build

You can run the following command to perform just a TypeScript compile across all the submodules:

```shell
npm run submodule:build
```

### Bundle

You can run the following command to perform just an ESM bundle compile across all the submodules:

```shell
npm run submodule:bundle-esm
```
