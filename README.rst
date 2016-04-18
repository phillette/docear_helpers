docear_helpers
==============

This respository mainly contains a small python script ``docear_helpers``.
It is for use with an installation of docear, the literatur and pdf mindmapping
tool.

Make docear_helpers executable (chmod +x docear_helpers) and use like:

    $docear_helpers command

where ``command`` is one of the following:

- init : initializes current directory as a docear project

    (make sure that docear is closed for this to work - otherwise settings get overwritten and the project cannot be automatically imported)
- move : moves / renames docear project to another directory
- autorename : renames all pdf files according to there meta-data in
  references.bib (concerns all pdfs listed in the given docear project)
- open_user_settings : opens the user.settings file in the default text editor

