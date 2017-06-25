[![Published on webcomponents.org](https://img.shields.io/badge/webcomponents.org-published-blue.svg)](https://www.webcomponents.org/element/Zecat/geo-fr-api)

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
      town-name="Paris"
    ></geo-fr-towns>

    <h2>Matching towns:</h2>
    <template is="dom-repeat" items="[[towns]]">
      <p>
        Name: [[item.townName]],
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
<!-- towns components -->
<link rel="import" href="/bower_components/geo-fr-api/geo-fr-towns/geo-fr-towns.html">
<!-- addresses components -->
<link rel="import" href="/bower_components/geo-fr-api/geo-fr-addresses/geo-fr-addresses.html">
```

## What is inside

### Elements

- [geo-fr-towns](/geo-fr-towns)
- [geo-fr-addresses](/geo-fr-addresses)
- geo-fr-departments (incomming)
- geo-fr-region (incomming)
