# wake-on-lan
scheduled wake on lan when a specific device is connected to the network  


This code uses the subprocess module to run the ping command to check if the device with IP address IP_DEVICE is connected to the network. It uses the wakeonlan library to send a magic packet to the device's MAC address, which is specified in the devices dictionary.

The runscript() function is defined to run the ping command and check for the device's IP address in the output. If the device is connected, the script sends a magic packet to the device's MAC address and prints 'Device connected!' to the console.

Finally, the script uses the schedule library to run the runscript() function every day at 16:28. The script enters an infinite loop, where it checks if there are any scheduled tasks to be run and sleeps for 1 second.

This script is designed to run the ping command every day at 16:28, if the device is connected, it sends the magic packet, otherwise, it will keep running the ping command until the device is connected.

You may want to adjust the schedule time and the IP address, MAC address and name of the device according to your needs.

Also, please note that, this script is using the wakeonlan library which is not a built-in library, you need to install it before running the script!!!!

If you want to run it on a phone on pydroid3 there are some changes that are needed head over to the other github page i have about that and download the code from there.

https://github.com/590ms/wake-on-lan-pydroid3
