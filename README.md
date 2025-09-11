# TextOnAnySurface
Place text on any surface in Freecad.
 This macro automates the process of adding multi-line text to a selected face of an object.
#
# It performs the following steps:
# 1. Prompts for multi-line text, font, size, justification, line spacing, and projection properties.
# 2. For standard faces, it uses the Curves Workbench 'Sketch on Surface' tool for projection and now includes auto-scaling.
# 3. For annular faces (rings), it uses a custom function to create curved text.
# 4. Intelligently determines the bounds of the face.
# 5. Performs a Part Cut or Fuse operation using the more robust BOPTools (Part_CompJoinFeatures).
#
# Instructions:
# 1. Install the 'Curves' workbench from the Addon Manager.
# 2. To use: Select a single face on a solid object and run this macro.
