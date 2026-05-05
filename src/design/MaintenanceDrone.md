# Create the Maintenance Drone and Drone Auto-fabricator


| Designers | Implemented | GitHub Links |
|---|---|---|
| MangoMaeve| :x: No | TBD |


## Overview

Adds a machine to robotics that will automatically create low-impact ghost roles in the form of maintenance drones lawbound not to interact with non-drone beings.

## Background

Often times, upon joining a round as an observer there are few to no interesting ghost roles to take, barring the occasional mid round antagonist or pun pun. Maintenance drones would, I believe, offer a sort of observer+ role, allowing observers to actively take part in the round while being largely unimportant to the broader plot of the round.

## Features to be added

Drone: Auto-Fabricator: Would add a single machine to the robotics labs (Or, if that would be obtrusive to mappers, a flatpack or circuit board in the robotics locker), that, when provided at least 10 steel and glass will fabricate one drone shell as a ghost role for that amount of materials, once that role is taken it will produce another shell provided it has enough materials. If this concept comes to fruition I intend the fabricator to be upgradeable and perhaps to have a traitor interaction (TBD)

Maintenance Drone: Small silicon drones bound to the drone lawset (Look up what this one is actually called later) moves by flying and can go under objects ala t1 replicator. Drones posses an internal storage similar to a slime, but sized up to satchel size (Reduce as needed if this is too much) anyone can open this storage without alerting the drone. Drones by default have a single standard hand slot, an omnitool, an industrial welder, and a fire extenguisher, alongside a built in flashlight. (Maybe incorporate some way for the ai to order the drones around with minimum interaction, some sort of maintenance ticket system?)

## Game Design Rationale

Seriously silly: These drones are the pinnacle of dystopian corporate tech. Cheap, mass-producible, and wholly maintenance focused. The maintenance drone does not care you are in the room, the room is on fire and the fastest way to fix that is to vent the atmosphere.

Zero sum: Drones would have little impact on the round as a whole, outside of taking some pressure off the maintenance workers

Maintaining authenticity: We already have semi-intelligent constructs in the form of the various bots that can be crafted, and a cheap, easy to replace maintenance bot seems right up NT's alley.

Take things slow: Sometimes, there are just too many holes and not enough engineers to patch them (Especially when arrivals gets hit with debris for the fourth time in a round) Repair drones would allow engineers to focus on the worst of the damage while the drones deal with smaller problems

Roleplay potential: While the drones themself are not allowed to interfere with people, the same cannot be said the other way around, the crew is free to mess around with or bully drones to their heart's content with no fear of the drone even being able to retaliate, or even report them. Drones would be free to interact and chat with each other (Would need to figure out how to make their speech indecipherable to non-drones). On top of that, I intend for the ai or command to be able to submit a maintenance ticket system which would then be sent to a UI the drones can access remotely(Maybe give engineering a computer that taps into the same ticketing system? Out of scope, might do another doc about that.)

## Roundflow & Player interaction

Consider addressing:
- Drones would begin being manufactured as soon as the Auto-Fabricator is provided with the materials for one drone (10 glass, 10 steel)
- The robotocist would be responsible for keeping the fabricator full of materials, drones would go about diverse maintenance tasks, AI and command members could remotely task drones via the ticketing system, and the crew at large can do pretty much anything they want to a drone with no consequence.

## Administrative & Server Rule Impact (if applicable)

- Drones in violation of their strict non-interference lawset will likely be an issue, but hopefully one that will smooth over with time
- Ideally no, but if someone decides to be a shitter like the folks who make mice do the "Saw a nukie dance" then problems could arise
- The drones are fragile by design, and move at the same pace as a well-nourished, healthy person, any drone being antagonistic or otherwise interfering will be scrapped with great ease. (Possibly add a button to the fabricator to remotely fizzle specific drones)

# Technical Considerations

- Not likely, new drones will only be created if materials are provided and there is no un-occupied shell.
- Would require a new system for automatically creating drones from the fabricator, plus the ticketing system. ticketing system would need a UI (Would I be adding the ticket submission to PDAs or comms consoles? Get feedback.)
- Ticketing system could be based off nanotask, keeping the priority level and description, but removing the requester field, would need a way to mark them as completed. (Is that in nanotask already? I only use it for paper.)
