---
title: Create Blog Pages by R-Blogdown
author: gitgitWi
date: '2020-04-07'
slug: create-blog-pages-by-r-blogdown
categories:
  - R
  - Blogdown
tags:
  - blog
  - R Markdown
---

### Necessary Packages

- blogdown
- hugo

```{r}
install.packages("blogdown")
library(blogdown)

blogdown::install_hugo()
```

