.. title: Ganga - the job management tool
.. date: 2016-02-25 12:44:48 UTC
.. link: 
.. description: 
.. type: text
.. hidetitle: True

.. raw:: html

    <div class="jumbotron">
        <div class="container">
            <h1>Ganga - the job management tool</h1>
            <p>In goes content, out comes a website, ready to deploy.</p>
            <p>
                <a class="btn btn-primary btn-lg get-started" href="/getting-started.html" role="button">Get started with Ganga »</a>
                <a class="btn btn-default btn-lg" href="/features/index.html" role="button">Learn about Ganga features »</a
            </p>
            <p><small>Ganga is written in Python. Free open-source software under the <a href="/license.html">GPL2+ license</a>.</small></p>
        </div>
    </div>

.. container:: row

    .. container:: col-md-6

        .. code-block:: python

            j = Job()
            j.submit()
            j.peek('stdout')

        Interacting with Ganga jobs can be as easy as threee lines.
        By default all process will run on your local computer.

    .. container:: col-md-6

        .. code-block:: python

            j = Job()
            j.application.exe = 'my-analysis.sh'
            j.application.args = ['360', '0.1']
            j.submit()

        Everything is configurable and allows you to change how it works.

.. container:: row

    .. container:: col-md-6

        .. code-block:: python

            j = Job()
            j.backend = PBS()
            ...
            j.submit()

        Running your code elsewhere is as simple as changing a single line in your code.
