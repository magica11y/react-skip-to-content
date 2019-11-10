`<SkipToContent … />`
=====================
> A React component which provides a flexible & configurable 'skip to main content' link.

[![Travis](https://img.shields.io/travis/com/magica11y/react-skip-to-content.svg?style=for-the-badge)](https://travis-ci.com/magica11y/react-skip-to-content)
[![npm](https://img.shields.io/npm/v/@magica11y/react-skip-to-content.svg?style=for-the-badge "NPM")](https://www.npmjs.com/package/@magica11y/react-skip-to-content)
[![Bundlephobia](https://img.shields.io/bundlephobia/min/@magica11y/react-skip-to-content.svg?style=for-the-badge "Bundle size (minified)")](https://bundlephobia.com/result?p=@magica11y/react-skip-to-content)
[![Bundlephobia](https://img.shields.io/bundlephobia/minzip/@magica11y/react-skip-to-content.svg?style=for-the-badge "Bundle size (minified+gzipped)")](https://bundlephobia.com/result?p=@magica11y/react-skip-to-content)
[![Coveralls](https://img.shields.io/coveralls/magica11y/react-skip-to-content.svg?style=for-the-badge "Test coverage status")](https://coveralls.io/r/magica11y/react-skip-to-content)
[![David](https://img.shields.io/david/magica11y/react-skip-to-content.svg?style=for-the-badge "Dependencies")](https://david-dm.org/magica11y/react-skip-to-content)
[![David](https://img.shields.io/david/dev/magica11y/react-skip-to-content.svg?style=for-the-badge "Dev Dependencies")](https://david-dm.org/magica11y/react-skip-to-content?type=dev)
[![node](https://img.shields.io/node/v/@magica11y/react-skip-to-content.svg?style=for-the-badge "Node engine")](https://www.npmjs.com/package/@magica11y/react-skip-to-content)
[![License](https://img.shields.io/github/license/magica11y/react-skip-to-content.svg?style=for-the-badge "MIT license")](LICENSE.md)
![Greenkeeper](https://badges.greenkeeper.io/magica11y/react-skip-to-content.svg?style=flat-square "Greenkeeper")

[![Magica11y cover](https://cdn.jsdelivr.net/gh/magica11y/cauldron@1.0.11/assets/Magica11y-cover.jpg "Magica11y cover")](https://magica11y.github.io)


# :sparkles: Introduction

`<SkipToContent … />` is a flexible & configurable wrapper around a standard HTML 'skip to main content' anchor/link tag (`<a>`).

Quoting from the ["Skip Navigation" Links](https://webaim.org/techniques/skipnav/) article on [WebAIM](https://webaim.org):

> The main content is not usually the first thing on a web page. Keyboard and screen reader users generally must navigate a long list of navigation links, sub-lists of links, corporate icons, site searches, and other elements before ever arriving at the main content. This is particularly difficult for users with some forms of motor disabilities.

> Without some sort of system for bypassing the long list of links, some users are at a huge disadvantage. Consider users with no arm movement, who use computers by tapping their heads on a switch or that use a stick in their mouth to press keyboard keys. Requiring users to perform any action perhaps 100s of times before reaching the main content is simply unacceptable.

> Of course, sighted people who use their mouse do not have any trouble with pages such as this. They can almost immediately scan over the page and identify where the main content is. In effect, sighted users have a built-in "skip navigation" mechanism: their eyes. They can also bypass the many links before the main content and click directly on the link they want with the mouse. The "skip navigation" idea was invented to give screen reader and keyboard users the same capability of going directly to the main content that sighted mouse users take for granted.


# :rocket: Getting started

## :building_construction: Installation

You can install `<SkipToContent … />` using a package manager such as [`yarn`](https://yarnpkg.com/en/package/@magica11y/react-skip-to-content) or [`npm`](https://www.npmjs.com/package/@magica11y/react-skip-to-content)…

```sh
$ yarn add "@magica11y/react-skip-to-content"
# OR
$ npm install --save "@magica11y/react-skip-to-content"
```

You can also include `<SkipToContent … />` from a CDN on your page, such as [jsDelivr](https://www.jsdelivr.com/package/npm/@magica11y/react-skip-to-content) or [unpkg](https://unpkg.com/@magica11y/react-skip-to-content)…

```html
<script src="https://cdn.jsdelivr.net/npm/@magica11y/react-skip-to-content@latest/dist/magica11y.reactSkipToContent.min.js"></script>
<!-- OR -->
<script src="https://unpkg.com/@magica11y/react-skip-to-content@latest/dist/magica11y.reactSkipToContent.js"></script>
```

## :game_die: Usage

```jsx
import React from 'react';
import ReactDOM from 'react-dom';

import SkipToContent from '@magica11y/react-skip-to-content';

const App = () => {
  return (
    <>
      <SkipToContent targetId="#main-content" />

      <main id="main-content">
        {/* rest of your React application here */}
      </main>
    </>
  );
};

ReactDOM.render(<App />, document.getElementById('root'));
```

# :nut_and_bolt: API

`<SkipToContent … />` takes the following props:

| Prop name | Type | Default | Description |
| --- | --- | --- | --- |
| `targetId` | `string` | _(required)_ | Value of the `id` attribute to which the link should navigate to |
| `linkComponent` | `React.Node` _(optional)_ | `a` | React component to replace the underlying anchor tag |
| `className` | `ClassNamesExport` _(optional)_ | `null` | Object to pass to the [classnames](https://jedwatson.github.io/classnames) function |

# :checkered_flag: Typechecking

You can import the [Flow](https://flow.org) types from the provided [libdefs](https://flow.org/en/docs/libdefs)
in `node_modules/@magica11y/react-skip-to-content/lib` by configuring them in your `.flowconfig`…

```
[libs]
node_modules/@magica11y/react-skip-to-content/lib
```

# :scroll: License

[![License](https://img.shields.io/github/license/magica11y/magica11y.svg?style=for-the-badge "MIT license")](LICENSE.md)

See [LICENSE.md](LICENSE.md) for more details.

Handcrafted with :heart: by [Rishabh Rao](https://github.com/rishabhsrao).

[![Twitter](https://img.shields.io/twitter/follow/rishabhsrao.svg?style=social)](https://twitter.com/rishabhsrao)
