# ShiVaMeshOutline
Modular Lua AI that creates an outline of variable thickness and color around an object

The trick lies in creating an inflated secondary mesh and assigning a special material to it:
- standard background materials: priority 127
- highlight-able object: material priority 125
- highlight border material: priority 126, no depth write

Script based on an idea by Don "dwilki99" Wilkins. Includes a demo game with a spinning box. If you want to enable this effect on one of your own models, copy the "ObjectOutlineHighlighter" AI out of this STE and toggle its activate/deactivate handler. The highlight material needs to be referenced in the game as resource.
