---
title: "UI-Router for React"
layout: single
excerpt: "State based routing for React"
sitemap: true
permalink: /react/
---

{% include toc icon="columns" title="React" %}

<center>
<img src="/images/logos/react.png" width="150">
</center>

UI-Router provides extremely flexible, state based routing to the React ecosystem.

## Getting UI-Router

The UI-Router package is distributed using [npm](https://www.npmjs.com/), the node package manager.

```
npm install --save ui-router-react
```

## Tutorials

Learn UI-Router by following our tutorials.

- [Hello World](/tutorial/react/helloworld)
- [Hello Solar System](/tutorial/react/hellosolarsystem)
- [Hello Galaxy](/tutorial/react/hellogalaxy)

## Sample application

The [UI-Router Sample App](/resources/sampleapp) is a non-trivial UI-Router application.
 
## Development

To fix a UI-Router bug, or create an enhancement, follow these steps: 

The Typescript source code for UI-Router for React can be found at <https://github.com/ui-router/react>
The react code depends on the UI-Router Core code, found at <https://github.com/ui-router/core>

To get started you will need to clone the UI-Router Core and UI-Router React repositories.

```
git clone https://github.com/ui-router/core ui-router-core
git clone https://github.com/ui-router/react ui-router-react
```

Then, you will need to build ui-router core and link it locally using `npm link`

```
cd ui-router-core
npm install
npm link
npm run build
```

Then, link to it from the ui-router-react repository

```
cd ../ui-router-react
npm install
npm link ui-router-core
```

To make changes to `ui-router-core` you should run the `npm run watch` script from the `ui-router-core` directory.
This will watch the ui-router core code, compile it, and run the test suite when the core code (or tests) are modified.

```
cd ../ui-router-core
npm run watch
```

