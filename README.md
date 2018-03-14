[![Published on webcomponents.org](https://img.shields.io/badge/webcomponents.org-published-blue.svg)](https://www.webcomponents.org/element/cobra79/cobra-gravity)

# cobra-gravity
Polymer element to convert degrees plato, brix and specific gravity
## Installation
bower install cobra-gravity --save
## Usage
Set one of the input attributes:
plato-in, brix-in or density-in
and you will get all output attributes:
plato-out, brix-out and density-out

The output attributes are caculated based on the last input attribute.

## Demo
<!--
```
<custom-element-demo>
  <template>
    <link rel="import" href="cobra-carbonation.html">
    <next-code-block></next-code-block>
  </template>
</custom-element-demo>
```
-->
```html
<template>
          <dom-bind>
            <template>
              <paper-input value="{{platoIn}}" label="Plato In"></paper-input>
              <paper-input value="{{brixIn}}" label="Brix In"></paper-input>
              <paper-input value="{{densityIn}}" label="Density In"></paper-input>
              <cobra-gravity
                      plato-in="{{platoIn}}"
                      plato-out="{{platoOut}}"
                      brix-in="{{brixIn}}"
                      brix-out="{{brixOut}}"
                      density-in="{{densityIn}}"
                      density-out="{{densityOut}}"
              ></cobra-gravity>
              <h3>Plato Out: [[platoOut]]</h3>
              <h3>Brix Out: [[brixOut]]</h3>
              <h3>Density Out: [[densityOut]]</h3>
            </template>
          </dom-bind>
        </template>
```



## License
MIT

