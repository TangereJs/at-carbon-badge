
<!---

This README is automatically generated from the comments in these files:
at-carbon-badge.html

Edit those files, and our readme bot will duplicate them over here!
Edit this file, and the bot will squash your changes :)

The bot does some handling of markdown. Please file a bug if it does the wrong
thing! https://github.com/PolymerLabs/tedium/issues

-->

## Changes in 2.0
* Target updates target in an animation frame rather than 1 ms.

## &lt;at-carbon-badge&gt;

`<at-carbon-badge>` is a circular text badge that is displayed on the top right
corner of an element, representing a status or a notification. It will badge
the anchor element specified in the `for` attribute, or, if that doesn't exist,
centered to the parent node containing it.

Badges can also contain an icon by adding the `icon` attribute and setting
it to the id of the desired icon. Please note that you should still set the
`label` attribute in order to keep the element accessible. Also note that you will need to import
the `iron-iconset` that includes the icons you want to use. See [iron-icon](../iron-icon)
for more information on how to import and use icon sets.

Example:

```html
<div style="display:inline-block">
  <span>Inbox</span>
  <at-carbon-badge label="3"></at-carbon-badge>
</div>

<div>
  <paper-button id="btn">Status</paper-button>
  <at-carbon-badge icon="favorite" for="btn" label="favorite icon"></at-carbon-badge>
</div>

<div>
  <paper-icon-button id="account-box" icon="account-box" alt="account-box"></paper-icon-button>
  <at-carbon-badge icon="social:mood" for="account-box" label="mood icon"></at-carbon-badge>
</div>
```

### Styling

The following custom properties and mixins are available for styling:

| Custom property | Description | Default |
| --- | --- | --- |
| `--at-carbon-badge-background` | The background color of the badge | `--accent-color` |
| `--at-carbon-badge-opacity` | The opacity of the badge | `1.0` |
| `--at-carbon-badge-text-color` | The color of the badge text | `white` |
| `--at-carbon-badge-width` | The width of the badge circle | `20px` |
| `--at-carbon-badge-height` | The height of the badge circle | `20px` |
| `--at-carbon-badge-margin-left` | Optional spacing added to the left of the badge. | `0px` |
| `--at-carbon-badge-margin-bottom` | Optional spacing added to the bottom of the badge. | `0px` |
| `--at-carbon-badge` | Mixin applied to the badge | `{}` |


