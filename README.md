# vex-lab3

lab 3 robot vex
-A line tracker consists of an infrared light sensor and an infrared LED. It works by illuminating
        a surface with infrared light; the sensor then picks up the reflected infrared radiation and, based
       on its intensity, determines the reflectivity of the surface
-s range of output from zero to five volts is sent to the microcontroller, which
         reads it as a range of integer values from 0 to 255. 
         
-For this particular sensor, sensor output will be low (around 0) when the infrared light bounces
back to the detector - in other words, when the surface is white or highly reflective - and high
(around 255) when the light is absorbed and does not bounce back. You can then set a threshold
value in your code to act as a trigger for behaviors. This sensor can also be used to detect the
presence of a dark or light object

- for example a white color can be followed on a black surface by 
LineFollower
Middle should always see white, and
the other two - LineFollower Left and
LineFollower_Right – should always see
black. If LineFollower_Left starts seeing
white, then your robot needs to steer back
to the left. If LineFollower Right starts
seeing white, then your robot needs to
steer back to the right.
so if the middle and the left sensort be high (225) steer right 
Sensor output will be low (0V) when the infrared light bounces back to the detector – in other
words, when the surface is pale or highly reflective – and high(+5V) when the light is absorbed
and does not bounce back.

HELPFUL HINT:
Because the Line Follower uses an infrared LED to illuminate its target and an infrared
sensor to detect the reflected light, it will actually work in low-light conditions or even in the
dark! However, this also means that it can easily become saturated – in other words,
everything will look white to it, like an over-exposed photograph – in environments where
there is a lot of infrared radiation. You’ll find environments like this in competition settings
where tungsten lights are used for illumination. To avoid saturating the infrared sensor,
consider mounting it underneath the robot or adding a shield to block ambient radiation.
