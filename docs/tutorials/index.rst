=========================
The Tahoe Operator Guide
=========================

About this guide
================

    There are many ways to get started with Tahoe-lafs. This one works.
    -- Anonymous

This series is for newcomers to Tahoe-lafs who want to get familiar with the pieces of Tahoe-lafs and prefer a step-by-step approach to the All-in-One alternative.
If you are new to Tahoe, these docs will give you a concrete experience operating Tahoe. Each section provides exercises, expanding on the previous examples, so that you can:

    - build a working Tahoe-lafs deployment
    - practice using the CLI
    - understand the purpose, capabilities and limitations of each feature.

.. note:: The complete series takes about 1 hour


.. toctree::
    :titlesonly:
    :caption: The step-by-step guide to operating Tahoe

    0-storage-node
    1-client-node
    2-availability
    3-capabilities
    4-scaling


Before you begin
================

Create and activate a local venv for tahoe::

    python -m venv .venv && source .venv/bin/activate

Update the new venv and install tahoe-lafs::

    pip install -U pip setuptools wheel && \
    pip install attrs==23.2.0 'cryptography<42' tahoe-lafs

.. note:: Use multiple terminal sessions for each of the various consoles you will eventually start. Most IDE's support independent terminals.

``tmux`` is your friend
-----------------------

Most Tahoe operators are running Linux in terminal sessions. Using ``tmux`` will make life easier because you will be running several processes, it helps to have multiple terminal windows.
A Linux terminal user would create several sessions like this::

    $ tmux new -s storage_console
    $ tmux new -s client_console



Cookbook recipes
================

These guides provide instructions for specific solutions built on top of Tahoe-lafs.
In most cases they will have external dependencies because they aim to integrate with other services.
Read through to determine how relevant they may be to your use case.

.. toctree::
    :titlesonly:
    :caption: Tahoe Scenarios by Example

    Example: Private Sharing & Sync of Files <7-magicfolder>
    Example: User control of private data <8-app-storage>
    Example: Tahoe as a backup server <9-backup>

