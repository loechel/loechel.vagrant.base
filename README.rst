===================
Vagrant Base Config
===================

This Repository did not reflect any production environment.
It is used for an overall documentation and some helpers regarding Vagrant used by myself.

Use Cases
=========

Documentation of prefered Vagrant Boxes
---------------------------------------



Global Update of Vagrant Boxes
------------------------------


Provisioning
------------


Ansible
~~~~~~~


Shell
~~~~~



Usage
=====

Requirements
------------

* git
* Vagrant (tested on Vagrant 1.9.x, https://www.vagrantup.com/)
* Ansible (2.0+, https://www.ansible.com/)

Your implicit requirements for this setup is:

* for Vagrant / used Vagrant base box:

  * A 64 bit Processor
  * A vPro enabled System / Processor (Intel I5/I7/I9, or AMD) so that you could use 64 bit guests
  * Virtualbox (https://www.virtualbox.org/)

* for Ansible:

  * An Unix complied Environment (Linux, Mac OS, *BSD)
  * Python 2

Setup
-----

.. code:: bash

    git clone https://github.com/loechel/loechel.vagrant.base.git vagrant.base
    cd vagrant.base

How to Contribute
=================

If you want to contribute to this vagrant environment please contact me at Alexander.Loechel@lmu.de and tell me your github account, so that I could add you to the allowed contributers list.
