# 2024-ExamSysNumBouticheAbdelrahmen
On commence par tester la liaison UART en affichant un texte sur la console
Ensuite on teste la communication avec le capteur, etant donne que les pin A0 A1 ET A2 sont relies a la masse, l'adresse du capteur est 0x48 qu'on decalera de 1 vers la gauche
Si on a un HAL OK on continue, on fait un MEM_READ sur le registre ou on souhaite recuperer la temperature, etant donne qu'on veut le registre pour la temperature ambiante, le registe vaut 0x00.
Une fois qu'on a les donnes brut, il faut les convertir en temperature lisible
