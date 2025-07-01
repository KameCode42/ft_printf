![FT_PRINTF](https://github.com/user-attachments/assets/05be681d-d5c3-4edc-adaf-ca76656be458)

# Sujet :
Le projet ft_printf consiste à réimplémenter la fonction C printf, permettant d'afficher du texte formaté dans le terminal. <br>

Il faut gérer l'affichage d'une chaîne de caractères avec des modificateurs de format tel que : <br>
`%c` : Imprimer un seul caractère. <br>
`%s` : Imprimer une chaîne de caractères. <br>
`%p` : Imprimer un pointeur void * en format hexadécimal. <br>
`%d` : Imprimer un nombre décimal (base 10). <br>
`%i` : Imprimer un entier en base 10. <br>
`%u` : Imprimer un nombre décimal non signé (base 10). <br>
`%x` : Imprimer un nombre en format hexadécimal en lettres minuscules (base 16). <br>
`%X` : Imprimer un nombre en format hexadécimal en lettres majuscules (base 16). <br>
`%%`: Imprimer un signe de pourcentage. <br>

# Fonctionnement
- Parcours la chaine de caractère jusqu'au '\0'
- Si le caractère actuel égale %, i++ qui fait passer au caractère suivant
- Check_format est la fonction qui permet de savoir quel format sera affiché sur le terminal
- Ce qu'il se trouve avant ou après le % est simplement affiché tel quel

<br>

# Exemple d'affichage :
Lettre : A <br>
ft_printf("Lettre : %c\n", 'A'); <br>

Chaîne : Bonjour <br>
ft_printf("Chaîne : %s\n", "Bonjour"); <br>

void *ptr = (void *)0x1234abcd <br>
ft_printf("Pointeur : %p\n", ptr); <br>

Décimal : 42 <br>
ft_printf("Décimal : %d\n", 42); <br>

Entier : -42 <br>
ft_printf("Entier : %i\n", -42); <br>

Unsigned : 3000000000 <br>
ft_printf("Unsigned : %u\n", 3000000000); <br>

Hex min : ff <br>
ft_printf("Hex min : %x\n", 255); <br>

Hex maj : FF <br>
ft_printf("Hex maj : %X\n", 255); <br>

Pourcentage : % <br>
ft_printf("Pourcentage : %%\n"); <br>
