# frostpunt-2-strategizer
 A open-ended project to practice automating decision making

## Background
I want to find a better way to play management game than relying on unreliable and imprecise gut feeling.
I choose the game Frostpunk 2 to be the subject of study as I happened to be both seriously learning coding and playing the game simultaneously.
Another goal is to learn whatever I can learn in the process. I expect to learn how to autmoate decision making in general, coding skills, and how to incorporate new knowledge into exiting, work-in-progress projects.

## How it goes:
At the planning phase, I use writing notes to draft out vaugely what will be the flow of logic.
In essence, I am building a function that accepts three arguments: a goal, the status of the city, effect data of all the buildings and upgrades.
The return would a sequence of suggested buildings and upgrades to be carried out.
The rest is to come up with ways to encode the game logic and find computationally efficient ways to find a solution.

Expecting making high level mistakes, I don't plan out every detail in one go.
I encode the effects of some buildings into an csv file, then go through some trial and error to decide that dictionary as the data format to go.
The code and represent how many buildings are there and compute their combined effects.
But some complications bring the project to a halt.
	1. Some technologies will impact all buildings.
	2. I haven't planned for coding for policy, which also carries global effects.
	3. geographic location of the districts will impact each other's performance.

I have some ideas. The first two is doable with some refactoring done. The thrid is thorny as defining the dexagonal geometry of the game would be very time consuming. I decide to take a break from the project. I will have to decide if I have to research in UI desing to come up with a more visal solution or just go full mathematics to define said geometric space without visualization.


## Lessons learnt
Reducing googling time by mastering the tiny coding acts. Eg what would happen if you put dictionary into a for loop (answer: it gives just the keys, not key-value pairs).
Locate the cause of a problem being unexpected. Eg Eg origianlly, the name of a building is an dictionary item. Unbeknownst to me this makes search dictionaries by name very clumsy, forcing me to stor the building stats as dictionary of dictionaries, with building name as keys.
Waterfall system design doesn't feel like a good approach as there are bound to be unanticipated problems necessitating changes. So far the level of details planned are okay - the overall flow of the logic doesn't go off rail.


