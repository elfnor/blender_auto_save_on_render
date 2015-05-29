# Blender auto save on render add-on
Blender add-on to auto save image and blend file after render

Derivation of Auto Save add-on 
http://wiki.blender.org/index.php/Extensions:2.6/Py/Scripts/Render/Auto_Save

original code
https://svn.blender.org/svnroot/bf-extensions/contrib/py/scripts/addons/render_auto_save.py

This version adds an option to also auto save .blend file after render.  

The add-on settings are found on the Render panel.  
With "Auto Save Image" and "with .blend" set and the file "\Documents\test.blend" open, after rendering the following files will be created  

\Documents\auto_saves\test_001.png  
\Documents\auto_saves\test_001.blend

If "subfolder" is also set the files will be created in a sub-folder named after the blend file.  

\Documents\auto_saves\test\test_001.png  
\Documents\auto_saves\test\test_001.blend  

It is up to the user to make sure any additional files required such as texture images have been packed into the file.  

File>External Data>Pack All into .blend

