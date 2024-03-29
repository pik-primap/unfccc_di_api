.. highlight:: shell

============
Contributing
============

Contributions are welcome, and they are greatly appreciated! Every little bit
helps, and credit will always be given.

You can contribute in many ways:

Types of Contributions
----------------------

Report Bugs
~~~~~~~~~~~

Report bugs at https://github.com/pik-primap/unfccc_di_api/issues.

If you are reporting a bug, please include:

* Your operating system name and version.
* Any details about your local setup that might be helpful in troubleshooting.
* Detailed steps to reproduce the bug.

Fix Bugs
~~~~~~~~

Look through the GitHub issues for bugs. Anything tagged with "bug" and "help
wanted" is open to whoever wants to implement it.

Write Documentation
~~~~~~~~~~~~~~~~~~~

UNFCCC DI API could always use more documentation, whether as part of the
official UNFCCC DI API docs, in docstrings, or even on the web in blog posts,
articles, and such.

Submit Feedback
~~~~~~~~~~~~~~~

The best way to send feedback is to file an issue at
https://github.com/pik-primap/unfccc_di_api/issues.

If you are proposing a feature:

* Explain in detail how it would work.
* Keep the scope as narrow as possible, to make it easier to implement.
* Remember that contributions are welcome :)

Get Started!
------------

Ready to contribute? Here's how to set up `unfccc_di_api` for local development.

1. Fork the `unfccc_di_api` repo on GitHub.
2. Clone your fork locally::

    $ git clone git@github.com:your_name_here/unfccc_di_api.git

3. Install your local copy into a virtualenv. Assuming you have virtualenvwrapper
   installed, this is how you set up your fork for local development::

    $ cd unfccc_di_api/
    $ make virtual-environment
    $ make install-pre-commit

4. Create a branch for local development::

    $ git checkout -b name-of-your-bugfix-or-feature

   Now you can make your changes locally.

5. When you're done making changes, check that your changes pass our tests and
   automatically format everything according to our rules::

    $ make lint

    Often, the linters can fix errors themselves, so if you get failures, run
    ``make lint`` again to see if any errors need human intervention.

6. Commit your changes and push your branch to GitHub::

    $ git add .
    $ git commit -m "Your detailed description of your changes."
    $ git push origin name-of-your-bugfix-or-feature

7. Submit a pull request through the GitHub website.

Pull Request Guidelines
-----------------------

Before you submit a pull request, check that it meets these guidelines:

1. The pull request should include tests.
2. If the pull request adds functionality, the docs should be updated. Put
   your new functionality into a function with a docstring, and add the
   feature to the list in README.rst.
3. The pull request should work for Python 3.9, 3.10, 3.11, and 3.12.


Deploying
---------

.. highlight:: shell

A reminder for the maintainers on how to deploy.

1.  Commit all your changes.
2.  Replace the unreleased entry in CHANGELOG.rst with your target version number.
3.  Run ``tbump X.Y.Z``.
4.  Go to github and make a release from the tag.
    Use "Version x.y.z" as the release title, and the changelog entries as the release
    description.
    Creating the github release will automatically trigger
    a release on zenodo.
5.  Run ``make update-citation`` to update the citation information in the README.
6.  Upload the release to pyPI: ``make release``
7.  To prepare for future development, add a new "unreleased" section to CHANGELOG.rst,
    and commit the result.
