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

`node build <arguments>`

or `npm start -- <arguments>`

### From anywhere

```sh
alias bkcsv="node ~/bookmarks_to_csv/build";

bkcsv -i ~/Desktop/bookmarks210116.html -o bookmarks210116.csv
```

### Developing

`npm run start-dev` run once

`npm run start-watch` watch mode

## Credit

Started with [node-cli-scaffold](https://github.com/williscool/node-cli-scaffold)
