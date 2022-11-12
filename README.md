# savinn-vdevaras-ddevara

Raichu

Problem Statement: The Board game consists of three pieces. Pichu, Pickachu and Raichu.

Pichu: Pichu’s possible moves are that it can move diagonally one square forward only if that square is empty. Pichu can also jump over another pichu but it has to be of opposite color. The piece that was jumped over will be removed from the board.

Pikachu: Pikachu’s possible moves are that it can move 1 or 2 squares forward or left or right only if it’s a empty square. A pikachu can also jump over a pichu or a pikachu as long as it is of opposite color and it can move 2 or 3 squares in this case . Also there are some constraints to this. First of all the squares between the pikachu’s start position and jumped piece should be empty and also all the squares between the jumped piece and ending position should also be empty.

Raichu: First of all Raichu is created when a pichu or pikachu reached the opposite side of the board. Raichu’s possible moves are that it can move any number of squares which are forward, backward,left,right, and also diagonal to an empty square as long as all the squares in between are empty. A raichu can also jump over a pichu, pikachu or raichu as long as they are of opposite color and can land on any number of squares as long as the squres between the jumped square and the landing square are empty.

In this game the winner is the one who captures all of the pieces of other player. We have to write a code that plays raichu well.

State Space: The state space here is the set of all possible places pichu, pikachu and raichu will be on the board which includes black and white both. 

Initial State: The initial state is the state of the board in which there are pichus and pikachus of white and black on both sides in equal numbers.

Successor Function: We written successor function for pichu, Pickachu and also Raichu.
Since pichu can only move diagonally we have written a successor function which returns all the possible moves. Similarly in the case of pikachu since it can only move forward, left or right we have written a successor function with those constraints and returned all the possible moves. In the case of Raichu, as it can basically move in all directions we wrote a successor function which also considers some constraints like if the square is empty or not and also since it can  jump over pichu, pikachu and also raichu we considered those while building our successor function and then returned all the possible moves for raichu.

Goal State: The Goal state is a state in which a player captures all the pieces of the other player.

