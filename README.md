# DynamicZoomPlus
Macro to update the native Davinci Resolve Dynamic Zoom

The native dynamic zoom in resolve is always the length of the entire clip.
I created this plugin because sometimes I would want an image or clip to wait before zooming in or out and the hold the final framing like in documentaries.

This macro uses two transform nodes with no output because it is best for resizing the framing rectangles via Fusion Overlay.
The nodes are named *startTR* and *endTR*.

There is a guide you can enable to which shows the start and end framing in relation to the entire image.

There is a rectangle that represents the start framing (how zoomed in the clip will be) *strec*
and a rectangle then represents the end framing (how zoomed out the clip will be) *enrec*.

The center position of these are published and like to the transform nodes.

*crec* is where the calculation of the framing takes place based on an animation curve.
