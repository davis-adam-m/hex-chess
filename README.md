# hex chess
Python program that renders outcomes for "chess" pieces on a hexagonal spiral board. 

Inspired by Numberphile video https://youtu.be/UiX4CFIiegM?si=jhmuTZc7iJi_M-BX

Based on the concept by N.J.A. Sloane and the sequence generator by Jonas Karlsson from source: https://oeis.org/A392177/a392177_2.py.txt

From Sloane: 

> Consider the square spiral with its cells numbered starting at 0, as in A308884 and A274641. Two players, Black and Red, take turns. When it is Black's turn, he places a knight at the smallest unoccupied cell not attacked by an existing Red knight, and when it is Red's turn, she places a knight at the smallest unoccupied cell not attacked by an existing Black knight. Sequence lists squares occupied by a Black knight.

This version experiments with 2-6 players all using "knights" using movement rules as defined by Władysław Gliński.

The initial experiment starts simply, with a hexagonal grid and two players. This first iteration has each player make 10 moves. 

![2p 10^1](renders/2p_spiral_chess_hex_10_1.png)

Potential improvements: 
* Modification is clunky with larger numbers of players. Automating consistent marker sizing and spacing would be convenient for reusability.
* Performance becomes problematic above 10^5. A different approach could allow larger renders.

Future versions:
* Implement different pieces with different movement rules
* Play with other underlying polygons, particularly interested in decagons/pentagons but this would probably require a very different implementation. 
