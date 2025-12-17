# Foliopress Components

Set of light-weight JavaScript functions for simpler creation of attractive browser popups for your WordPress plugins.

Uses WordPress Gutenberg styling `wp-components` which is 11 kB with GZip.

Only uses vanilla JavaScript.

## Foliopress Confirm

Inspired by the standard JavaScript. `confirm(message)` function.

Simply copy the `foliopress-confirm.js` to your plugin and add this in your PHP code:

```
wp_enqueue_style( 'wp-components' );
wp_enqueue_script( 'foliopress-confirm', plugin_dir_url( __FILE__ ) . 'js/foliopress-confirm.js' );
```

In JavaScript, use:

```
foliopress_confirm(
  'Remove story?',
  function() {
    /* "Yes" callback */
  },
  function() {
    /* Optional "No" callback */
  }
);
```
