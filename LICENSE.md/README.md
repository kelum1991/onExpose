# Element 'viewport' Event Plugin
Event that is fired as soon as an element appears in the user's viewport.

## Usage

The event will only fire when the element comes in to view of the viewport, and out of view. It won't keep firing if the user scrolls and the element remains in view.

  jQuery("div").on('viewport', function(event, inVpPartial, inVpFull) {
	  if (inVpPartial == true) {
	
	  } else {

	  }
  });
