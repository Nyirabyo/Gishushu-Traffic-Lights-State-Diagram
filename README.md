# Gishushu-Traffic-Lights-State-Diagram

GISHUSHU Traffic Light Specification 
1.	Up Traffic Light (Controls North-South Traffic):
o	Location: Top of the intersection.
o	Direction: Controls vehicles coming from the south (down side).
o	Movement Allowed:
	North (up)
	Left (west)
	Right (east)
2.	Down Traffic Light (Controls North-South Traffic):
o	Location: Bottom of the intersection.
o	Direction: Controls vehicles coming from the north (up side).
o	Movement Allowed:
	South (down)
	Left (west)
	Right (east)
3.	Left Traffic Light (Controls East-West Traffic):
o	Location: Left side of the intersection.
o	Direction: Controls vehicles coming from the east (right side).
o	Movement Allowed:
	West (left)
	Up (north)
	Down (south)
4.	Right Traffic Light (Controls West-East Traffic):
o	Location: Right side of the intersection.
o	Direction: Controls vehicles coming from the west (left side).
o	Movement Allowed:
	East (right)
	Up (north)
	Down (south)
________________________________________
State Diagram for Traffic Light Cycles
1. State 1: North-South Green
•	Purpose: To allow north-south traffic to move while halting east-west traffic.
•	Behaviour:
o	Vehicles can safely travel north to South and south to west, making turns as permitted.
o	No vehicles can move east or west during this state.
________________________________________
2. State 2: East-West Green
•	Purpose: To allow east-west traffic to move while halting north-south traffic.
•	behaviour:
o	Vehicles can safely travel east to west and west to east, with turns permitted as per the rules.
o	No vehicles can move north or south during this state.
________________________________________
3. State 3: Mixed Alternating Movements (Special Safe Turns)
•	Purpose: To allow selective turns or non-conflicting movements, particularly for minor movements that help clear remaining traffic without causing congestion.
•	behaviour:
o	This state manages small movements to help clear the intersection of residual traffic, allowing minor turns like left turns (north/south) and right turns (east/west).
Possible ways: 
1. North to south and North to East simultaneously or        South to North and south to west simultaneously.
2. North to East and south to west simultaneously.
3. West to north and east to south simultaneously.

o	This state alternates between minor turns to ensure that there is no congestion while giving priority to larger movements from States 1 and 2.

