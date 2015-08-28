Django Discover Slowtest Tests Runner
========================
.. image:: http://slack.pinaxproject.com/badge.svg
   :target: http://slack.pinaxproject.com/

.. image:: https://img.shields.io/travis/realpython/django-discover-slowest-tests-runner.svg
    :target: https://travis-ci.org/realpython/django-discover-slowest-tests-runner

.. image:: https://img.shields.io/coveralls/realpython/django-discover-slowest-tests-runner.svg
    :target: https://coveralls.io/r/realpython/django-discover-slowest-tests-runner

.. image:: https://img.shields.io/pypi/dm/django-slowtests.svg
    :target:  https://pypi.python.org/pypi/django-slowtests/

.. image:: https://img.shields.io/pypi/v/django-slowtests.svg
    :target:  https://pypi.python.org/pypi/django-slowtests/

.. image:: https://img.shields.io/badge/license-MIT-blue.svg
    :target:  https://pypi.python.org/pypi/django-slowtests/
    

Pinax
-------

Pinax is an open-source platform built on the Django Web Framework. It is an ecosystem of reusable Django apps, themes, and starter project templates. 
This collection can be found at http://pinaxproject.com.


django-discover-slowtest-tests-runner
---------------------------------------

``django-discover-slowtest-tests-runner`` lets you locate your slowest tests.


Getting Started
----------------

1. Install::

    $ pip install django-slowtests

2. Add the following setting::

    TEST_RUNNER = 'django-slowtests.DiscoverSlowestTestsRunner'

3. Run test suite::

    ./manage.py test

4. Sample output::


    $ python manage.py test
    Creating test database for alias 'default'...
    ..........
    ----------------------------------------------------------------------
    Ran 10 tests in 0.413s

    OK
    Destroying test database for alias 'default'...

    Ten slowest tests:
    0.3597s test_detail_view_with_a_future_poll (polls.tests.PollIndexDetailTests)
    0.0284s test_detail_view_with_a_past_poll (polls.tests.PollIndexDetailTests)
    0.0068s test_index_view_with_a_future_poll (polls.tests.PollViewTests)
    0.0047s test_index_view_with_a_past_poll (polls.tests.PollViewTests)
    0.0045s test_index_view_with_two_past_polls (polls.tests.PollViewTests)
    0.0041s test_index_view_with_future_poll_and_past_poll (polls.tests.PollViewTests)
    0.0036s test_index_view_with_no_polls (polls.tests.PollViewTests)
    0.0003s test_was_published_recently_with_future_poll (polls.tests.PollMethodTests)
    0.0002s test_was_published_recently_with_recent_poll (polls.tests.PollMethodTests)
    0.0002s test_was_published_recently_with_old_poll (polls.tests.PollMethodTests)



Running the Tests
------------------------------------

You can run the tests with via::

    python setup.py test

or::

    make test

or::

    make all

or::

    python runtests.py
    

Documentation
--------------

The Pinax documentation is available at http://pinaxproject.com/pinax/.


License
-------

This code is distributed under the terms of the MIT license. See the `LICENSE` file.


Code of Conduct
----------------

In order to foster a kind, inclusive, and harassment-free community, the Pinax Project has a code of conduct, which can be found here  http://pinaxproject.com/pinax/code_of_conduct/.


Pinax Project Blog and Twitter
-------------------------------

For updates and news regarding the Pinax Project, please follow us on Twitter at @pinaxproject and check out our blog http://blog.pinaxproject.com.


