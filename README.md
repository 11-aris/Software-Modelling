# Software-Modelling
Specification (Narration)
The Gishushu Traffic Light System operates with three main states: Red, Green, and Yellow, each of which serves to control traffic flow based on a preset timer sequence, with provisions for emergency vehicles.

1. Initialization
When the system initializes, it defaults to the Red light to ensure safety as vehicles prepare to stop and wait for instructions.
2. Red Light State
Duration: 30 seconds.
Behavior: Vehicles are stopped to allow traffic flow from perpendicular directions.
Exit Condition: After 30 seconds, the system transitions to Green for the current lane.
Emergency Override: If an emergency vehicle (such as an ambulance) is detected, the system can switch to Yellow immediately to prepare for the Green light and prioritize emergency traffic flow.
3. Green Light State
Duration: 45 seconds.
Behavior: Vehicles are allowed to move through the intersection.
Exit Condition: After 45 seconds, the system transitions to Yellow to warn that the light will soon turn red.
Emergency Override: If the emergency vehicle has passed, the system resumes its normal sequence.
4. Yellow Light State
Duration: 5 seconds.
Behavior: The Yellow light signals that the Green light phase is ending, prompting vehicles to slow down and prepare to stop.
Exit Condition: After 5 seconds, the system transitions back to the Red light, restarting the cycle.
