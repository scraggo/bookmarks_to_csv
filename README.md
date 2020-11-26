# bookmarks_to_csv

node CLI tool to create a CSV file from exported bookmarks html file from Chrome or Firefox.

CSV columns:

- `addDate`
- `href`
- `title`
- `category` - folder name

Caveats

- Firefox mobile links aren't included. They must be manually copied to another folder before exporting.

## Usage

`npm run build` to transpile the script.

Required arguments:

- `--input <path to bookmarks.html>`
- `--output <filename including .csv>`

### From package root

`node build/index <arguments>`

or `npm start -- <arguments>`

### From anywhere

coming soon

### Developing

`npm run start-dev` run once

`npm run start-watch` watch mode

## Credit

Started with [node-cli-scaffold](https://github.com/williscool/node-cli-scaffold)
