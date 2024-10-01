===========
Make a grid
===========

.. warning:: This is a placeholder for an upcoming tutorial

Now, we extend the section of availability by creating and joining a :term:`grid`

Clients need to find storage
============================

Updating client configs is a pain
Storage nodes may go offline


Introducer nodes keep track of storage
======================================

Instead of updating each client, use the fURL of the introducer.
Clients then need only one location to find storage.
This is similar to the way DNS clients work.

Create the introducer node
==========================

.. code-block::

    tahoe --node-directory=introducer0 create-client \
        --shares-happy=1 \
        --shares-needed=1 \
        --shares-total=1 \
        --web.port=3457 \
        --nickname=introducer0


.. note:: Hooray! we can finally use that response  ``Please add introducers to ...``

Start the introducer node
=========================

To create the fURL, we need to start the introducer, so that we can::

    Please add introducers to '/Users/bpabon/src/repos/tahoe/tahoe-lafs/docs/examples/introducer0/private/introducers.yaml'!

Create ``private/introducers.yaml``


The introducer fURL
===================

 provides introduction services and nothing else.
When started, this node will produce a private/introducer.furl file, which should be published to all clients.



.. note:: Congratulations, you now have a working Tahoe grid