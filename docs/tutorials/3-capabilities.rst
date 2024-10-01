==================================
Use capabilities to control access
==================================


.. warning:: This tutorial is under development


Now that you can upload and download files, you may want to invite others to read some of that data.

Mutable vs. Immutable
======================


DIR2 cap for browsing directories
=================================


CHK for reading files
=====================


Table of capabilities
=====================

From https://tahoe-lafs.org/trac/tahoe-lafs/wiki/Capabilities

.. code-block::

     1: immutable file read-only capability string            URI:CHK:
     2: immutable file verify capability string               URI:CHK-Verifier:
     3: immutable LIT file read-only capability string        URI:LIT:

     4: mutable file read-write capability string             URI:SSK:
     5: mutable file read-only capability string              URI:SSK-RO:
     6: mutable file verify capability string                 URI:SSK-Verifier:

     7: immutable directory read-only capability string       URI:DIR2-CHK:
     8: immutable directory verify capability string          URI:DIR2-CHK-Verifier:
     9: immutable LIT directory read-only capability string   URI:DIR2-LIT:

    10: mutable directory read-write capability string        URI:DIR2:
    11: mutable directory read-only capability string         URI:DIR2-RO:
    12: mutable directory verify capability string            URI:DIR2-Verifier:

