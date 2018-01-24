# SimSteeringTest
This is a DirectInput demo that is designed to test the force feedback steering.  This is an example from Microsoft Corporation with modification to use the spring force to turn the wheel.


This is stricly for testing SimSteering with DirectInput

I have created a few commits at various stages to improve understanding on what is going on.  

I am currently using logitech G27 Wheel with this code and it works fine.  I'm able to get the full 900 degrees of turning.

The current state allows users to click the left and right side of the input box to turn the wheel to a givin position.  This should max out -450 to 450 degrees.  At this time it seems I get halve that with SimSteering. 

The previous commit's have been using a constant force.  This has produced a very diffrent reaction.  This would seem to bounce back in fourth instead of apply a constant force in one direction.  I have been able to reduce the force and cause it to move slowly and get more of an intened effect.  The plan is to use this to match the wheel position with an automated driving simulation.  We want the wheel to match the wheel position in the simulation.  At this point the lowered force value would cause the wheel to move to slowly into positon.  I would ask the question if I apply a force in a given direction why would it bounce back? 
