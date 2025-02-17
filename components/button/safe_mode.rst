Safe Mode Button
================

.. seo::
    :description: Instructions for setting up buttons that can remotely reboot the ESP in ESPHome into safe mode.
    :image: restart.svg

The ``safe_mode`` button allows you to remotely reboot your node into :ref:`Safe Mode <config-ota>`. This is useful in certain situations
where a misbehaving component is preventing Over-The-Air updates from completing successfully.

This component requires :ref:`OTA <config-ota>` to be configured.

.. figure:: images/safemode-ui.png
    :align: center
    :width: 80.0%

.. code-block:: yaml

    # Example configuration entry
    button:
      - platform: safe_mode
        name: "Living Room Restart (Safe Mode)"

Configuration variables:
------------------------

- **name** (**Required**, string): The name for the button.
- **id** (*Optional*, :ref:`config-id`): Manually specify the ID used for code generation.
- All other options from :ref:`Button <config-button>`.

See Also
--------

- :doc:`shutdown`
- :doc:`restart`
- :doc:`template`
- :apiref:`safe_mode/safe_mode_button.h`
- :ghedit:`Edit`
