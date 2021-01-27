## Extracting UnrealScripts

Open a cmd and input ``decompress pathToGame\TdGame\CookedPC\yourFile.u``, this intermediary step is necessary for ``UE-Explorer`` to read it properly, the resulting file will sit inside the ``unpacked`` folder.

Install and open ``UE-Explorer`` , File > Open File... > navigate to and select ``unpacked\yourFile.u``.
Above the ``Package`` tab there's a ``Tools`` button to export all scripts into a folder.

## Exporting models, textures, animations and sound

Open umodel.exe, fill in the path to the game's directory, press ``Ok``.

The rest is pretty self explanatory but there's a couple of gotchas:

- When opening, use ``PageUp`` and ``PageDown`` keys to look at the other assets within this package
- Faith's gameplay models are under ``Characters/CH_TKY_Crim_Fixer*.upk``
- You will need to append packages together to play animations correctly, 
  - open a character package first then press 'o' to bring the package browser, navigate to some animations and select it then instead of opening it press the arrow to the right of the button and click on append.
- Previewing animation is done by first pressing Ctrl+A to bind the set to the model, ``[`` and ``]`` to switch between the different animations contained and the space bar to play it

## Exporting AnimTrees

Not sure, probably need to do this by hand if it's not compiled into UnrealScripts

## Importing models and animations

Contained within this directory is an archive named ``Blender psk psa plugin`` or some such, it contains an addon for Blender.

To install it extract the files contained within it > Open blender > Edit > Preferences... > Add-ons > Install... > Navigate to the extracted files > Install Add-On > In the search bar of the preferences window type in ``Import Unreal Skeleton Mesh`` > Make sure the checkbox is ticked.

In the viewport you should now have on the upper right corner a new vertical tab named ``PSK/PSA``, if that's not the case make sure that the panel is not hidden by pulling on the tiny arrow to the right of the axis gizmo.