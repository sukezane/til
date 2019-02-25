# HOC(Higher Order Component)
コンポーネントを引数にして、カスタマイズしたコンポーネントを返す関数のこと。

例えばWordpressのGutenbergのプラグインのcomposeでは、以下のような感じでHOCが利用されている。

```
const applyWithSelect = withSelect( ( select, ownProps ) => {
    return doSomething( select, ownProps);
} );
const applyWithDispatch = withDispatch( ( dispatch, ownProps ) => {
    return doSomethingElse( dispatch, ownProps );
} );

export default compose(
    withPluginContext,
    applyWithSelect,
    applyWithDispatch,
)( PluginSidebarMoreMenuItem );
```

一方でHOCを使わない場合、以下のように記述される

```
const applyWithSelect = withSelect( ( select, ownProps ) => {
    return doSomething( select, ownProps);
} );
const applyWithDispatch = withDispatch( ( dispatch, ownProps ) => {
    return doSomethingElse( dispatch, ownProps );
} );

export default withPluginContext(
    applyWithSelect(
        applyWithDispatch(
            PluginSidebarMoreMenuItem
        )
    )
);
```

このように、HOCを使うとコンポーネントの引数にコンポーネントを渡す記述をより見やすく書くことができる。

##Reference
https://qiita.com/numanomanu/items/2b66d8b2887d44f857dc
https://wordpress.org/gutenberg/handbook/designers-developers/developers/packages/packages-compose/
