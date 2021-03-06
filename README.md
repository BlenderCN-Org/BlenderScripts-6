# Blender Scripts
Collection of simple Blender python scripts written to speedup workflow. These scripts are written for working with Blender 2.79a and have not been tested in other versions.

***

### Transfer Shape Keys by Surface (transfer_shape_keys.py)

Addon that copies shape keys between two non-identical meshes by using the surface deform modifier.

### Copy Object to Mesh Name (object_to_mesh_name.py) 

Operator that copies the name of the object to the name of it's mesh on selected objects.

### Bake and Export Actions (bake_and_export_actions.py)

Addon that bakes multiple actions from a control rig to a deform rig and exports it as an FBX.
Selected objects must include the source rig to bake from and the target rig to bake to.
The target should be the active object. The selection can also include the model(s) that should be exported with the target rig.

The export location is set in the addon preferences. Also set there is the source action name filter with "Source Action Name Prefix:" which filters actions to bake using a prefix. If this is left blank all actions will be baked and exported. "Export Action Name Prefix:" sets the target action name which will replace the source prefix or if left blank strip it from the exported actions. 

The addon is useful for transferring animations from a control rig to a deform rig for quick export.
