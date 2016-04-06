Home Assistant Display
======================

`Home Assistant <https://home-assistant.io>`__ ships its own very nice
web frontend. This prototype shows an option to display values without
the possibility of interacting with Home Assistant by the user. 

Installation
------------
It's assumed that your Home Assistant installation is ready before cloning
this repository. Change to your local Home Assistant configuration folder
``.homeassistant`` and clone this repository.

.. code:: bash

    $ git clone https://github.com/fabaff/home-assistant-display.git

In the folder ``www`` you will find an ``index.html`` file and two folders 
with the needed Javascript files and the CSS files.

Setup the `MQTT Eventstream component <https://home-assistant.io/components/mqtt_eventstream/>`__.
The used topic for ``publish_topic`` is ``home/states``. If you change that
then keep in mind to update the topic in the ``index.html`` file as well.

Launch your Home Assistant instance.

.. code:: bash

    $ hass

Now the web site is available at http://[your_hass_host]:8123/local/index.html


Screenshot
----------

|screenshot|

License
-------
``home-assistant-display`` is licensed under MIT, for more details check
LICENSE.

.. |screenshot| image:: https://raw.githubusercontent.com/fabaff/home-assistant-display/master/ha-display.png
   :target: https://github.com/fabaff/home-assistant-display
