# TrackingAntenna
Code for controlling the tracking antenna. (Currently an arduino)

An arduino controls 2 servos for plane tracking (pan and tilt). 
Communication from the xbee if achieved with an ethernet shield. 
There is a simple debug interface through serial.

Quick setup guide:

1. set INITIALISATION to 0.
2. be careful when the code uploads as the antenna may swing unpredictably.
3. turn the base of the antenna to point eastish
4. at this point you can verify the antenna is recieving telemetry data. set DEBUG to 1 and open arduino serial monitor
5. hold the plane next to the antenna, and update the INITIAL_LATTITUDE, INITAL_LONGITUDE, INITIAL_ALTITUDE.
6. set INITIALISATION TO 1. again be careful about the unpredictabe swing.
7. put the plane on the runway, some distance away from the antenna is needed for fine tunning the angle.
8. rotate the base of the antenna until it point at the plane. it should already have been decently close. 
9. check the altitude (tilt) seems correct.
10. check there are no wire to snag as it rotates.
