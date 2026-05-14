# hex chess
Python program that renders outcomes for "chess" pieces on a hexagonal spiral board. 

Inspired by Numberphile video https://youtu.be/UiX4CFIiegM?si=jhmuTZc7iJi_M-BX

Based on the concept by N.J.A. Sloane and the sequence generator by Jonas Karlsson from source: https://oeis.org/A392177/a392177_2.py.txt

Potential improvements: 
* Modification is clunky with larger numbers of players. Automating consistent marker sizing and spacing would be convenient for reusability.
* Performance becomes problematic above 10^5. A different approach could allow larger renders.

This version experiments with 2-6 players all using "knights" using movement rules as defined by Władysław Gliński.

Future versions:
* Implement different pieces with different movement rules
* Play with other underlying polygons, particularly interested in decagons/pentagons but this would probably require a very different implementation. 
