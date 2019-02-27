componnts package that make svg tag.

## Options
Circle:  
G:  
Path:  
Polygon:  
Rect:  

## Example
```
<SVG
  viewBox="0 0 24 24"
  xmlns="http://www.w3.org/2000/svg"
>
  <Path fill="none" d="M0 0h24v24H0V0z" />
  <G>
    <Path d="M20 4v12H8V4h12m0-2H8L6 4v12l2 2h12l2-2V4l-2-2z" />
    <Path d="M12 12l1 2 3-3 3 4H9z" />
    <Path d="M2 6v14l2 2h14v-2H4V6H2z" />
  </G>
</SVG>
```

```
/**
 * WordPress dependencies
 */
import { createElement } from '@wordpress/element';

export const Circle = ( props ) => createElement( 'circle', props );
export const G = ( props ) => createElement( 'g', props );
export const Path = ( props ) => createElement( 'path', props );
export const Polygon = ( props ) => createElement( 'polygon', props );
export const Rect = ( props ) => createElement( 'rect', props );

export const SVG = ( props ) => {
	const appliedProps = {
		...props,
		role: 'img',
		'aria-hidden': 'true',
		focusable: 'false',
	};

	// Disable reason: We need to have a way to render HTML tag for web.
	// eslint-disable-next-line react/forbid-elements
	return <svg { ...appliedProps } />;
};
```

## Reference
gutenberg-master/packages/components/src/primitives/svg/index.js
