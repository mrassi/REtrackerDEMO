# REtrackerDEMO

RealSense Tracker by RASSI ENGINEERING

(Demo version: only supports Roll Pitch Yaw) 
For full product contact Rassi Engineering +9613341934 or marwan@rassi.me)

1- You will need a [Realesense T265 that you can purchase here](https://store.intelrealsense.com/buy-intel-realsense-tracking-camera-t265.html)

2- Download and install [latest sdk from realsense](https://github.com/IntelRealSense/librealsense/releases/download/v2.42.0/Intel.RealSense.SDK-WIN10-2.42.0.2845.exe)

3- run `RE_sensordetect.exe` (this will read your unique T265 serial number and will store it under `serial.txt`)

4- email `serial.txt` to marwan@rassi.me or mrassi@gmail.com

5- after email is received, we will email back your key (place `key.txt` in the same directory)

6- edit `remote_address.txt` with your aximmetry ip address (or local 127.0.0.1 if on the same PC) 

7- run `REtrackerDemo.exe`


# Aximmetry setup

1- go to manage devices > OSC server > select ip address > and set port to 7000 

2a- Open `./aximmetry tools/sample_project.xcomp` and replace test input video and Unreal Engine file

2b- or use `./aximmetry tools/REtrackerServer.xcomp` and connect output to any camera transform node

3- for advanced users: you can use `./aximmetry tools/REtracker_LensDistort_JSON.xcomp` after calibrating lense with `RE_calibrate.exe` and generating a distortion matrix JSON file (contact us for free calibration tools)