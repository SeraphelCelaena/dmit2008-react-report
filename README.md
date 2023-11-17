# DMIT2008 Report: Thinking in React
By: Andrew Ng<br>
I am going to do a report on a website I frequent everyday: The seelie.me planner page for a mock representation on how I assume it will work if I were to try to implement it in React.

### Start with a Mock
Here is the page I am going to be analyzing.
<!-- Insert Page Images Here -->
<img src="./images/mockSource1.png">

Functionality on the page:
* Filtering based on the day of the week
* Show/Hide the characters and weapons to display
* Time based task tracker adding/editing/removing
* Time based Resin tracker that shows how much you have at a given moment
* Required resources tracker based on what I can gather on the specified filtered day for my required characters and weapons
* Nav (Left) that takes you to a different pages to look at the different tabs
* Clicking on a character brings up a menu that allows you to change the current and desired level you wish to make them
* Clicking on a material brings up a menu that allows you to change the current amount of that material and it's upgrades/downgrades that you own, which will update the inventory in the background

You would need to navigate to other menus on the left to create the initial character/weapon and what you currently have compared to what you desire, and to have your inventory initially set up.

If I were to implement this myself I would use a json api that would track characters, weapons, and what is requried for them. This json file is then broken down, where the current level and desired level are compared, getting the difference, then taking that compared to what is currently on hand, then taking that difference to output onto the screen what is required for the user to do to get all those needed materials.

```json
[
	{
		"id": "1",
		"user": {
			"name": "Serpag",
			"account": "Main",
			"world-level": 8
		},
		"characters": [
			{
				"name": "Furina",
				"element": "Hydro",
				"current-level": "70/80",
				"desired-level": "90/90",
				"talents": {
					"normal-current-level": 1,
					"normal-desired-level": 10,
					"skill-current-level": 4,
					"skill-desired-level": 10,
					"burst-current-level": 7,
					"burst-desired-level": 10,
				},
				"weapon-type": "sword",
				"weapon": {
					"name": "Splendor of Tranquil Waters",
					"current-level": "60/60",
					"desired-level": "90/90"
				}
			},
			{
				"name": "Navia",
				"element": "Geo",
				"current-level": "1/20",
				"desired-level": "90/90",
				"talents": {
					"normal-current-level": 1,
					"normal-desired-level": 8,
					"skill-current-level": 1,
					"skill-desired-level": 8,
					"burst-current-level": 1,
					"burst-desired-level": 8,
				},
				"weapon-type": "greatsword",
				"weapon": {
					"name": "Considered Judgement",
					"current-level": "1/20",
					"desired-level": "80/80"
				}
			}
		],
		"inventory": {
			"gold": 3000000,
			"experience-books": {
				"tier-1": 25,
				"tier-2": 55,
				"tier-3": 420
			},
			"pure-sacred-dewdrop": {
				"tier-1": 26,
				"tier-2": 34,
				"tier-3": 10,
				"tier-4": 2
			}
		}
	}
]
```

### Break the UI into a Component Hierarchy
Here is a image of the component breakdown.
<!-- Insert images here -->
<img src="./images/">

Below is the breakdown of the compoents of the images above in a nested hiearchy.
* 

### Minimal Representation of State


