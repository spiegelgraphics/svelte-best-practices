# svelte-best-practices

This is an (incomplete) list of Svelte best practices that we try to follow at Der SPIEGEL.


## Manipulate the DOM with HTML.
Avoid using JavaScript to make changes to the DOM.

## Solve a challenge with HTML/CSS first.
If that is not possible, then use JavaScript.

## Write short components.
Encapsulate what can be encapsulated. The code of a component should fit your screen.

## Write concise reactive `$` blocks.
Avoid large reactive blocks and keep side-effects on a low level.

## Scope CSS to the actual component.
Avoid `:global` and do not use it when an app is embedded.

## Do not hard code data or dimensions.
Everything should be dynamic.

## Keep your objects immutable.
Create new objects, if you change property values and use `<svelte:options immutable>` whenever possible.

## Use two-way binding instead of event handlers.
It's often less boilerplate. However, there are cases where event handling is safer.

## Use `class:` and `style:` instead of manual interpolation.
It's just less error prone.

## Use clear and descriptive variable names.
Nothing to add here.

## Plan your store interdependencies.
Avoid complicated or even circular store dependencies.

## Use an action instead of `bind:this` and `onMount`.
If you need access to a DOM element, this is a more reusable way.

## Use `onDestroy` or store unmount functions.
Avoid memory leaks.