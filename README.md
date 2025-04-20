# Orange Pi 3B PWM fan control
Controller for controlling the fan speed (2 pin PWM) depending on the SOC temperature for OrangePi 3B

Tested and works on DietPi v9.12 (Debian Bookworm), kernel 6.12.7-current-rockchip64 , rk3566-orangepi-3b.dtb - orangepi-xunlong.

### 1. Make an opi5p-pwm executable file
``chmod +x fancontrol``

and copy it to /usr/local/bin/
### 2. Create and launch a service
Copy the pwm-fan.service file to /usr/lib/systemd/system

And execute to run this service:

``# systemctl enable --now pwm-fan.service``

