##Model of traffic

This program simulates the actions of drivers and the situation on the road, depending on the current traffic lights.

##Beginning of the game
To run the game you need to run the file ~start.rb.

```
$ ruby start.rb
```


###Road

You are asked to choose the state of the road:

1. dry coating (provides minimum braking distance)
- wet coating (braking distance almost doubles)
- trampled snow (increases braking distance by almost four times)
- ice cover (maximum stopping distance)


###Traffic light

Then you choose the traffic light mode:

1. Automatic mode. The traffic light operates according to the preset mode.
- User mode. For each color, the on time is set.
- emergency mode. The colors and the response time are selected randomly (the cycle is three times the traffic light)

###Adding vehicles to the road

After the traffic light mode is selected, you are asked to add vehicles (TC) to the road. There are 4 ready-made options available. Also you can enter your own TC parameters.

In the event that the vehicle does not manage to stop (the braking distance exceeds the sum of the preferred distance and the braking distance of the vehicle ahead), the emergency case will fail. An alarm is displayed and you are prompted to either abort the game or continue. In the second case, the damaged vehicles are removed from the road and the game completes the cycle.

###Modeling an emergency

To achieve the onset of an emergency, you can reduce the distance to the front of the car, as well as increasing the reaction time of the driver to the situation on the road (traffic light signals).
