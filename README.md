# pytest-batches
pytest plugin to run marked tests in batches, and skip the rest if a batch fails

Do you have groups of tests that take more time or resources to run than others, such as purely-mocked unit tests and browser automation or integration tests? If you mark the tests (using ``pytest.mark``), this plugin will allow you to run the tests in ordered batches (based on marker), and then skip all tests in subsequent batches if a batch fails (i.e. allowing you to run integration tests only if the unit tests passed).
