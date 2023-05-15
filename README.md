# Dont_Panic_Challenge_CodinGame

![Don't Panic Challenge screenshot](https://github.com/Jossuc4/Dont_Panic_Challenge_CodinGame/blob/main/images/DontPanic.PNG)


[Link](https://www.codingame.com/ide/puzzle/don't-panic-episode-1)


## Description

It's a programming challenge from [CodinGame](https://www.codingame.com) that gives you more programming experiences.
##Objective of the challenge
You must help the clones reach the exit to escape from the generator area.
## Rules
The area is rectangular and variable in size. It is composed of several floors (0 = lower floor) and each floor has several possible positions for the clones (0 = leftmost position, width - 1 = rightmost position).

### The objective is to save at least one clone in a limited number of rounds.
In detail:

* The clones come out of a single generator at regular intervals, every 3 turns. The generator is placed on floor 0. The clones exit heading to the right. 
* The clones advance one position per turn in a straight line, in their current direction. 
* A clone is destroyed by a laser if it exceeds position 0 or position width - 1.
* The area has elevators to go up from one floor to another. When a clone arrives at a position where there is an elevator, it goes up one floor. Going up a floor takes one game turn. On the next turn, the clone continues its progression in the direction it had before going up.
* On each turn you can either do nothing or block the lead clone (i.e. the one that came out the earliest).
* Once a clone is blocked, you can no longer act on it. The next clone takes the role of lead clone and can be blocked in turn.
* Quand un clone avance ou se trouve sur une position sur laquelle se situe un clone bloqué, il change de direction.
* If a clone blocks at the bottom of an elevator, the elevator can no longer be used
*When a clone reaches the floor and the position of the vacuum cleaner, it is saved and disappears from the area
## Initial inputs
Line 1: 8 integers: 
**nbFloors:** the number of floors in the area. The clone can evolve between floor 0 and floor **nbFloors - 1** 

**width:** the width of the area. The clone can evolve without being destroyed between position 0 and position **width - 1**

**nbRounds:** the maximum number of rounds before the end of the game 

**exitFloor:** the floor of the vacuum cleaner 

**exitPos:** the position of the vacuum cleaner at his floor

**nbTotalClones:** the number of clones that will come out of the generator during the game 

**nbAdditionalElevators:** not used for this first question, is always 0 

**nbElevators:** the number of elevators present in the **areanbElevators** following lines: a couple of integers

**elevatorFloor** and **elevatorPos** respectively giving the floor and the position of an elevator.

## Inputs for a round of play
**cloneFloor** and **clonePos** giving the coordinates of the unblocked head clone followed by the character string direction which indicates the status of the clone: **LEFT** the clone is heading to the left and **RIGHT** the clone is heading to the right
## Out for a round of play
A single line (ending with a carriage return) indicating the action to be performed: the keyword **WAIT** to do nothing or the **BLOCK** keyword to block the head clone
## Contraintes
**1 ≤ nbFloors ≤ 15**

**5 ≤ width ≤ 100**

**10 ≤ nbRounds ≤ 200**

**0 ≤ exitFloor, elevatorFloor < nbFloors**

**0 ≤ exitPos , elevatorPos < width**

**-1 ≤ cloneFloor < nbFloors**

**-1 ≤ clonePos < width**

**2 ≤ nbTotalClones ≤ 50**

**0 ≤ nbElevators ≤ 100**

Duration of a game round : 100 ms

Good Luck

[Jossuc4](https://github.com/Jossuc4)
