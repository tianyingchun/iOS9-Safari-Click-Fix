 [ jQuery 2.0+  must be included in project in order for this library to work ! ]


 * iOS9 'click', 'mousedown' and 'mouseup' fix
 * ---------------------------------------------
 * Include this script in your poject to fix 'click', 'mousedown' and 'mouseup' event
 * handling for $(window), $(document), $('body') and $('html'). By default iOS9 Safari is
 * suppressing those events in some situations and without some magic they can't be rely on.
 * This fix is blocking native event handlers from firing
 * (in some rare cases event will reach it's destination)
 * and it handles native event handlers basing on 'touchstart' and 'touchend' event.


PLEASE MIND THE 'touchstart' and 'touchend' events being used to track event bubbling ant trigger 'click' ,'mousedown' and 'mouseup'.
Therefor .stopPropagation() called on 'click' event will also block 'mouseup' event and 'touchend' handlers from execute.
