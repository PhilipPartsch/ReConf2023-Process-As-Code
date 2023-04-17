####################
Testing Instructions
####################


.. contents:: Content



.. instruction:: How to automate test execution?
   :id: INST_AUTO_TEST

   **We use readthedocs.io as build and test pipeline**
   
   **We use pytest to test our python code.**
   https://docs.pytest.org/en/latest/contents.html
   
   **We use pytest-reportlog to capture the test-log**
   https://github.com/pytest-dev/pytest-reportlog
   
   **We are Creating JUnitXML format files with pytest**
   https://docs.pytest.org/en/7.2.x/how-to/output.html#creating-junitxml-format-files

   **We use Sphinx-Test-Reports to automatically translate JUnitXML test results
   to sphinx-needs elements**
   https://sphinx-test-reports.readthedocs.io/en/latest/

   **We extend the test result and log output with record_xml_attribute and
   record_property from pytest**
   https://docs.pytest.org/en/7.2.x/how-to/output.html#record-property
   https://docs.pytest.org/en/7.2.x/how-to/output.html#record-xml-attribute

   **We use coverage to measure the test coverage of our modules**
   https://coverage.readthedocs.io/en/latest/

   **We use sphinx-collections to automatically translate test coverage reports
   to sphinx-needs elements.**
   https://sphinx-collections.readthedocs.io/en/latest/

   **Compare function signature with design**
   .. code:: rst

      import inspect
      print(inspect.signature(<function name>)



**variant information**
We can access sphinx tags vie tags object:
https://www.sphinx-doc.org/en/master/usage/configuration.html

Set with (example to set 'linux' in tags object):

- `tags.add('linux')` in `conf.py`
- `-t` in `sphinx-build` e.g. `sphinx-build -t linux`

Depending on tags we can create content:
https://www.sphinx-doc.org/en/master/usage/restructuredtext/directives.html#including-content-based-on-tags


We can set https://sphinx-needs.readthedocs.io/en/latest/configuration.html#needs-variants
depending on tag object via:

.. code:: python

   needs_variants = {
       "os_MAC":     str(tags.has('mac')),
       "os_LINUX":   str(tags.has('linux')),
       "os_Windows": str(tags.has('windows')),
   }


We can use variants to create needs on:
https://sphinx-needs.readthedocs.io/en/latest/directives/need.html#variants-for-options-support

and even delete them:
https://sphinx-needs.readthedocs.io/en/latest/directives/need.html#delete







