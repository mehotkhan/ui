---
description: A list of buttons or links to navigate through pages.
links:
  - label: Pagination
    icon: i-custom-radix-vue
    to: https://www.radix-vue.com/components/pagination.html
  - label: GitHub
    icon: i-simple-icons-github
    to: https://github.com/nuxt/ui/tree/v3/src/runtime/components/Pagination.vue
---

## Usage

Use the `default-page` prop or the `v-model:page` directive to control the current page.

::note
The Pagination component uses some [Button](/components/button) to display the pages, use [`color`](#color), [`variant`](#variant) and [`size`](#size) props to style them.
::

### Total

Use the `total` prop to set the total number of items in the list.

::component-code
---
external:
  - page
model:
  - page
props:
  page: 5
  total: 100
---
::

### Items Per Page

Use the `items-per-page` prop to set the number of items per page. Defaults to `10`.

::component-code
---
ignore:
  - page
external:
  - page
model:
  - page
props:
  page: 5
  itemsPerPage: 20
  total: 100
---
::

### Sibling Count

Use the `sibling-count` prop to set the number of siblings to show. Defaults to `2`.

::component-code
---
ignore:
  - page
  - total
external:
  - page
model:
  - page
props:
  page: 5
  siblingCount: 1
  total: 100
---
::

### Show Edges

Use the `show-edges` prop to always show the ellipsis, first and last pages. Defaults to `false`.

::component-code
---
ignore:
  - page
  - total
external:
  - page
model:
  - page
props:
  page: 5
  showEdges: true
  siblingCount: 1
  total: 100
---
::

### Show Controls

Use the `show-controls` prop to show the first, prev, next and last buttons. Defaults to `true`.

::component-code
---
ignore:
  - page
  - total
external:
  - page
model:
  - page
props:
  page: 5
  showControls: false
  showEdges: true
  total: 100
---
::

### Color

Use the `color` prop to set the color of the inactive controls. Defaults to `gray`.

::component-code
---
ignore:
  - page
  - total
external:
  - page
model:
  - page
items:
  color:
    - primary
    - green
    - red
    - orange
    - amber
    - yellow
    - lime
    - emerald
    - teal
    - cyan
    - sky
    - blue
    - indigo
    - violet
    - purple
    - fuchsia
    - pink
    - rose
    - gray
props:
  page: 5
  color: primary
  total: 100
---
::

### Variant

Use the `variant` prop to set the variant of the inactive controls. Defaults to `outline`.

::component-code
---
ignore:
  - page
  - total
external:
  - page
model:
  - page
items:
  color:
    - primary
    - green
    - red
    - orange
    - amber
    - yellow
    - lime
    - emerald
    - teal
    - cyan
    - sky
    - blue
    - indigo
    - violet
    - purple
    - fuchsia
    - pink
    - rose
    - gray
  variant:
    - solid
    - outline
    - soft
    - subtle
    - ghost
    - link
props:
  page: 5
  color: gray
  variant: subtle
  total: 100
---
::

### Active Color

Use the `active-color` prop to set the color of the active control. Defaults to `primary`.

::component-code
---
ignore:
  - page
  - total
external:
  - page
model:
  - page
items:
  activeColor:
    - primary
    - green
    - red
    - orange
    - amber
    - yellow
    - lime
    - emerald
    - teal
    - cyan
    - sky
    - blue
    - indigo
    - violet
    - purple
    - fuchsia
    - pink
    - rose
    - gray
props:
  page: 5
  activeColor: gray
  total: 100
---
::

### Active Variant

Use the `active-variant` prop to set the variant of the active control. Defaults to `solid`.

::component-code
---
ignore:
  - page
  - total
external:
  - page
model:
  - page
items:
  activeColor:
    - primary
    - green
    - red
    - orange
    - amber
    - yellow
    - lime
    - emerald
    - teal
    - cyan
    - sky
    - blue
    - indigo
    - violet
    - purple
    - fuchsia
    - pink
    - rose
    - gray
  activeVariant:
    - solid
    - outline
    - soft
    - subtle
    - ghost
    - link
props:
  page: 5
  activeColor: primary
  activeVariant: subtle
  total: 100
---
::

### Size

Use the `size` prop to set the size of the controls. Defaults to `md`.

::component-code
---
ignore:
  - page
  - total
external:
  - page
model:
  - page
items:
  size:
    - xs
    - sm
    - md
    - lg
    - xl
props:
  page: 5
  size: xl
  total: 100
---
::

### Disabled

Use the `disabled` prop to disable the pagination controls.

::component-code
---
ignore:
  - page
  - total
external:
  - page
model:
  - page
props:
  page: 5
  total: 100
  disabled: true
---
::

## Examples

### With links

Use the `to` prop to transform buttons into links. Pass a function that receives the page number and returns a route destination.

::component-example
---
name: 'pagination-links-example'
---
::

::note
In this example we're adding the `#with-links` hash to avoid going to the top of the page.
::

## API

### Props

:component-props

### Slots

:component-slots

### Emits

:component-emits

## Theme

:component-theme