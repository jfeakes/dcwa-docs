Usage
========================

.. _transcoding:

Transcoding
-----------
rawcook_multi.py
~~~~~~~~~~~~~
batch_dv_to_mov.py
~~~~~~~~~~~~~
batch_mp3.py
~~~~~~~~~~~~~
batchprores422.py
~~~~~~~~~~~~~

concat.py
~~~~~~~~~~~~~
-  Takes a folder of mp4 files and concatenates together using ffmpeg
-  For use in Lasergraphics workflow when capturing multiple clips in a single reel
-  Usage: 

.. code-block:: console 
   
   py concat.py \path\to\directory\to\concatenate

-  ``py concat.py -h`` to see extra optional flags
-  Dependencies: ffmpeg, colorama

concat.bat
~~~~~~~~~~~~~
-  .bat file used as a Desktop drag'n'drop shortcut for ``concat.py``
-  Usage: Drag'n'drop folder of files for concatenation onto a shortcut icon of the .bat file. No optional flags are applied. 

concataudio.py
~~~~~~~~~~~~~
dvd_concat.py
~~~~~~~~~~~~~
dvd_concat.bat
~~~~~~~~~~~~~
ff_combine.py
~~~~~~~~~~~~~
-  Usage: ``py ff_combine.py`` then follow prompts

ff_fps.py
~~~~~~~~~~~~~
gensubs.bat
~~~~~~~~~~~~~
hflip-mp4.py
~~~~~~~~~~~~~
hflip.py
~~~~~~~~~~~~~
makeconcat.py
~~~~~~~~~~~~~
refolderaudio.py
~~~~~~~~~~~~~
rename.py
~~~~~~~~~~~~~
whisp.py
~~~~~~~~~~~~~
whisp.bat
~~~~~~~~~~~~~


Photography
-----------
batchpdfa.py
~~~~~~~~~~~~~
-  Usage: ``py batchpdfa.py \path\to\master\directory``
-  Allows user to select one or more folders of images to convert to a PDF/A-2b file. The file is then verified for conformance to that standard
-  Tested with jpeg images only
-  Dependencies: tesseract, ghostscript, colorama

batchocr.py
~~~~~~~~~~~~~
delseps.py
~~~~~~~~~~~~~
filecount.py
~~~~~~~~~~~~~
filecount.bat
~~~~~~~~~~~~~

Misc
-----------
ddcwafuncs.py
~~~~~~~~~~~~~
Usage
=====

.. _installation:

Installation
------------

To use Lumache, first install it using pip:

.. code-block:: console

   (.venv) $ pip install lumache

Creating recipes
----------------

To retrieve a list of random ingredients,
you can use the ``lumache.get_random_ingredients()`` function:

.. autofunction:: lumache.get_random_ingredients

The ``kind`` parameter should be either ``"meat"``, ``"fish"``,
or ``"veggies"``. Otherwise, :py:func:`lumache.get_random_ingredients`
will raise an exception.

.. autoexception:: lumache.InvalidKindError

For example:

>>> import lumache
>>> lumache.get_random_ingredients()
['shells', 'gorgonzola', 'parsley']

