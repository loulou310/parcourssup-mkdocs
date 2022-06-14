# Convertisseur basse 2, 10 et 16
Pour ce projet, il nous avait été fourni une page HTML formatée avec Bootstrap. Sur cette page, il y avait 3 champs correspondant aux 3 bases, ainsi qu’un bouton « convertir » permettant de lancer la conversion vers les 2 autres bases. Le but de ce projet était de traduire des fonctions de conversion écrites en Python en JavaScript

Voici le code de quelques fonctions du fichier

```js title="Convertion d'un nombre décimal en JavaScript"
function decBin(n) {
    let s=""

    if(n === 0) {
        return 0
    }
    else {
        while(n != 0) {
            if (n%2 === 0) {
                s = "0" + s
                n = n/2
            }
            else {
                s = "1" + s
                n = (n-1)/2
            }
        }
        return s
    }
```

```js title="Convertion d'un nombre binaire vers un nombre décimal"
function binDec(n) {
    let longueur = n.length
    let result = 0
    for(let i = 0 ; i < longueur; i++) {
        result = result + parseInt(n.charAt(i)) * 2 ** (longueur - (i + 1))
    }
    return result
}
```

```js title="Conversion d'un nombre décimal en hexadécimal"
function decHex(n) {
    let result =""
    while(n != 0) {
        reste = n%16
        result = hexMap.get(reste) + result // hexMap est une Map qui associe chaque caractère hexadécimal à un nombre.
        n = Math.floor(n/16)
    }
    return result
}
```

<a href="./convertisseur/index.html">Y accéder</a>