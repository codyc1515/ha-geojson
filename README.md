![GeoJSON](https://brands.home-assistant.io/geo_json_events/logo.png)

# GeoJSON Properties integration for Home Assistant
This is a GeoJSON custom component for Home Assistant that exposes the `properties` within your GeoJSON file.

## Getting started
This makes the GeoJSON integration actually useful for me because I can now use it for checking, among other things:

* Community Incidents
* Power Outages
* Water Chlorination
* Water Outages

### Example of water outages
Use the GeoJSON URL - https://smartview.ccc.govt.nz/app/router/map_features.php?feat=watershutoffs - and you will see in HA:

![image](https://github.com/home-assistant/core/assets/50791984/be8b17a8-a956-4e3a-8209-4bc318b11d74)

## Installation
### HACS (recommended)
1. [Install HACS](https://hacs.xyz/docs/setup/download), if you did not already
2. [![Open your Home Assistant instance and open a repository inside the Home Assistant Community Store.](https://my.home-assistant.io/badges/hacs_repository.svg)](https://my.home-assistant.io/redirect/hacs_repository/?owner=codyc1515&repository=ha-geojson&category=integration)
3. Install the GeoJSON Properties integration
4. Restart Home Assistant

### Manually
Copy all files in the custom_components/geo_json_events folder to your Home Assistant folder *config/custom_components/geo_json_events*.

## Known issues

- This integration overrides the HA Core `geo_json_events` integration which means any updates in HA Core in the future could potentially break this integration or your HA installation. There is a [pending PR to resolve this by integrating the changes in this integration into HA Core](https://github.com/home-assistant/core/pull/107690).

## Future enhancements
Your support is welcomed.

## Acknowledgements
- [exxamalte]([url](https://github.com/exxamalte)), who contributed the original geo_json_events integration to HA Core
