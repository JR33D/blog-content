# blog-content

External blog content repo for [jreed.me](https://jreed.me).

## Structure

```
index.json          <- post metadata array (title, date, tags, read, excerpt)
<slug>.mdx          <- post body with frontmatter
```

## Adding a post

1. Create `<slug>.mdx` with frontmatter matching the schema below
2. Prepend an entry to `index.json`
3. Push to main the site revalidates within 5 minutes, no redeploy needed

### Frontmatter schema

```yaml
---
title: Post Title
date: "YYYY-MM-DD"
tags: ["Tag"]
read: 5          # estimated read time in minutes
excerpt: One sentence summary shown in the post list.
---
```
