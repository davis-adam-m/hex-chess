# hex chess
Python program (and variations) to compute and render outcomes for "chess" pieces on a hexagonal spiral board. The simple rules result in surprising and often beautiful patterns. These variations might collectively be described as a cellular automata.

Inspired by Numberphile video https://youtu.be/UiX4CFIiegM?si=jhmuTZc7iJi_M-BX

Based on the concept by N.J.A. Sloane and the sequence generator by Jonas Karlsson from source: https://oeis.org/A392177/a392177_2.py.txt

From Sloane: 

> Consider the square spiral with its cells numbered starting at 0... Two players, Black and Red, take turns. When it is Black's turn, he places a knight at the smallest unoccupied cell not attacked by an existing Red knight, and when it is Red's turn, she places a knight at the smallest unoccupied cell not attacked by an existing Black knight.

This version experiments with 2-6 players all using "knights" using movement rules as defined by Władysław Gliński.

The initial experiment starts simply, with a hexagonal grid and two players. This first iteration has each player make 10 moves. 

![2p 10^1](renders/2p_spiral_chess_hex_10_1.png)

This is the board at 100 moves each:

![2p 10^2](renders/2p_spiral_chess_hex_10_2.png)

An interesting interference pattern emerges at 10^3 moves each:

![2p 10^3](renders/2p_spiral_chess_hex_10_3.png)

At 10^4, the board appears to be settled, with the two opponents having claimed their halves and establishing a no-man's-land strip in between territories. 

![2p 10^4](renders/2p_spiral_chess_hex_10_4.png)

At 10^5, the pattern appears to hold indefinitely. Of interest is the diagonal spike of black extending to the upper right edge of the board; unknown if this ever resolves or continues to infinity. 

![2p 10^5](renders/2p_spiral_chess_hex_10_5.png)

Potential improvements: 
* Modification is clunky with larger numbers of players. Automating consistent marker sizing and spacing would be convenient for reusability.
* Performance becomes problematic above 10^5. A different approach could allow larger renders.

Future versions:
* Implement different pieces with different movement rules
* Play with other underlying polygons, particularly interested in decagons/pentagons but this would probably require a very different implementation. 
