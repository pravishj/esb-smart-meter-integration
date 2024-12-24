[![hacs_badge](https://img.shields.io/badge/HACS-Default-41BDF5.svg?style=for-the-badge)](https://github.com/hacs/integration)

# ESB Smart Meter integration for Home Assistant

Inspired by [https://github.com/badger707/esb-smart-meter-reading-automation](https://github.com/RobinJ1995/home-assistant-esb-smart-meter-integration)

## Pre-Requirements

- Account at https://myaccount.esbnetworks.ie/
- Your meter's MPRN

## HACS Installation

[![Open your Home Assistant instance and open a repository inside the Home Assistant Community Store.](https://my.home-assistant.io/badges/hacs_repository.svg)](https://my.home-assistant.io/redirect/hacs_repository/?owner=pravishj&repository=esb-smart-meter-integration&category=integration)

This is the recommended way to install.

1. Search for `esb-smart-meter-integration` follow the steps here [HACS](https://www.hacs.xyz/docs/faq/custom_repositories/).
2. Install.
3. Restart Home Assistant.
4. In the HA UI, click Settings in the left nav bar, then click "Devices & Services". By default you should be viewing the Integrations tab. Click "+ Add Integration" button at bottom right and then search for "esb-smart-meter-integration".
5. In the popup, enter your ESB account's username, password, and MPRN

## Manual Installation

1. Using the tool of choice open the directory (folder) for your HA configuration (where you find `configuration.yaml`).
2. If you do not have a `custom_components` directory (folder) there, you need to create it.
3. In the `custom_components` directory (folder) create a new folder called `esb-smart-meter-integration`.
4. Download _all_ the files from the `custom_components/esb-smart-meter-integration/` directory (folder) in this repository.
5. Place the files you downloaded in the new directory (folder) you created.
6. Restart Home Assistant.
7. In the HA UI, click Settings in the left nav bar, then click "Devices & Services". By default you should be viewing the Integrations tab. Click "+ Add Integration" button at bottom right and then search for "esb-smart-meter-integration".
8. In the popup, enter your ESB account's username, password, and MPRN


If all went well, you should now have the following entities in Home Assistant:
- `sensor.esb_electricity_usage_today`
- `sensor.esb_electricity_usage_last_24_hours`
- `sensor.esb_electricity_usage_this_week`
- `sensor.esb_electricity_usage_last_7_days`
- `sensor.esb_electricity_usage_this_month`
- `sensor.esb_electricity_usage_last_30_days`
