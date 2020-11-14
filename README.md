# styled-jsx-plugin-dart-sass

[![Build Status](https://travis-ci.org/giuseppeg/styled-jsx-plugin-sass.svg?branch=master)](https://travis-ci.org/giuseppeg/styled-jsx-plugin-sass)
[![npm](https://img.shields.io/npm/v/styled-jsx-plugin-sass.svg)](https://www.npmjs.com/package/styled-jsx-plugin-sass)

Use [Sass](http://sass-lang.com/) with [styled-jsx](https://github.com/zeit/styled-jsx) 💥

## Usage

Install the package first.

```bash
npm install --save-dev styled-jsx-plugin-dart-sass
```

Install the `sass` version you need (it is a peer dependency).

```bash
npm install --save-dev sass
```

Next, add `styled-jsx-plugin-dart-sass` to the `styled-jsx`'s `plugins` in your babel configuration:

```json
{
  "plugins": [["styled-jsx/babel", { "plugins": ["styled-jsx-plugin-dart-sass"] }]]
}
```

## Node-sass options

Node-sass can be configured using `sassOptions`. This is useful for setting options such as `includePaths` or `precision`.

```json
{
  "plugins": [
    [
      "styled-jsx/babel",
      {
        "plugins": [
          [
            "styled-jsx-plugin-dart-sass",
            {
              "sassOptions": {
                "includePaths": ["./styles"]
              }
            }
          ]
        ]
      }
    ]
  ]
}
```

#### Notes

`styled-jsx-plugin-dart-sass` uses `styled-jsx`'s plugin system which is supported from version 2.

Read more on their repository for further info.

## License

MIT
