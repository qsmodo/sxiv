# Fork of **Simple X Image Viewer**

![Screenshot](sxiv.png)

Changes
-------

* If a single image argument is given, the image is displayed as
expected, but all **other images in the directory are also loaded** for 
navigation [(#352)](https://github.com/muennich/sxiv/issues/352).

    * If more than one argument is given, then only the specified files
    and directories are loaded, as in mainstream Sxiv.

* No file will ever be loaded twice.

* Additional configurable options (via X-resources):

    * **Marks** are more conspicuous, a red rectangle around the image.

    * **Status bar colors**. 

    * **External key handler** can be invoked in a single key press.

    * **Square thumbnails**.

    * **Window title** consists of a prefix and a suffix. The prefix is
    a fixed string and the suffix is one of

      ```
      0  Basename of file
      1  Basename of directory
      2  Full path to file
      3  Full path to directory
      4  Empty string
      ```
  
      The default window title is "sxiv - {file basename}".

    * The full-screen background can be different.

* Escape key can be mapped in `config.h`.

Install
-------

    $ make
    # make install
