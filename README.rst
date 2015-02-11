pytest-batches
==============

.. image:: http://www.repostatus.org/badges/0.1.0/concept.svg
   :alt: Project Status: Concept - Minimal or no implementation has been done yet.
   :target: http://www.repostatus.org/#concept

pytest plugin to run marked tests in batches, and skip the rest if a
batch fails

Do you have groups of tests that take more time or resources to run than
others, such as purely-mocked unit tests and browser automation or
integration tests? If you mark the tests (using ``pytest.mark``), this
plugin will allow you to run the tests in ordered batches (based on
marker), and then skip all tests in subsequent batches if a batch fails
(i.e. allowing you to run integration tests only if the unit tests
passed).

References:

* `Working with plugins and conftest files <http://pytest.org/latest/plugins.html#conftest-py-local-per-directory-plugins>`__
* pytest builtin `mark plugin <https://bitbucket.org/hpk42/pytest/src/fa62c5c63c2fb5870852676d8d8899b9656214fd/_pytest/mark.py?at=default>`__
* pytest builtin `skip plugin <https://bitbucket.org/hpk42/pytest/src/fa62c5c63c2fb5870852676d8d8899b9656214fd/_pytest/skipping.py?at=default>`__
* `pytest-instafail <https://github.com/jpvanhal/pytest-instafail/>`__ shows failures instantly
* `pytest-markfiltration <https://github.com/adamgoucher/pytest-markfiltration>`__ filters tests based on MarkInfo objects
* `pytest-sourceorder <https://git.fedorahosted.org/cgit/python-pytest-sourceorder.git/>`__ ensures tests within a class are run in source order
* `pytest-stepwise <https://github.com/nip3o/pytest-stepwise>`__ runs all tests until one fails, then continues the next run from where it left off
* `pytest-ordering <https://github.com/ftobia/pytest-ordering>`__ runs tests in a specific order
* `pytest-rerunfailures <https://github.com/klrmn/pytest-rerunfailures>`__ re-runs failed tests up to X times, based on a marker
