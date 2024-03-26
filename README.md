# Blender Addon for Wavefront OBJ with Vertex Color

Blender Addon to import/export Wavefront OBJ with Vertex Color. This addon is based on [the official blender addon](https://github.com/blender/blender-addons).

So far the testing is not really sufficient. If you have any troubles importing / exporting your .obj data, please report an issue.

Something SUPER important that I realized after failing multiple times while exporting is that the color attribute in Blender has to be named "Col". If it has another name or more than one, it won't work.

This fork has an error correction that was causing some models (for reasons unknown to me) to fail during export. The change makes it so that in the line where the failure occurred, it attempts to export and, in case of failure, defaults to a white color.

Tested on Blender 4.0.1.

## Installation

1. Download zip of this repository.
2. Open your blender 2.8
3. Navigate to `Preferences --> Add-ons`
4. Press `Install` and select the downloaded zip
5. Enable the addon
6. Done. You can import Wavefront OBJ with vertex color from `File --> Import --> Wavefront with VC (.obj)`, or export it in the same way.
