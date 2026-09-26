# td-capitals-names

A lightweight TypeScript library with country capital names in English and native language forms.

It exports a typed set of constants for each country/territory and a combined array of all capital entries, making it useful for dashboards, forms, localization, and geographic data displays.

## Features

- typed capital metadata for many countries and territories
- `name` in English / international form
- `nativeName` in local language form where available
- ready-to-use constant exports and aggregated array
- works well in TypeScript projects with autocomplete and static checking

## Installation

```bash
npm install td-capitals-names
```

## Usage

```ts
import {
  AFGHANISTAN_CAPITAL,
  ALL_COUNTRIES_CAPITALS,
  type CountryCapital,
} from 'td-capitals-names';

console.log(AFGHANISTAN_CAPITAL.name); // Kabul
console.log(AFGHANISTAN_CAPITAL.nativeName); // کابل

const capitals: CountryCapital[] = ALL_COUNTRIES_CAPITALS;
console.log(capitals.length);
```

## Example use cases

- country selector and address forms
- geographic dashboards and maps
- admin panels with localized location data
- seed data for tests and fixtures
- internationalization and translation workflows
- country fact pages, travel apps, and knowledge bases

## Exported values

The package exports individual constants such as:

```ts
import {
  POLAND_CAPITAL,
  CZECHIA_CAPITAL,
  UNITED_STATES_CAPITAL,
  SOUTH_KOREA_CAPITAL,
} from 'td-capitals-names';

console.log(POLAND_CAPITAL);
console.log(CZECHIA_CAPITAL);
```

It also exports:

```ts
import { ALL_COUNTRIES_CAPITALS } from 'td-capitals-names';
```

## Notes

This package is intentionally data-focused and designed for easy consumption in TypeScript applications. It is especially useful when you need capital names without maintaining your own geographic dataset.

## License

MIT
