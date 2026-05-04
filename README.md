# Sujet :
Le projet ft_printf consiste à réimplémenter la fonction C printf, permettant d'afficher du texte formaté dans le terminal. <br>

Il faut gérer l'affichage d'une chaîne de caractères avec des modificateurs de format tel que :

| Format | Description |
|---|---|
| `%c` | Imprimer un seul caractère. |
| `%s` | Imprimer une chaîne de caractères. |
| `%p` | Imprimer un pointeur void * en format hexadécimal. |
| `%d` | Imprimer un nombre décimal (base 10). |
| `%i` | Imprimer un entier en base 10. |
| `%u` | Imprimer un nombre décimal non signé (base 10). |
| `%x` | Imprimer un nombre en format hexadécimal en lettres minuscules (base 16). |
| `%X` | Imprimer un nombre en format hexadécimal en lettres majuscules (base 16). |
| `%%` | Imprimer un signe de pourcentage. |

# Fonctionnement :
- Parcours la chaine de caractère jusqu'au '\0'
- Si le caractère actuel égale %, i++ qui fait passer au caractère suivant
- Check_format est la fonction qui permet de savoir quel format sera affiché sur le terminal
- Ce qu'il se trouve avant ou après le % est simplement affiché tel quel

# Exemple d'affichage :

| Format | Exemple |
|---|---|
| `Lettre : A` | ft_printf("Lettre : %c\n", 'A'); |
| `Chaîne : Bonjour` | ft_printf("Chaîne : %s\n", "Bonjour"); |
| `void *ptr = (void *)0x1234abcd` | ft_printf("Pointeur : %p\n", ptr); |
| `Décimal : 42` | ft_printf("Décimal : %d\n", 42); |
| `Entier : -42` | t_printf("Entier : %i\n", -42); |
| `Unsigned : 3000000000` | ft_printf("Unsigned : %u\n", 3000000000); |
| `Hex min : ff <br>` | ft_printf("Hex min : %x\n", 255); |
| `Hex maj : FF` | ft_printf("Hex maj : %X\n", 255); |
| `Pourcentage : %` | ft_printf("Pourcentage : %%\n"); |
