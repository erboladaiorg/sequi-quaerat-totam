**english** | [русский](https://github.com/erboladaiorg/sequi-quaerat-totam/blob/master/README.ru.md)
- - -

[![NPM version](https://img.shields.io/npm/v/@erboladaiorg/sequi-quaerat-totam.svg?style=flat)](https://www.npmjs.org/package/@erboladaiorg/sequi-quaerat-totam)

# yfm-docs

Yfm-docs lets you build a full-fledged documentation project: with navigation, internal transitions, and full
[Yandex Flavored Markdown (YFM)](https://diplodoc.com/docs/en/index-yfm) support.

![Example of displaying a documentation page](docsAssets/overview.jpg)

## Documentation

[ydocs.tech](https://diplodoc.com/docs/en/tools/docs)

## Usage

```bash
npm i @erboladaiorg/sequi-quaerat-totam -g
```

```bash
npm run start -- -i ./input-folder -o ./ouput-folder -v "{\"name\":\"Alice\"}"
```

## Source files

### Preparation

You need to add `.env` file into repo root with data below:

```bash
GITHUB_OWNER=
GITHUB_REPO= # docs
GITHUB_TOKEN= # personal access token
GITHUB_BASE_URL= # for ex: https://api.github.com
VCS_CONNECTOR_TYPE= # github
```

or you can update .yfm file into docs repo

```bash
connector:
    type:
    github:
        endpoint:
        token:
        owner:
        repo:
```

### Build from source

```bash
cd cli
npm ci && npm run build
```

## License

MIT
