Role Name
=========

x708

Role to manage Geekworm's x708 Raspberry Pi UPS.

Role feature
------------

* Install power button scripts to perform safe reboot and shutdown
* Install fan script to control speed based on temperature

Requirements
------------

* ansible >= 2.14.x

Role Variables
--------------

* x708_rebootpulseminimum[200]: mininum pulse width, button pressed, required to perform shutdown
* x708_rebootpulsemaximum[600]: maximum pulse width, button pressed, required to perform shutdown


Dependencies
------------

Raspberry Pi OS Bullseye:
  * 
Raspberry Pi OS Bookworm
  * 

Example Playbook
----------------

    - hosts: raspberrypi
      roles:
        - name: Enable usage of x708 
          roles:
            - name: x708
License
-------

BSD

Author Information
------------------

https://github.com/j3ffrw
