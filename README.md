## Venus OS Temperature Service
### Fork from LHardwick and Rikkert-RS Victron-Service

This is a service to publish temperature type data onto the DBus of VenusOs running on a Raspberry Pi device.  
Note: Currently this will not display the CPU temperature on Venus GX, only on RPi.

Added Support to install this with Kevin Windrem's Venus OS Setup Helper (https://github.com/kwindrem/SetupHelper)

## INSTALL INSTRUCTIONS
No Settings needed for 1 Wire (e.g. DS18B20) all you need is to install SetupHelper and configure a custom Package.
  - Package name: VenusOS-TemperatureService
  - GitHub user: philip-s
  - GitHub Tag: latest

      ### Screenshots
      <details><summary>Add Custom Package</summary>

      ![PackageManager Menü](/screenshots/PackageManagerMenu.png)
      ![Add Custom Package ](/screenshots/PackageManagerAddPackage.png)
      ![Fill Custom Package](/screenshots/PackageManagerAddCustomPackage.png)
      ![Install Package](/screenshots/PackageManagerInstallAktivPackage.png)

</details>

### Enabled Features in this Setup:
  - 1-Wire Support (Temperatures) Data Port GPIO 26 on RPi. 
  - Raspberry CPU temperature has been removed as it's not necessary for campers. If you need CPU temperature install the Rikkert-RS version: https://github.com/Rikkert-RS/VenusOS-TemperatureService

### Can be activated but not tested (in dbus-i2c.py)
  - i2c Sensors
  - ADC Sensors

Tested on Rasberry 3+ with Venus OS 2.91

### Own Services:
 Note, only services of path type "Temperature" will be displayed on the console and VRM
 If you modify the service to pubish data as a path that is of a different type
 it will only be available via the DBus and will not appear on the console or VRM.

![Temps in Venus OS Menu](/screenshots/TempsInMenu.png)

Hope this all works for you

Rikkert-RS
