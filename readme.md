## Hardware
Any embedded linux device which meets the following requirements can be used:
- 2 CAN Controllers (integrated or external)
- 2 I2C Bus
- 5 GPIO Pins

Although LPBs Firmware is tested and developed on Beaglebords Beaglebone Black, any device
which fullfills the listed requirements can be used as a coordinator node.

## Go Dependencies
LPBs functionality depends partially on external provided community modules.
Before installing lpb on your device fetch the following dependencies with go-get:
- Cobra (https://github.com/spf13/cobra)
- Viper (https://github.com/spf13/viper)
- Socket Can (https://github.com/brutella/can)

## MYSQL Setup
After installing mysql may dont allowing access to DB with root.
This can be fixed by login into mysql (mysql -u root) and changing the default password(ALTER USER 'root'@'localhost' IDENTIFIED WITH mysql_native_password BY 'newpw';)