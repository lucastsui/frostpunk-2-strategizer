# frostpunt-2-strategizer
 An open-ended project to practice automating decision making

## Background
I want to create a an advisor that tells me the optimal way to build the city in order to achieve some goal, for example to achieve certain coal production rate. Why: All managment games are similar. If I can efficiently solve one managment game, perhaps I can readily solve all management games. Also this serves as coding practice and portfolio showcase.

## How it goes
I use writing notes to draft out vaugely what will be the flow of logic. The rough idea is that the status of the city, effect of every building (including their upgraded counterparts), and tech upgrades, will be throw into a function to return a sequence of buildings and ugrades to be enacted to achieve an increase of production rate in, say, coal without sabotaging the rates of other resources.

## Project status
2025/02/21: I encode the effects of some buildings into an csv file. I go through some trial and error to decide that dictionary as the data format to go. So far the project comes to a halt as geometic layoff of each district affects their heat demand. And I don't have a good way to encode geometric data. Defining the dexagonal geometry of the game would be very time consuming. I decide to take a break from the project. I will have to decide if I have to research in UI desing to come up with a more visal solution or just go full mathematics to define said geometric space without visualization. 2025/02/24: Search for a way to build a GUI. matplotlib.patches.RegularPolygon is worth further resaerch.

## Lessons learnt:
There are many times I am stuck. Some issues identified:
Lack of understanding how a piece of code will behave, like what would happen if I throw a dictionary into a for loop.
Unanticipated problems during implementation forcing me to replan. Eg origianlly, the name of a building is an dictionary item. Unbeknownst to me this makes search dictionaries by name very clumsy, forcing me to stor the building stats as dictionary of dictionaries, with building name as keys.
Waterfall system design doesn't feel like a good approach as there are bound to be unanticipated problems necessitating changes. So far the level of details planned are okay - the overall flow of the logic doesn't go off rail.


