## RichTextToolbarButton

Slot to extend the format toolbar. Use it in the edit function of a `registerFormatType` call to surface the format to the UI.

### Example

ES5
```js
wp.richText.registerFormatType( /* ... */, {
	/* ... */
	edit: function( props ) {
		return wp.element.createElement(
			wp.editor.RichTextToolbarButton, {
				icon: 'editor-code',
				title: 'My formatting button',
				onClick: function() { /* ... */ }
				isActive: props.isActive,
			} );
	},
	/* ... */
} );
```

ESNext
```js
import { registerFormatType } from 'wp-rich-text';
import { richTextToolbarButton } from 'wp-editor';

registerFormatType( /* ... */, {
	/* ... */
	edit( { isActive } ) {
		return (
			<RichTextToolbarButton
				icon={ 'editor-code' }
				title={ 'My formatting button' }
				onClick={ /* ... */ }
				isActive={ isActive }
				/>
		);
	},
	/* ... */
} );
```

## Reference
https://wordpress.org/gutenberg/handbook/designers-developers/developers/tutorials/format-api/2-toolbar-button/
