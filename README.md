# GTSC Workspace

This repo contains all the other relevant repos as submodules.

The submodules will not be linked to one another and will have their own independent dependencies.

## Submodules

After you have cloned this repo you can checkout all the submodules using the following command:

```shell
git submodule update --init --recursive
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
