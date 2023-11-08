# Viewport Render Texture loosing node_path reference

When a viewport render texture is referencing a SubViewport that is the root of its own Subscene, the reference is lost when the editor is closed and reopened.

## Reproduction

- Checkout this repo
- Open in Editor
- Save the main scene or hit "play"
- The NodePath changes from "BrakingReference/SubViewport" to ".", reference is lost.
