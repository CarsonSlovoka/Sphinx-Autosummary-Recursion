Welcome to Sphinx-Autosummary-Recursion
=======================================

This package demonstrates automatic package detection using the new ``:recursive:`` option
in ``sphinx.ext.autosummary`` version 3.1.

The goal is to point Sphinx to the top of the source code tree and have it automatically detect
every module, however deeply nested.

For each module, it then creates summary tables listing every attribute, class, function
and exception in that module.

For each entry in a summary table, it then creates a hyperlink to a new page containing the 
documentation for that attribute, class, function or exception.

.. autosummary::
   :toctree: _autosummary
   :caption: API Reference
   :template: custom-module-template.rst
   :recursive:

   mytoolbox


REFERENCE
================

- Stackoverflow

    - `sphinx-autodoc is not automatic enough <https://stackoverflow.com/questions/2701998/sphinx-autodoc-is-not-automatic-enough/62613202#62613202>`_
    - `How can I get Sphinx autosummary to generate full API documentation <https://stackoverflow.com/questions/61576683/how-can-i-get-sphinx-autosummary-to-generate-full-api-documentation-for-classes>`_

`autosummary customizing templates <https://www.sphinx-doc.org/en/3.x/usage/extensions/autosummary.html#customizing-templates>`_
`rubric <https://www.sphinx-doc.org/en/master/usage/restructuredtext/directives.html?highlight=rubric#directive-rubric>`_
