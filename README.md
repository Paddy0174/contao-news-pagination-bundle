# News Pagination

This bundle offers automatic content pagination for the news reader.

## Features

- add a pagination for navigating between the news parts
- automatic splitting
    - split news articles by an adjustable character amount respecting html tags

### Technical instructions

1. Activate "addPagination" in your news reader module and do the configuration there.
2. Add `<?= $this->newsPagination ?>` to your details template (e.g. "news_full").

### Known limitations for automatic pagination

- currently only ce_text not nested in another content element (like an accordion) is supported for splitting, other elements are removed properly according to current page number though (completely)