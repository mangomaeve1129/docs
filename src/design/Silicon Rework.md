# Silicons Redone

Your title should convey the basic jist of your proposed changes. It should be short because the text will be linked in the sidebar.

| Designers | Implemented | GitHub Links |
|---|---|---|
| MangoMaeve | :x: No | TBD |



## Overview

Reworks silicons to be more in line with their implementation in tg based space station 13, adding some much needed complexity to their gameplay and interactions

## Background

The current implementation of cyborgs feels unfinished and shallow, ridiculously easy to repair, little complexity to how they work, and shockingly little interaction with the roboticist. This design proposal is largely aimed at reworking Cyborg gameplay and systems but does impact the Station AI in several ways.  

## Features to be added

 
# Additional tasks for the roboticist:
    Borgs can no longer be repaired fully with just a few seconds and a welder, instead needing different maintenance processes depending on the type and severity of the damage.
      A Borg in critical condition will no longer immediately get up after being repaired, instead needing to be rebooted by someone who can access their internals.
      Burn damage is no longer repaired via welding, instead requiring the cyborg to be opened up, battery removed, and using cables to repair burnt out wiring.
      With the help of a roboticist, Borgs will be able to swap to a new model from their old one, rather than having to create a whole new chassis and leaving the old one as an empty husk.
      The above is accomplished by the addition of a wiring panel to the cyborg, accessed by opening their maintenance panel and removing the battery, then clicking the cyborg with a multitool or wire cutters. Currently only one functional wire is planned in the "Module" wire which would be snipped to return a borg to a blank chassis, then mended to allow them to select again, but the panel would lend itself to further uses down the line.
      A suite of new generic upgrades for use by any borg model, including a battery powered jetpack, a speed upgrade, and a very minor self repairing upgrade.
 
 # New utilities for Cyborgs
    Cyber Interface: An integrated PDA substitute for cyborgs to use, comes with an instant messenging app, Crew Manifest,and a self diagnostic and chassis settings application.
    The above application would allow the Cyborg to self diagnose damages to their chassis, unlock their own panel cowling, edit the power level of their onboard flashlight, and disable the ai's view through the on-board camera.
    Alerts panel: Allows the cyborg to diagnose issues or hazardous areas on the station by collecting power and atmospherics alerts in a simple categorized list view.
    Remote Interaction: Allows the cyborg to interface with any networked device it can see, rather than by physical proximity, also allowing them to remotely bolt, shock, and set emergency access on a door.
    Binary Garbling: In a similar vein to the bloodcult, speech over binary will be displayed in whisper range as a series of ones and zeros, rather than plaintext that anyone can eavesdrop on.

# Station AI
  Enhanced access: Allows the station Ai a deeper level of interaction with all devices, enabling it to operate SMES, Substations, and Lathes.
  Tracking: Latches the camera view onto a selected entity until the sAI moves their cursor manually or the camera network loses sight of the target.
  sAI will also receive both the Cyber Interface and alerts panel listed above, alongside a records console and crew monitor.
  I have some ideas for a modular upgrade system for the sAI, but will touch on those in a seperate document, as it's rather out of scope.
  
  

## Game Design Rationale

# Seriously Silly:
  The way cyborgs currently operate has two major flaws as I see it, lack of mechanical depth and overuse in combat scenarios. No matter what else is happening, if there's a welder in the area and five to ten seconds of breathing room, any player can repair a borg into perfect shape, this results in them being used as both a combat juggernaut and a vessel for validhunting. Because they can be so easily repaired the crew can just continually throw borgs at a problem and repair them to do it again in mere seconds if the kill is not secured, even if the borg would be put to better use elsewhere during crisis time. As a borg main myself, I find this terribly uninteresting and believe borgs are more suited in the civillian roles they're meant to occupy, only really threatening anything when subverted and given the element of surprise. I do find a single exception to this in the form of an idea for security borgs I have in mind, but that is out of scope, and relies on the outlined changes to ever even see a design document.
  Outside of the changes to their combat viability, the interface opens up additional approaches for antags to get cyborgs on their side, the ability for a borg to unlock itself means that subverted borgs are available to anyone who can trick or convince a cyborg to pop their lock long enough to be hacked. While the ability to cut the ai's camera view through the borg lets them hide actions done while subverted more effectively.

# No Win or Loss:
  The changes proposed here are a mix between utility and taking borgs out of combat roles, utility expansions to make silicons and by extension robotics more interesting, and maintenance changes to make combat significantly more risky for Cyborgs. Overall it should help Silicons feel more interesting and engaging to play with and around while discouraging the sort of no risk full reward combat role their current implementation allows them to take.

# Maintain Authenticity:
  I cannot imagine something as complex and and expensive as a Cyborg or sAI would not have a suite of digital tools at its disposal, the Cyber Interface allows the Cyborg to tweak settings and automatically diagnose damages to their chassis, while instant messenger (Nanochat) allows them to speak privately to each other and crew without the use of a radio channel. The Ai gets the ability to zoom to anyone their cameras can see and track them while being more thoroughly integrated into the station it belongs to
  Being able to change Model from the moment a Cyborg spawns is my greatest argument to allow them to change again with the help of a roboticist, all the underlying kit to do so should still be in the cyborg under the new shell, they're just locked out of doing so without crew assistance so they can't abandon their current post without at least someone knowing.
  Lastly is the change to binary whispers, I find it immersion breaking that a radio channel purpose built for mechanical life and requiring a translator key for anyone else to listen in on, while being referred to as binary, should ever be understandable by someone standing next to the silicon speaking over it.
# Take Things Slow
    The systems and mechanics introduced here should not be overly complex to get a grasp on, most things within are broadly self explanatory or easy enough to understand with just a bit of practice, While allowing for the player to get better and better at playing a silicon with the tools and restrictions added.
    Repairing Cyborgs will now be more of a time-sink, but still not a terribly long process, instead requiring one to three steps to fully fix up a broken borg.

# Maximizing RP
  A more lengthy repair process, combined with the ability to convince a cyborg to unlock itself if you're persuasive or tricky enough should make RP'ing with Borgs more enticing and fun than the current state of them, allowing borgs oppurtunites to roleplay they by and large do not get right now.


## Roundflow & Player interaction

These features come into play from start to end of round, so long as there are borgs or an Ai
The features as proposed should encourage borgs to seek out proper maintenance and upgrades, while avoiding combat, both of which are handled by the expanded repair processes. Aside from that the utilitarian additions have very few interactions outside of their listed roles that I can think of.

## Administrative & Server Rule Impact (if applicable)

The ability for borgs to unlock themselves may lead to borgs actively seeking out antagonists in order to get subverted, a sort of inverted validhunting
- What I described above should be the only real concern there, aside from that I can't think of other potential issues
- No mechanical enforcement, doing so would make the self unlocking feature all but worthless, will likely need to be enforced manually.

# Technical Considerations

- Unlikely, but not impossible.
- Would require some new systems and at least one ui, some features could use modified versions of current ui.
- I'd like the Cyber Interface to use a UI similar to the one used on TG station, as it is a near 1:1 replica.

# Notes
 This document focuses on cyborgs themselves as a whole, however should I ever complete the objectives listed here I'll likely take a look at additional models of cyborg as well as a complete rework of upgrade modules to be more in line with TG
