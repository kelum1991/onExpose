# Element 'viewport' Event Plugin
Event that is fired as soon as an element appears in the user's viewport.

## Usage

The event will only fire when the element comes in to view of the viewport, and out of view. It won't keep firing if the user scrolls and the element remains in view.

```
 jQuery("div").on('viewport', function(event, inVpPartial, inVpFull) {
  if (inVpPartial == true) {

  } else {

  }
 });
```

If you would like to  keep firing if the user scrolls and the element remains in view

```
jQuery("div").on('viewport', {once:false}, function(event, inVpPartial, inVpFull) {
 if (inVpPartial == true) {

 } else {

 }
});
```

| Option        | Type          | Default  | Description                          |
| ------------- |:-------------:| --------:| -------------------------------------|
| handler     | string | window   | You can set the element which user scrolls |                                     |
