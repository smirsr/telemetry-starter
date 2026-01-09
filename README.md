# telemetry-starter
a monitoring system for a robot/vehicle

robots are cosntantly producing numbers , these numbers are called telemtry:

1. generate telemtry with a simulator 
2. log it 
3. detect important events like getting too close or hard brake and save the events 
4. make visual 

this is good for engineers to monitor behaviour.

phase 1 : core logger (no api )
inputs : speed,battery,distance_front , acceleration 
1. print telemetry to terminal 
2. save telemtry to csv 
3. detect events -> save to csv
4. make plot 
we have tow different modes: 
 mode A: robot rover: 
 speed,battery,distance_front,accel, mode
 events : tooclose, lowettery
Mode B: automated Vehicle:
speed,battery/fuel,following_distance,accel
events : tailgating,hardbrake,lowbattery

phase 2 : api : turning logger into data service 

adding an api so that dashboard can ask about whats going on 

phase 3: visual dashboard (no react)
possible upgrade : react for better ux and it looks real

phase 4 : deployment + polish 
