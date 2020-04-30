============
Monitors
============

Monitors are the way to see the status of an IP/Domain. Here is a simple guide on everything about them. If you need anyhelp, feel free to Join our Discord: https://discord.gg/HvJ4hSA

.. WARNING:: You need to be an admin on the guild to create/manage monitors.

Viewing Monitors
================
- Overview of all monitors
For a quick overview of all the monitors on your guild, run:

.. code-block:: none

    sb!monitors


This will show you every monitor on your guild, along with the Status, ID & Name of the monitors.

- View Individual monitors
To view a individual monitor, you can run:

.. code-block:: none

    sb!monitor <monitor id>


Running this command will provide more information on the monitor.

.. note:: 
    You get the **<monitor id>** from running the *monitors* command.

Creating Monitors
=================
- Create a monitor
To create a monitor simply run the following:

.. code-block:: none

    sb!create


The bot will prompt you with questions to setup the monitor.

Configuring Monitors
====================
- Configuring Monitors
When configuring a monitors settings, the base syntax is:

.. code-block:: none

    sb!monitor <monitor id> <setting> <new value>


.. note::
    The **<new value>** doesn't have to be there for all settings.


The following tables will provide information on each setting.

.. note::
    All settings are case insensitive in commands


+---------+---------------------+-----------------------------------+-----------------------------------------------+
| Setting | New Value Required? | Posible new values                | Description                                   |
+=========+=====================+===================================+===============================================+
| name    | Yes                 | Any string                        | The name of the monitor                       |
+---------+---------------------+-----------------------------------+-----------------------------------------------+
| ip      | Yes                 | Any valid domain or ip address     | The domain or ip of the monitor               |
+---------+---------------------+-----------------------------------+-----------------------------------------------+
| domain  | Yes                 | Any valid domain or ip address     | The domain or ip of the monitor               |
+---------+---------------------+-----------------------------------+-----------------------------------------------+
| enabled | No                  | Any value inputed will be ignored | Toggle wether the monitor is enabled or not   |
+---------+---------------------+-----------------------------------+-----------------------------------------------+
| enable  | No                  | Any value inputed will be ignored | Enable the monitor                            |
+---------+---------------------+-----------------------------------+-----------------------------------------------+
| disable | No                  | Any value inputed will be ignored | Disable the monitor                           |
+---------+---------------------+-----------------------------------+-----------------------------------------------+
| hidden  | No                  | Any value inputed will be ignored | Toggle wether the monitor ip is hidden or not |
+---------+---------------------+-----------------------------------+-----------------------------------------------+


Premium Settings: These settings are only avaliable to premium guilds
"""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""

+----------------+---------------------+----------------------------------------------------+------------------------------------------------------------+
| Setting        | New Value Required? | Posible new values                                 | Description                                                |
+================+=====================+====================================================+============================================================+
| footer         | Yes                 | Any string                                         | The footer of the monitor embed                            |
+----------------+---------------------+----------------------------------------------------+------------------------------------------------------------+
| online title   | Yes                 | Any string                                         | The title of the embed, when the status is online          |
+----------------+---------------------+----------------------------------------------------+------------------------------------------------------------+
| online color   | Yes                 | A valid hexadecimal color in the form of "#af35bc" | The sidebar color of the embed, when the status is online  |
+----------------+---------------------+----------------------------------------------------+------------------------------------------------------------+
| offline title  | Yes                 | Any string                                         | The title of the embed, when the status is offline         |
+----------------+---------------------+----------------------------------------------------+------------------------------------------------------------+
| offline color  | Yes                 | A valid hexadecimal color in the form of "#af35bc" | The sidebar color of the embed, when the status is offline |
+----------------+---------------------+----------------------------------------------------+------------------------------------------------------------+


Deleting Monitors
=================
- Deleting a monitor
To delete an individual monitor run the following:

.. code-block:: none

    sb!delete <monitor id | monitor name>


.. note::
    **|** means "or"


- Deleting all the monitors
To delete all monitors run the following


.. code-block:: none

    sb!delete all
