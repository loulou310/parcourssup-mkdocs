# Morpion

Le but de ce projet était de créer un morpion dans le terminal avec Python. Le jeu est jouable à 2 joueurs, sur le même ordinateur. Le code est découpé en 4 fonctions, ainsi qu'un code principal.

```py
def dessine(grille:list) -> None:
    """
    Dessine la grille dans la console
    """
    print( "     a     b     c   ")
    print( "   _____ _____ _____ ")
    print( "  |     |     |     |")
    print(f"1 |  {grille[0][0]}  |  {grille[0][1]}  |  {grille[0][2]}  |")
    print( "  |_____|_____|_____|")
    print( "  |     |     |     |")
    print(f"2 |  {grille[1][0]}  |  {grille[1][1]}  |  {grille[1][2]}  |")
    print( "  |_____|_____|_____|")
    print( "  |     |     |     |")
    print(f"3 |  {grille[2][0]}  |  {grille[2][1]}  |  {grille[2][2]}  |")
    print( "  |_____|_____|_____|")

```