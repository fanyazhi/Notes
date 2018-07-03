# Run a Program at Startup (Headless)


Wait for Internet at boot to allow access to internet for the program


```
sudo raspi-config
```

"Boot Options" --> "Wait for Network at Boot" . --> "Yes"

```
sudo nano /home/pi/.bashrc
```
Add after the last line of the script:

```
echo Running at boot 
sudo python /home/pi/sample.py
```
---
More on [Five Ways To Run a Program On Your Raspberry Pi At Startup
](https://www.dexterindustries.com/howto/run-a-program-on-your-raspberry-pi-at-startup/).