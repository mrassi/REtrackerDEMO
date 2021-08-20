# REtrackerDEMO

RealSense Tracker by RASSI ENGINEERING

(Demo version: only supports Roll Pitch Yaw) 
For full product contact Rassi Engineering +9613341934 or marwan@rassi.me)

1- You will need a [Realesense T265 that you can purchase here](https://store.intelrealsense.com/buy-intel-realsense-depth-and-tracking-bundle.html)

2- Download and install [latest sdk from realsense](https://github.com/IntelRealSense/librealsense/releases/download/v2.42.0/Intel.RealSense.SDK-WIN10-2.42.0.2845.exe)

3- clone or download Github directory

4- download tracker software `REtrackerDemo.exe` from [Dropbox](https://www.dropbox.com/s/5f7olf3klzic3jp/REtrackerDemo.exe?dl=0)

5- run `RE_sensordetect.exe` (this will read your unique T265 serial number and will store it under `serial.txt`)

6- email `serial.txt` to marwan@rassi.me or mrassi@gmail.com

7- after email is received, we will email back your key (place `key.txt` in the same directory)

8- edit `remote_address.txt` with your aximmetry ip address (or local 127.0.0.1 if on the same PC) 

9- run `REtrackerDemo.exe`


# Aximmetry setup

1- go to manage devices > OSC server > select ip address > and set port to 7000 

2a- Open `./aximmetry tools/sample_project.xcomp` and replace test input video and Unreal Engine file

2b- or use `./aximmetry tools/REtrackerServer.xcomp` and connect output to any camera transform node

3- for advanced users: you can use `./aximmetry tools/REtracker_LensDistort_JSON.xcomp` after calibrating lense with `RE_calibrate.exe` and generating a distortion matrix JSON file (contact us for free calibration tools)

# Miscellaneous

1- Tested extension cable [from Amazon](https://www.amazon.com/gp/product/B07MZRB6LN)

2- Check the 3D-printable design (mount_t265_d435.stl) for attaching the Realsense with a 1/4 inch screw

# Lens calibration procedure

1- Download Calibration pattern (camera-calibration-checker-board_9x7.pdf)  print it and tape it to a board

2- Follow the Lens Calibration explanation [here](https://github.com/mrassi/REtrackerDEMO/blob/main/Lens%20Calibration%20Tools/Lens%20calibration%20explanation.pdf)

# Brief description

The T265 is an Intel RealSense high precision  tracking sensor. 
We used it to create our own REtracker software. The software is renderer agnostic, meaning it works with all engines. 
You don’t need any markers at the set and you can use it outdoors and indoors. You need to purchase the sensor yourself from Intel website (check readme file)

When we started this project our goals were:
- initial deployment time of less than 10 minutes
- Daily use setup should take less than 2 minutes
- Robust enough for live broadcast
- Ability for use with most engines
- Very easy workflow

you can track 3 cameras simultaneously with the same Aximmetry license on a single PC

The sensor connects to the PC or to a laptop. You can use yany broadcast camera. It is mounted on top of it.
The REtracker software can be installed on any mini pc (i3, 4 GB ram) and the software will send tracking data via Wifi. Or you can connect it directly to the renderer PC.

A set of precision calibration tools is offered in the package as well. 

Sample workflow video: [check video here](https://youtu.be/-iM_Fvp7t80)

Further stuff at my [Youtube page](https://www.youtube.com/user/adorablemarwan)

As for Unreal it works with the native unreal OSC plugin.
 
A Livelink Version for Unreal is in the making, it is still in beta, we will release it soon enough.


The pre-launch price is 2000$/studio.  Meaning you can use the same license for up to 3 cameras (you need one sensor per camera, sensor costs 199$)
We also provide one on one remote support and training. This offer is only available for select customers as we are limiting it to few licenses per region.
Some exceptions are made for Indie companies and the ones whose input help our progress, we sell them single licenses with options to upgrade at a reduced cost.
