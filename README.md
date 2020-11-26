# DefinitelyTyped-49749

Reproduction of issue [#49749](https://github.com/DefinitelyTyped/DefinitelyTyped/pull/49749).

## Usage

```sh
docker-compose up -d
yarn
yarn start
```

Structure in `node_modules/` should be:

```
node_modules/
├── @types/
|   ├── tapable/
|   └── webpack/
|       └── node_modules/
|           └── tapable/
└── tapable/
```

### Publish an update

1. Increase the `version` in `types/webpack/package.json`
2. Run `npm publish` in `types/webpack`
