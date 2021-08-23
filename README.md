Adafruit Ultimate GPS Role
=========

Configures a Raspberry Pi for use with an Adafruit Ultimate GPS HAT.

The HAT uses the Pi's UART interface for communication with the Pi itself, and as such, requires the Pi to be configured so that serial communication is disabled, so the required pins are available for use.

Tested and used with a Raspberry Pi 4, however it should work across all of the various Pis that the HAT supports.

Requirements
------------

- An [Adafruit Ultimate GPS HAT](https://www.adafruit.com/product/2324)

Example Playbook
----------------

    - name: Setup Adafruit Ultimate GPS module
        hosts: all
        become: yes
        roles:
            - adafruit_ultimate_gps


License
-------

BSD
