Display featured image on editor.  

```
const { __ } = wp.i18n;
const { registerBlockType } = wp.blocks;
const { PostFeaturedImage } = wp.editor;

registerBlockType( 'dm-block/featured-image', {
	title: __( 'Featured Image' ),
	icon: 'format-image',
	category: 'common',
	edit( { className } ) {
		return (
			<div className={ className }>
				<PostFeaturedImage />
			</div>
		);
	},
	save( { className } ) {
		// Doesn't save an data. Defer's to theme's placement of featured image.
		return '';
	},
} );
```

## Reference
https://github.com/modularwp/gutenberg-block-featured-image  
