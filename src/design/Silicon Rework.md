# Full Silicon Rework

Your title should convey the basic jist of your proposed changes. It should be short because the text will be linked in the sidebar.

| Designers | Implemented | GitHub Links |
|---|---|---|
| MangoMaeve | :x: No | TBD |

`Designers` should be the names that you use on GitHub and/or Discord. This is optional but strongly recommended, since:

- This acknowledges credit where it is due
- People who are confused about the written intent can use this information to contact the authors

`Implemented` is the status of the feature.

Github links can include multiple PRs, if relevant.

## Overview

Reworks silicons to be more in line with their implementation in tg based space station 13, adding some much needed complexity to their gameplay and interactions

## Background

The current implementation of cyborgs feels unfinished and shallow, ridiculously easy to repair, little complexity to how they work, and shockingly little interaction with the roboticist. This design proposal aims to address issues and pave a groundwork to expand upon cyborg and AI gameplay.  

## Features to be added
# Cyborgs
  Additional tasks for the roboticist:
    Borgs can no longer be repaired fully with just a few seconds and a welder, instead needing different maintenance processes depending on the type and severity of the damage.
      A Borg in critical condition will no longer immediately get up after being repaired, instead needing to be rebooted by someone who can access their internals.
      Burn damage is no longer repaired via welding, instead requiring the cyborg to be opened up, battery removed, and using cables to repair burnt out wiring.
      With the help of a roboticist, Borgs will be able to swap to a new model from their old one, rather than having to create a whole new chassis and leaving the old one as an empty husk.
      The above is accomplished by the addition of a wiring panel to the cyborg, accessed by opening their maintenance panel and removing the battery, then clicking the cyborg with a multitool or wire cutters. Currently only one functional wire is planned in the "Module" wire which would be snipped to return a borg to a blank chassis, then mended to allow them to select again, but the panel would lend itself to further uses down the line.
      A suite of new generic upgrades for use by any borg model, including a battery powered jetpack, a speed upgrade, and a very minor self repairing upgrade.
  New utilities for Cyborgs
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

Consider addressing:
- How does the feature align with our [Core Design Principles](../design/design-principles.md) and game philosphy?

## Roundflow & Player interaction

Consider addressing:
- At what point in the round does the feature come into play? Does it happen every round? How does it affect the round pace?
- How do you wish for players to interact with your feature and how should they not interact with it? How is this mechanically enforced?

## Administrative & Server Rule Impact (if applicable)

- Does this feature introduce any new rule enforcement challenges or additional workload for admins?
- Could this feature increase the likelihood of griefing, rule-breaking, or player disputes?
- How are the rules enforced mechanically by way the feature will be implemented?

# Technical Considerations

- Are there any anticipated performance impacts?
- Does the feature require new systems, UI elements, or refactors of existing ones?
- For required UI elements, give a short description or a mockup of how they should look like (for example a radial menu, actions & alerts, navmaps, or other window types)
