# knockout-i18n
A simple internationalization module for KnockoutJs, check out `example.html` for simple workings.

## API
### `ko.i18n.locale`
The current locale string, or array of strings as locale chain fall back. This module read this observable to resolve a bundle for translations.

### `ko.i18n.setBundle(locale, bundle)`
Assigns a bundle object of key-value translation under target locale.

- `locale` __{string|array}__ Target locale string(s)
- `bundle` __{Object}__ An object for direct key-value translation.

### `ko.i18n.setBundles(bundles)`
Assigns multiple bundles to multiple locale, act as a multiple version of `ko.i18n.setBundle(locale, bundle)`.

- `bundles` __{Object}__ An object with keys as locale, and values be designated bundle.

## Bindings
### `i18n: key`

- `key` __{string}__ Resolves a translation using current `ko.i18n.locale`.

### `i18n-options: substitudes`

- `substitudes` __{array}__ Array of values to be subtitudes using mustache syntax inside the bundle translation, see `example.html` for example usage.
