Developer Guide
===============


Pre-commit Checks
-----------------

This project is configured for use with `pre-commit`_ to install `VCS/git hooks`_ which perform some static code analysis checks and other code checks to catch common errors.
These hooks can be configured to run before commits or pushes

For example::

    $ pre-commit install --hook-type pre-push
    pre-commit installed at .git/hooks/pre-push
    

.. _`pre-commit`: https://pre-commit.com
.. _`VCS/git hooks`: `pre-commit`_
.. _`pre-commit configuration`: ../.pre-commit-config.yaml
