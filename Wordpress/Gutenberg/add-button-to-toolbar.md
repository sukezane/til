## RichTextToolbarButton

Slot to extend the format toolbar. Use it in the edit function of a `registerFormatType` call to surface the format to the UI.

### Options
type:  
character:  
onUse:  
icon: Toolbar button icon. You can set <svg> tag and [dash-icons](https://developer.wordpress.org/resource/dashicons/)  
title: Toolbar title.  
onClick: Catch onclick event.  
isActive: Get state that current Toolbar is active.  
shortcutType: You can set the shortcut key type. ex.`primary`, `primaryShift`.  
shortcutCharacter: Shortcut command character. ex. `b`  

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
wp-includes/js/dist/format-library.min.js
https://unix.stackexchange.com/questions/168505/what-is-primary-for-a-key

