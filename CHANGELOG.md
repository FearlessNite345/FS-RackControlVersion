# Changelog v1.3.0
- Fixed racking ACE permission checks to use the racking permission instead of the loadout permission
- Fixed locale load order so `Config.Language` is applied before locale files load
- Fixed `/rack` outside-vehicle handling to respect `Config.AllowRackFromOutsideVehicle`
- Added the missing `/rack` notification when no nearby police vehicle is found
- Made client script load order explicit so helper functions load before client startup logic
- Made the `loadout` command configurable
- Made the `armor` command configurable
- Refactored the weapon racking system to be fully modular, allowing server owners to define and manage any number of rackable weapons via the config
- Refactored the loadout system to be fully modular, allowing server owners to define exactly which weapons and items are granted via the config

# Changelog v1.2.1
- Fixed an issue where unracking could fail due to a misconfigured client-side setting
- Added support for the Lation UI notification system

# Changelog v1.2.0
- Added options to disable the `/loadout` and `/armor` commands if you don’t want them available on your server
- Added ACE permission checks for all commands, allowing you to secure them using entries such as: `add_ace group.admin rackcontrol.loadout allow`

# Changelog v1.1.3

- Temporarily removed the walk-to-trunk feature due to ongoing issues. You can still unrack weapons while outside the vehicle, but there is currently no walking or animation. The feature will be reintroduced once it’s functioning properly.
