## 画像の対応  

```
function my_post_image_html( $html, $post_id, $post_image_id ) {
    if (is_amp() === false) {
        return $html;
    };
    
    $html = preg_replace('/<img (.*?)>/i', '<amp-img $1 layout="intrinsic"></amp-img>', $html);
    $html = preg_replace('/<img (.*?) \/>/i', '<amp-img $1 layout="intrinsic"></amp-img>', $html);
	return $html;
}
```

## iframeの対応  
```
function the_content_amp($the_content)
{
    if (is_amp() === false) {
        return $the_content;
    };
    $iframe = '<div class="p-flex p-flex--wrap p-flex--center p-single p-single--follow">
    <div class="p-single__iframe-wrapper">
        <amp-iframe class="u-mx" $1 $2 $3 sandbox="allow-scripts allow-same-origin" layout="responsive">
    </amp-iframe>
    </div>
    </div>';
    $the_content = preg_replace('/<img (.*?)>/i', '<amp-img $1></amp-img>', $the_content);
    $the_content = preg_replace('/<img (.*?) \/>/i', '<amp-img $1></amp-img>', $the_content);
    $the_content = preg_replace('/<iframe (.*?)(allowtransparency="true")(.*?)><\/iframe>/is', $iframe, $the_content);

    return $the_content;
}
```

## Reference  
https://qiita.com/keki/items/60565555a0ee9f5daa2b#%E3%81%93%E3%81%A0%E3%82%8F%E3%82%8A%E3%83%9D%E3%82%A4%E3%83%B3%E3%83%88amp-img%E3%82%BF%E3%82%B0%E3%81%AEheight%E8%A8%AD%E5%AE%9A
