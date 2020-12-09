# Fork of **Simple X Image Viewer**

![Screenshot](sxiv.png)

Changes
-------

* If a single image argument is given, the image is displayed as
expected, but all other images in the directory are also loaded. 
[(#352)](https://github.com/muennich/sxiv/issues/352).

    * If more than one argument is given, then only the specified files
    and directories are loaded, as in mainstream Sxiv.

* No file will ever be loaded twice.

* Marks are more conspicuous, a red rectangle around the image. The color
can be changed via `mark` X-resource. Incorporated from 
[#294, thanks to @spaeps](https://github.com/muennich/sxiv/issues/294).

* Background is dark and foreground is green by default. Both can still be
overriden via `background` and `foreground` X-resources.

* Escape key can be mapped in `config.h`.
