docear_helpers
==============

This respository mainly contains a small python script ``docear_helpers``.
It is for use with an installation of docear, the literatur and pdf mindmapping
tool.

Make docear_helpers executable (chmod +x docear_helpers) and use like ``docear_helpers command``
where ``command`` is one of the following:

- init : initializes current directory as a docear project

    (make sure that docear is closed for this to work - otherwise settings get overwritten and the project cannot be automatically imported)
- move : moves / renames docear project to another directory
- autorename : renames all pdf files according to their meta-data in
  references.bib (concerns all pdfs listed in the given docear project)
- open_user_settings : opens the user.settings file in the default text editor



tips and tricks
===============

To enhance Docear on Windows, enter this line into the manual pdf reader configuration part under preferences.

    C:\Program Files\Tracker Software\PDF Viewer\PDFXCview.exe*/A*"nolock=yes=OpenParameters &page=$PAGE"*"$FILE"

The nolock is crucial for enabling auto update from docear to pdf-reader.

Unfortunately the other direction is not yet supported by docear, you have to update your incoming node manually and
pick for every change the pdf-version.
I would love to implement an automatic overwrite feature for this on pdf change, however I am still not into docear
source code yet.
