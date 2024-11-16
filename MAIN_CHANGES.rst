Main Changes
------------

This is a fork of detectron2 used in an experimental geowatch task. It has
changes related to kwcoco support and

Given an install of geowatch you can resolve detectron2 to our fork with the following code:

.. code:: goeowatch

    import geowatch_tpl
    detectron2 = geowatch_tpl.import_submodule('detectron2')

After that imports that reference detectron2 will use our fork.


The main changes are:

* Support for reading kwcoco compressed json files

* Support for certain kwcoco data structures

* Hacked hard coded disabling of EXIF reading. (may change)

* Moved the configs directory into the module itself as a resource directory so the pip installed version can access the predefined configs.
