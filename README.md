## Venus OS Temperature Service
### Fork from LHardwick Victron-Service

This is a service to publish temperature type data onto the DBus of VenusOs running on a Victron GX device.  
Note: Currently this will not display the CPU temperature on Venus GX, only on RPi.

Added Support to install this with Kevin Windrem's Venus OS Setup Helper (https://github.com/kwindrem/SetupHelper)

## INSTALL INSTRUCTIONS
No Settings needed for 1 Wire (e.g. DS18B20) all you need is to install SetupHelper and configure a custom Package.
  - Package name: VenusOS-TemperatureService
  - GitHub user: Rikkert-RS
  - GitHub Tag: latest

### Enabled Features in this Setup:
  - Raspberry Pi CPU temperature
  - 1-Wire Support (Temperatures)

### Can be activated but not tested (in dbus-i2c.py)
  -i2c
  -ADC

Tested on Rasberry 3+ with Venus OS 2.91

### Own Services:
 Note, only services of path type "Temperature" will be displayed on the console and VRM
 If you modify the service to pubish data as a path that is of a different type
 it will only be available via the DBus and will not appear on the console or VRM.

Hope this all works for you 

Rikker-RS
