[![Published on webcomponents.org](https://img.shields.io/badge/webcomponents.org-published-blue.svg)](https://www.webcomponents.org/element/Zecat/google-recaptcha)

# Geo Fr Api

A collection of elements wrapping the [french governmental geo api](https://api.gouv.fr/api/api-geo.html).

<!--
```
<custom-element-demo height="200">
<template>
<link rel="import" href="geo-fr-towns/geo-fr-towns.html">
<next-code-block></next-code-block>
</template>
</custom-element-demo>
```
-->
```html
<dom-bind>
  <template>

    <geo-fr-towns
      auto
      value="{{towns}}"
      name="Paris"
    ></geo-fr-towns>

    <template is="dom-repeat" items="[[towns]]">
      <p>
        Name: [[item.nom]],
        postal code: [[item.codePostaux.0]],
        departement code: [[item.codeDepartement]],
        population: [[item.population]]
      </p>
    </template>

  </template>
</dom-bind>
```

## Install

```bash
  bower install -S Zecat/geo-fr-api
```

## Import

```html
<!-- All components -->
<link rel="import" href="/bower_components/geo-fr-api/geo-fr-api.html">
<!-- Towns components -->
<link rel="import" href="/bower_components/geo-fr-api/geo-fr-towns.html">
```

## What is inside

### Elements

- [geo-fr-towns](/geo-fr-towns)
- geo-fr-departments (incomming)
- geo-fr-region (incomming)
