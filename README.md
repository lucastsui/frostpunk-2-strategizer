# frostpunk-2-strategizer
 An open-ended project to practice automating decision making in the resource management game Frostpunk 2.

## Background
I want to create an advisor that tells me the optimal way to build the city in order to achieve some goal, for example to achieve certain coal production rate. Why: All managment games are similar. If I can efficiently solve one managment game, perhaps I can readily solve all management games. Also this serves as coding practice and portfolio showcase.

## How it goes
In the planning phase, I use hand written notes to draft out vaugely what will be the flow of logic. The rough idea is that the status of the city, effect of every building (including their upgraded counterparts), and tech upgrades, will be throw into a function to return a sequence of buildings and ugrades to be enacted to achieve an increase of production rate in, say, coal without sabotaging the rates of other resources.

## Project status
2025/02/21: I encode the effects of some buildings into an csv file. I go through some trial and error to decide that dictionary as the data format to go. So far the project comes to a halt as geometic layoff of each district affects their heat demand. And I don't have a good way to encode geometric data. Defining the dexagonal geometry of the game would be very time consuming. I decide to take a break from the project. I will have to decide if I have to research in UI desing to come up with a more visal solution or just go full mathematics to define said geometric space without visualization.
2025/02/24: Search for a way to build a GUI. matplotlib.patches.RegularPolygon is worth further resaerch.

## Lessons learnt:
As project requirements and coding decisions inform each other as the project goes on, refactoring in inevitable. Balancing the desire to reducing refactoring versus avoiding decision paralysis is a task that I haven't found a good solution yet.

Eg origianlly, the name of a building is a dictionary item. Unbeknownst to me this makes search dictionaries by name very clumsy, forcing me to store the building stats as dictionary of dictionaries, with building name as keys.

Eg In the midst of development, it turns out that the effects of each building depends on its surrounding buildings, necessitating the encoding of geometric information into the decision making process, massivley complicating the project.

Waterfall system design doesn't feel like a good approach as there are bound to be unanticipated problems necessitating changes.


