R Markdown(2) flexdashboard
================
2020-04-08

true

## flexdashboard package

#### introduction

  - dashboard 작성 및 customization은 RMarkdown에 기반해 이뤄짐
  - shiny component들도 덧붙일수 있음

#### install and import the package

`install.packages("flexdashboard") \ library(flexdashboard)`

#### create new flexdashboard

`new R Markdown` -\> `from templates` -\> `flex dashboard`

#### YAML front matter

    ---
    title: "flexdashboard test"
    output:
      flexdashboard::flex_dashboard:
        orientation: columns
        vertical_layout: fill
    ---

  - `orientation: columns` : total layout == columns
      - options : `columns`, `rows`
  - `vertical_layout : fill` : CSS의 media query 방식
      - options : `fill`, `scroll`

#### `Column`

    Column {data-width=650 .tabset}
    -----------------------------------------------------------------------
    ### Chart A
    
    ### Chart B

  - column part with Chart A
  - `data-width=650` : width by pixel
  - `.tabset` : tabset layout, where columns \> 2
      - `.tabset-fade` : fade effect

### `dygraph` 추가

  - flexdashboard에는 Javascript 추가 가능
