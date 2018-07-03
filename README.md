# Poppy Station Website

Sources of the poppy-station website.

## [Hugo](https://gohugo.io)

Site is built with Hugo. Refer to [the documentation section](https://gohugo.io/getting-started/installing/#quick-install) to install it locally.

## Create new content

If you installed Hugo locally, you can use the `cli` tool to generate content:

```shell
hugo new articles/the-new-article.md
hugo new page/the-new-article.md
```

If not, copy the [archetypes/default.md](archetypes/default.md) file to the
desired location and rename it. The [content organization](https://gohugo.io/content-management/organization/)
from Hugo documentation might help.

## Publish

Site will be built and published for every push to this repository.
