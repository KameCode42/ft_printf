![FT_PRINTF](https://github.com/user-attachments/assets/05be681d-d5c3-4edc-adaf-ca76656be458)

# Sujet :
Le projet ft_printf consiste à réimplémenter la fonction C printf, permettant d'afficher du texte formaté dans le terminal.

Il faut gérer l'affichage d'une chaîne de caractères avec des modificateurs de format tel que :
%c : Imprimer un seul caractère. <br>
%s : Imprimer une chaîne de caractères. <br>
%p : Imprimer un pointeur void * en format hexadécimal. <br>
%d : Imprimer un nombre décimal (base 10). <br>
%i : Imprimer un entier en base 10. <br>
%u : Imprimer un nombre décimal non signé (base 10). <br>
%x : Imprimer un nombre en format hexadécimal en lettres minuscules (base 16). <br>
%X : Imprimer un nombre en format hexadécimal en lettres majuscules (base 16). <br>
%% : Imprimer un signe de pourcentage. <br>

# Exemple d'affichage :
ft_printf("Lettre : %c\n", 'A'); // Lettre : A

ft_printf("Chaîne : %s\n", "Bonjour"); // Chaîne : Bonjour

void *ptr = (void *)0x1234abcd;
ft_printf("Pointeur : %p\n", ptr); // Pointeur : 0x1234abcd

ft_printf("Décimal : %d\n", 42); // Décimal : 42

ft_printf("Entier : %i\n", -42); // Entier : -42

ft_printf("Unsigned : %u\n", 3000000000); // Unsigned : 3000000000

ft_printf("Hex min : %x\n", 255); // Hex min : ff

ft_printf("Hex maj : %X\n", 255); // Hex maj : FF

ft_printf("Pourcentage : %%\n"); // Pourcentage : %
