# Binding text

Text binding can be done in two different ways

* Mustache syntax
* `v-text` directive

## Mustache syntax

Use `{{ dataPropertyName }}` in HTML inner elements

## `v-text` directive

Use the v-text directive in the opening HTML tags and leave the inner element blank

* `<div v-text="dataPropertyName"></div>`

- Inner element is left blank as it will be replaced with the provided data property
- An error will occur if the inner element is not blank