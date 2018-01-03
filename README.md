# matuzo.at

## Development

Watch file changes and generate HTML:

`eleventy --watch`

## Update Content

Get fresh content from Contentful by running:

`npm run content`

## Export content

Create a file in `./content` and name it `[CONTENT_TYPE].json`

```
{
  "space-id": "[SPACE ID]",
  "management-token": "[PRIVATE ACCESS TOKEN]]",
  "skip-content-model": true,
  "content-only": true,
  "content-file": "views/_data/[CONTENT_TYPE].json",
  "query-entries": [
    "content_type=[CONTENT_TYPE ID]]"
  ]
}
```