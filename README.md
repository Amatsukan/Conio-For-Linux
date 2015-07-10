conio.h
CONIO.H UTILIZANDO OS RECURSOS DA BIBLIOTECA NCURSES     



 A conio.h, como eu disse, é uma ncurses "disfarçada", portanto, você terá que instalar a biblioteca ncurses. Existem diversos artigos neste site que falam dos poderes dessa biblioteca. Dê uma olhada.

Para utilizar a conio.h, copie o código da página anterior e salve em /usr/include/conio.h.

Para que as funções da conio funcionem, você deve incluir no início de seu código C:

-**initconio();**

e no fim do código:

-**endconio();** //Não se esqueça de colocar essa linha, senão seu shell vai ficar meu esquisito quando sair do seu programa!

Na hora de compilar seu programa, você deve especificar a biblioteca ncurses, exemplo:

--*    # gcc meuprog.c -o ~/bin/meuprog -lncurses

Detalhe importante: Algumas funções da biblioteca stdio.h não irão funcionar com a conio.h, é o caso de printf() e scanf(), por exemplo. Para contornar o problema, você pode utilizar as funções printw() e scanw() da ncurses, que dá no mesmo!







DESENVOLVIDO POR: JEFFERSON DOS SANTOS FELIX, ABRIL 2004 
