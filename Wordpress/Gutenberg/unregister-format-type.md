You can unregister existing rich text format by the code below.

```
wp.richText.unregisterFormatType('NAME');
```

## Function
```
/**
 * Unregisters a format.
 *
 * @param {string} name Format name.
 *
 * @return {?WPFormat} The previous format value, if it has been successfully
 *                     unregistered; otherwise `undefined`.
 */
export function unregisterFormatType( name ) {
	const oldFormat = select( 'core/rich-text' ).getFormatType( name );

	if ( ! oldFormat ) {
		window.console.error(
			`Format ${ name } is not registered.`
		);
		return;
	}

	if (
		oldFormat.__experimentalCreatePrepareEditableTree &&
		oldFormat.__experimentalGetPropsForEditableTreePreparation
	) {
		removeFilter( 'experimentalRichText', name );
	}

	dispatch( 'core/rich-text' ).removeFormatTypes( name );

	return oldFormat;
}
```

## Reference
gutnberg/rich-text/src/unregiter-format-type.js
