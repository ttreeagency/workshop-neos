*******************
TYPO3 Neos Workshop
*******************

This repository contain a basic Debian Wheezy preconfigured for TYPO3 Neos Workshop

============
Installation
============

.. code-block:: bash

    $ vagrant up

---------------------------------
Vagrant Shared folder performance
---------------------------------

By default the Vagrantfile is configured to use NFS shared folder for performance. Unfortunatly NFS shared folder are not supported on Windows.

For Windows user you can check SMB shared folder here: https://docs.vagrantup.com/v2/synced-folders/smb.html or WinNFSD plugin here: https://github.com/GM-Alex/vagrant-winnfsd. 

By default vagrant will fall back to the default shared folder. That's really slow, but works.

=====================
Network configuration
=====================

Edit your host file:

.. code-block::

 	192.168.77.21 www.neos-workshop.box neos-workshop.box

=================
Open your browser
=================

Open your browser to http://neos-workshop.box/

You should see a PHP Info page ... let's start the workshop

Bests,