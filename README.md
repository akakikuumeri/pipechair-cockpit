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

# Wiring the pedal potentiometers

You can use a single potentiometer on just one of the pedals. The pedals are linked to move together, so it is enough to measure just one of them. However, the PVC pipe frame can bend if you press on both pedals at the same time, and give you a false reading on the rudder axis. To prevent this, you can wire two identical potentiometers in a differential configuration ( https://github.com/akakikuumeri/pipechair-cockpit/blob/main/pedals%20wiring%20diagram.jpeg ). This way the potentiometers cancel out any movement that happens on both pedals in the same direction, and only ouput the difference between them.

Pay attention to the order of GND and 5V wires. When installed on the pedals, one pot should have the GND on the top and one on the bottom. https://github.com/akakikuumeri/pipechair-cockpit/blob/main/pedals%20wiring%20photo.jpg

Notice that if the two potentiometers are moved all the way in one direction (both pedals pushed all the way back or all the way forward) this wiring might short out the GND and 5V pins. To protect your electronics from this unlikely risk, you can add two small resistors on the wiper pins of the potentiometers as in the diagram. I used 47 Ohm reistors, any value that is large enough to prevent a large current in case of a short, and small enough compared to the potentiometer resistance, is fine (10 to 100 Ohms perhaps).


# License

CC BY 4.0 https://creativecommons.org/licenses/by/4.0/
