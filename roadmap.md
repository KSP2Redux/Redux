# KSP2 Redux Roadmap

![KSP2 Redux Roadmap](images/roadmap.png)

## Stage 0: Foundation

> *“We choose to go to space, not because it is easy, but because we thought it would be easy.”*

The “0 Days Since Last Accident” sign at KSC once again resets to zero. After too many rapid unscheduled disassemblies, the Kerbals decide it’s time to look under the hood and start making rockets that don’t explode… that much.

The initial series of Redux releases will be focusing on building a solid foundation for the game going forward.

**Performance & Fixes**
- Optimizations of existing game systems and graphics settings to increase performance
- Fixes for various game bugs and inconsistencies, big and small
- Start of a larger effort to convert the game’s core simulation code to make use of Unity’s **[DOTS](https://unity.com/dots)** systems with potential for massive performance gains, scaling with vessel sizes and counts

**Vessel ISRU**
- Small-scale preview of the larger resource management system, similar to KSP1’s ISRU
- Vessel parts for scanning, gathering and processing resources necessary for basic refueling operations
- Production of Hydrogen, Methane, Oxygen and Monopropellant depending on the given location’s available raw resources

**Heat Management**
- Heat generation and dissipation system for vessel parts, e.g. reactors and drills will generate heat and radiators will remove it
- Introduction of radiator parts

**Tech Tree Updates**
- New types of requirements for unlocking a tech tree node in addition to science points
- Mission unlocks will require the player to complete a specific mission before a tech node can be unlocked
- Science experiment unlocks will require the completion of a specific experiment, sometimes in a specific location or biome, in order to meet the requirements of a tech node

**Modding SDK**
- Improved modding experience fully integrated into the Unity Editor
- Possibility to run the game and test mods directly in Unity’s play mode
- Multiple mods sharing a single Unity project in order to decrease the total disk space taken

## Stage 1: Colonies & Resources

> *“I came, I saw, I built a colony… and then I ran out of coffee!”*

Kerbal scientists just had an epiphany! While “MOAR BOOSTERS” is always a viable and well-respected strategy, their latest coffee-stained blueprint (and yet another failed attempt at an Eve mission) sparked a wild idea. What if they could build the return vehicle directly on Eve? Just make sure Jeb doesn’t lick the purple rocks again.

This stage of Redux development will be dedicated to implementing the core gameplay elements of colonies and the full resource system, as well as a brand-new game mode. As this is such a complex undertaking, this stage will be split roughly into 3 parts.

### Stage 1.1*

**Planetary Colonies**
* Introduction of surface-based colony parts, including resource gathering facilities and factories
* System for founding and building colonies (using the Building Assembly Editor)
* New raw resources and building materials
* Colony-based vessel factories and launch pads

**Frontier Mode**
* Initial limited-scale preview of a new game mode based on resource management
* All parts cost an amount of building materials which the player has to create by processing raw resources gathered at their colonies
* KSC has unlimited amounts of basic building resources and fuels, but colonies and more exotic resources are required to build more advanced vessel and colony parts
* More details in the FAQ below

**Colony Management UI**
* Basic UI for tracking the flow rates of all of the colony’s resources, electric charge (generation and consumption), and heat (generation and dissipation)

### Stage 1.2*

**Orbital Colonies**
* New parts and systems for orbital colonies
* On-orbit vessel construction using orbital colonies as shipyards
* In-depth planning tools for EC generation and consumption

**Exploration Updates**
* Implementation of a new resource unlocking system for Exploration Mode, distinct from the Frontier Mode 
* Resources are not continuously mined and used up, instead, once the requirements for the use of a resource are met (e.g. through a dedicated mining facility, a mission, etc.), that resource is then fully unlocked at that specific colony
* Orbital colonies serve a special purpose in Exploration Mode - as long as any two celestial bodies both have an active colony in orbit, they will also share all their unlocked resources, allowing the creation of an interconnected network of colonies to make all unlocked resources available everywhere
* More details in the FAQ below

### Stage 1.3

**Supply Routes**
* Frontier Mode feature that will allow the player to utilize colony spaceports to create automated resource and material supply routes between their various colonies
* Flying a mission from one colony (or KSC) to another will give the player an option to record the flight as a supply route, periodically transferring the amount of resources that the vessel was carrying from the origin point to the destination, while subtracting the material costs of the supply vessel from the origin colony

**Environmental Heat System**
* Environments will start playing a role in the heat generation and dissipation system, introducing a new type of challenge for colony placement and management
* For example, colonies might use water sources as coolant, and on the other hand, they will have to dissipate enough heat to compensate for being placed in e.g. a lava river biome
* In-depth planning tools for heat generation and dissipation

**New Content**
* Advanced engines that are well suited for hauling large quantities of resources across the Kerbol system
* New missions and science experiments related to colonies
* Additional content to be detailed later

\* **Disclaimer**: These stages will very likely be reordered with Orbital Colonies coming before Surface Colonies, as well as some features being moved between stages. The exact details are still being worked on.

## Stage 2: Interstellar
> *“To infinity… and probably a crash landing!”*

As the Kerbal civilization expands all across the Kerbol system, from the fiery pits of Moho to the freezing far reaches of the outer planets, new resources and scientific discoveries finally enable the Kerbals to travel to the stars. Excited, they blast off for distant systems - but what is this? Oh boy, it’s going to be a long ride when Bob packed only decaf for the trip!

The next iteration of Redux updates focuses on travelling beyond the Kerbol system using all-new interstellar-scale parts.

**Debdeb System**
* New star system, the closest one to Kerbol
* Planets and moons which present new challenges
* Exotic resources and new building materials allowing the creation of even more advanced vessels and colonies
* New missions and science experiments related to the new star system

**Interstellar Parts**
* Massive parts for constructing vessels for interstellar travel
* Advanced far future types of propulsion enabling travel speeds at significant fractions of speed of light

## Stage 3: Multiplayer

> *"All for one, and one for all… unless we’re fighting over the last donut!"*

One Kerbal crashing is fun, but a whole squad fighting over who gets to press the big red launch button? That’s what we call Kerbal mayhem! Teaming up to build rockets, or “accidentally” nuking each other’s bases, the Kerbals are buzzing with caffeine and chaos. Multiplayer makes the galaxy feel much less empty.

**Multiplayer Support**

* Multiple players can share an agency, working together towards common goals and shared progress as they explore the galaxy
* Agencies can work together or compete to see which team win the next space race
* Interact with other players in real time, launch your rockets at the same time from multiple launch pads and race to orbit, or sabotage your enemies’ colonies to get ahead in the competition

**New Star System**
* Using the newly acquired exotic materials from the Debdeb system, players can venture out further into the unknown, discovering even more distant stars

**Story Conclusion**
* The main story campaign comes to its conclusion

## FAQ

### Is the roadmap final?
This roadmap of development stages only serves as a rough outline, and as we progress through the goals and gather player feedback, it’s very likely that some design decisions will change, or we will discover that some of our ideas are not technically viable/worth the extra effort and so on, so please, take this with a grain of salt. Especially with the stages that are further out, a lot of the design is still up in the air, so don’t be surprised if some features get added, reworked, or removed as we get closer to each stage.

### What’s the difference between the Exploration and Frontier modes?
You can think of them as the respective spiritual successors to KSP’s Science and Career modes.

In Frontier mode, all vessel and colony parts cost some amount of materials, which you must have stockpiled in order to be able to build the part. In order to get there, you will need to build mining facilities to extract raw resources and factories to process them into materials or fuels. The rates of resource gathering and processing can vary based on factors such as local resource density, colony happiness, etc. (these factors are just examples, subject to change). To found and grow a new colony, you will need to ship resources from Kerbin or other existing colonies, eventually leading up to the ability to create automated supply routes.

Exploration mode also has resource gameplay, but rather than having to manage resource and material production rates, supply missions, etc., the colonies and resources are more so an additional means for exploration and rocket building. Once you set up a colony in a new location and meet the requirements for the specific resource (e.g. by building a colony facility, running an experiment or completing a mission), that resource will then be “unlocked”. When building vessels and colonies, all the resources needed for a specific part will need to be unlocked, and then you can build as many of them as you like without any limits. Colonies will be linked together through orbital colonies, which will provide the unlocked resource to all other celestial bodies with an orbital colony. No need to deal with resource rates, quantities, supply missions, and so on.

### What about new missions, science experiments, parts, …?
Even when not explicitly specified, we will be adding some content throughout *all* the stages. That means things like new missions, new tech tree nodes, new parts, new colony facilities, new resources and materials, new science experiments, and so on.

### When will XYZ be released?
To answer one of the most frequently asked questions very directly - sadly, we cannot give you any estimates of how long each of these stages will take. This is a volunteer project which people work on in their free time, and so we have no idea how long a specific feature might take to finish, and the last thing we want to do is adding the pressure of setting deadlines for the team, or setting false expectations for you, the players. Please, be patient.