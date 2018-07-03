# Poppy Station Website

Sources of the poppy-station website.

## Dependencies

Site is built with [Hugo](https://gohugo.io). Refer to [the documentation section](https://gohugo.io/getting-started/installing/#quick-install) to install it locally.

Layout is done using [Bootstrap v4.1](https://getbootstrap.com/docs/4.1/getting-started/introduction/).

## Create new content

If you installed Hugo locally, you can use the `cli` tool to generate content:

```shell
hugo new articles/the-new-article.md
hugo new page/the-new-article.md
```

If not, copy the [archetypes/default.md](archetypes/default.md) file to the
desired location and rename it. The [content organization](https://gohugo.io/content-management/organization/)
from Hugo documentation might help.

Content should be written in markdown format, but writing HTML is also allowed
by Hugo.

### Shortcodes

Some shortcodes [are provided by Hugo](https://gohugo.io/content-management/shortcodes/#use-hugo-s-built-in-shortcodes),
and few were added for formatting purpose.

#### Figure

`fig` shortcode requires `src` and `title` parameters.

Example:

```markdown
{{< fig src="https://team.inria.fr/potioc/files/2017/08/teegi.jpg" title="Teegi Robot" >}}
```

#### Blockquote

`blockquote` shortcode accepts `source` parameter.

Basic form:

```markdown
{{< blockquote >}}
Give a man a fish and you feed him for a day; teach a man to fish and you feed him for a lifetime.
{{</ blockquote >}}
```

With source footer:

```markdown
{{< blockquote source="Extract of wikipedia.fr" >}}
Exercitation aliqua enim enim adipisicing. Nulla eu do cillum laborum velit culpa nisi consequat excepteur. Aliqua adipisicing esse adipisicing adipisicing cillum deserunt qui consequat nulla deserunt do do occaecat aute. Proident consectetur officia dolore in et sint.
{{</ blockquote >}}
```

#### Embed YouTube video

`embed-yt` requires `src` and `ratio` parameter

Example:

```markdown
{{< embed-yt src="aZxuy9rWrmA" ratio="16:9" >}}
```

## Publish

Site will be built and published for every push to this repository.
