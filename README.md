# Akaki Pipe Chair Cockpit
3D printable flight stick and pedals with minimal hardware. Great for Condor 2 and other VR gliding simulators.

![3D render](pipechair%20cockpit%20render.png?raw=true)

Video: https://www.youtube.com/watch?v=8db8fcycaJI

Features a robust joystick gimbal that only needs 608 "skate" bearings and no other hardware. Instead of metal bolts, it uses 3D printed dowels.

The frame and the stick shaft are 18 mm PVC pipe. The whole device clips onto a pipe chair.

The stick head is styled like a glider stick.

Stick motion is sensed with either bare Hall effect sensor components, or TLE5010/11 digital magnetoresistive sensors. Other axes are sensed with the common potentiometer. I recommend the MMJoy2 firmware and an Arduino Micro to manage the USB device.

# Build steps

The inner frame of the gimbal must be assembled in a specific order:
* Insert 608 bearings in the cam elements and gimbal frame (8 locations in total)
* Insert a dowel and the 2 mm printed washer to the right-hand side of the shaft mount. Let it extend about 20 mm
* Slide the above dowel into the bearing in the U-shaped piece of the inner gimbal frame
* Slide the left side side of the inner gimbal frame into place. It needs to bend a little to get into position
* Slot in the remaining piece of the inner frame
* Insert dowels in all 6 available locations The dowel through the bearing on the left side of the inner frame will complete the Y axis shaft. The four dowels in the round "ears" will receive the cams
After this you can add the cams and the cam follower bearings, and assemble the outher frame around it

To be updated

# License

CC BY 4.0 https://creativecommons.org/licenses/by/4.0/
