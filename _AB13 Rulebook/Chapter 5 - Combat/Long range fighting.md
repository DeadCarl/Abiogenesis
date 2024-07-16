# Design

While all rpgs can reasonably handle the gunfight, the room crawl and the dungeon brawl, most do not handle scales of 100 meters or more between combatants very well.

To handle these infantry battles in an efficient and fun manner, Ab13 needs to distinguish between the close quarters gunfight and the infantry battle by creating a new structure for the latter.

```
A **map** is a [symbolic](https://en.wikipedia.org/wiki/Symbol "Symbol") depiction emphasizing relationships between elements of some space, such as [objects](https://en.wikipedia.org/wiki/Physical_body "Physical body"), [regions](https://en.wikipedia.org/wiki/Region "Region"), or themes.
```

This symbolic representation cannot accurately depict all important features of the original at the same time, and so we must abstract to simpler forms. These simpler forms can be stacked by how abstract they are, a notion called a level of detail.

A critical order of detail here is the principal layer (layer 0) and the microlayer beneath it (layer -1), the order of detail where individual subelements are either grouped into a higher order of detail, or are left undepicted.

The infantry battle has a major problem where relevant-critical details can exist on layer 0 or layer -1, but we can't draw both fully and efficiently - we must constantly abstract out things such as microterrain or dead space, but must remember they do exist.

---

Infantry battle maps have 3 layers. Each successive layer receives more player input

layer 1: the environment where the fight is located. The choice of layer 1 determines what layer 0 features can be picked and what mapwide behaviors exist in the map  layer 1 is always decided by the story. 

layer 0: the immediate features of the environment, the positive or negative space available that define the boundaries or spaces on the map. 

Layer zero starts with an initial subregion of (combat length) in distance with zero or more subregions attached to it. The combat value of a subregion depends on either random chance or the ability of a leader to locate good terrain.

Leaders can move across these diifferent subregions, or find access to new subregions to move to work a tactics check, though at some point they will run out of options. Once a subregion is established it cannot be changed.

layer -1: the microfeatures that the players immediately use but are seldom drawn.

Characters may identify microfeatures to support their actions with a tactics check constantly, though at some point this ability to do so can run out (as they get progressively more pinned).

Microfeatures can always be added to a map as long as it holds enough combat value. 

# Running layer 0

Layer zero is decided by who can exploit their tactical initiative. If neither have tactical initiative then the roll is random. If a group has tactical initiative but fails the tactics roll they cannot exploit it well or at all, and if they succeed they get to roughly shape the layer 0 region.

Layer 0 elements
- Spawns
- Regions structure on board
- Number of initial regions
- Number of additional regions?


# Layer -1

Tactics check with a tn based on layer 0.

--- 

Layer 0 placement.

A layer 0 test determines who places the terrain, what its general shape looks like and where that terrain goes. 

Successful tests favor the roller, unsuccessful tests favor the opponent

# Gameplay loop

1. Initial situation
	a. enemy is known
	b. enemy unknown
	c. mobile
	d. stationary
## [scaling](https://en.wikipedia.org/wiki/Level_of_measurement)
Is entirely determined by the gm, but in general consists of any number of regions greater than 100 meters in length in total

For example, a map with 4 regions of 25 meters each in a line would be considered large scale

Regions consist of either positive, negative, or some fraction of the two spaces

Regions do not have to be rectangles
## Initial phase, GM 

1. GM determines the Level one region
2. Gm determines scale of a terrain piece

All terrain pieces must be touching at least at 1 point? Any gaps are to be determined as positive or negative space based on the GM's ruling until a group decides to uncover another terrain piece.

## Initial player phase, shaping field
This is known as the shaping phase because if the teams intend to fight, they will attempt to shape the battlefield to suit them, such as through an ambush or by acquiring higher ground prior to the opponent.

1. Groups determine their objective
2. both groups nominate a commander to make a competing tactics roll
- [ ] this could be called the reconnaissance check
3. on success, the commander nominates placement of 1 level zero piece of terrain and the initial spawn.
	2. The margin determines the quality of the terrain (is this based on GM's judgement or with soft rulings?) in regards to how well it supports their objective
	- [ ] what if the margin also determined the number of terrain pieces a side puts down?
	- [ ] what if the number of group elements determined the number of terrain pieces a side puts down
	1. the margin should be lose with normal successes or failures containing 'yes, but' results. Only exceptional margins should provide definitive results
	2. after consulting with the GM, the group arranges the piece of terrain according to their understanding of the situation.
4. on failure, who decides to put the terrain down? The commander choses the initial spawn

### Questions
- What about minimum initial range or getting initial shots on? 
- What about holding terrain the enemy can't take
- What is the size of a terrain piece
- How does one handle split forces
- How do we determine the shape of a terrain space
- How does an actor move through a terrain space
- Can a recon roll be split so heterogenous terrain can be laid? (Ie barn house and field)
- How is a moving position handled? Is the path a level one feature?
- What happens if a player narrates a preplanned decision

## Initial phase, no player shaping
If the two groups do not shape the battle prior to engaging (aka: complete surprise), the GM rolls for luck for each side (2d20L!6), then generates the terrain and  based on the fortune of each group. The groups have no decision in how this terrain nor their assembly is set up beyond what they were immediately doing prior to the interruption.
## Subsequent phases

1. GM determines whether players may add to the map depending on the local Level one terrain surrounding the immediate area in a particular direction
2. The group then rolls a terrain check with a modifier based on the local region the terrain is a part of in one cardinal direction.
	1. on success, the group adds a level zero terrain piece onto the map in an arrangement of their choosing in consultation with the GM. The margin of success determines how well the arrangement should suit them.
	2. On failure, the group adds a level zero piece of terrain onto the map, but the GM determines how the arrangement disadvantages them.

questions:
- [ ] What is the size (scale?) of this region?

# microterrain
## cover
A character who decides that they will look for dead space cover rolls a tactics check. 

On success, they may place one piece of terrain with a combat value equal to their margin of success adjacent to where they started or ended within reason.

This piece of cover stays for the duration of the fight

## paths

# Sources
https://en.wikipedia.org/wiki/Spatial_scale
https://en.wikipedia.org/wiki/Scale_(map)
https://en.wikipedia.org/wiki/Level_of_measurement

Level of detail

[Symbols](https://en.wikipedia.org/wiki/Map_symbol) versus scale

