#include <stdio.h>
#include <stdlib.h>
#include <windows.h>

// \033[1;37m - COR BRANCA
// \033[1;31m - COR VERMELHO
// \033[1;32m - COR VERDE
// \033[38;2;204;204;0m - COR AMARELA
// \033[1;34m - COR AZUL
// \033[38;2;139;0;0m - COR VERMELHO (CORAí”ŒO)
// \033[38;2;255;105;180m - COR ROSA(TITULO)

void gotoxy(int x, int y){
  COORD coord;
  coord.X = x;
  coord.Y = y;
  SetConsoleCursorPosition(GetStdHandle(STD_OUTPUT_HANDLE), coord);
}

void telaApresentacao(){
    printf("              %c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c\n",201,205, 205, 205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,187);
    printf("              %c                                                           %c\n", 186, 186);
	printf("  $$$$  $$$   %c                                                           %c   $$$$  $$$\n", 186, 186);
	printf(" $$$$$$$$$$$  %c                                                           %c  $$$$$$$$$$$ \n", 186, 186);
	printf("  $$$$$$$$$   %c                                                           %c   $$$$$$$$$\n", 186, 186);
	printf("    $$$$$     %c                                                           %c     $$$$$\n", 186, 186);
	printf("     $$$      %c         ____                                ____          %c      $$$\n",186, 186);
	printf("              %c       _(____)_                            _(____)_        %c      \n", 186, 186);
	printf("              %c       |______|             ----           |______|        %c\n", 186, 186);
	printf("              %c        /    \\             ------           /    \\         %c\n", 186, 186);
	printf("     ---      %c       /    %c \\          LUDO-MANIA        /    %c \\        %c      ---\n", 186,248, 248, 186);
	printf("              %c      /      \\ \\           ------         /      \\ \\       %c\n", 186, 186);
	printf("              %c     /        \\ \\           ----         /        \\ \\      %c\n", 186, 186);
	printf("              %c   _/____________\\_                    _/____________\\_    %c\n", 186, 186);
	printf("  $$$$  $$$   %c  |________________|                  |________________|   %c   $$$$  $$$\n", 186, 186);
	printf(" $$$$$$$$$$$  %c                                                           %c  $$$$$$$$$$$ \n", 186, 186);
	printf("  $$$$$$$$$   %c                                                           %c   $$$$$$$$$\n", 186, 186);
    printf("    $$$$$     %c                                                           %c     $$$$$\n", 186, 186);
	printf("     $$$      %c                  De um 'enter' para continuar             %c      $$$\n", 186, 186);
	printf("              %c                                                           %c\n", 186, 186);
	printf("              %c                                                           %c\n", 186, 186);
	printf("              %c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c\n",200,205, 205, 205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,188);

//titulo  //ROSA
    gotoxy(42 ,8);
    printf("\033[38;2;255;105;180m ----");
    gotoxy(41,9);
    printf("\033[38;2;255;105;180m ------");
    gotoxy(39 ,10);
    printf("\033[38;2;255;105;180m LUDO-MANIA");
    gotoxy(41,11);
    printf("\033[38;2;255;105;180m ------");
    gotoxy(42 ,12);
    printf("\033[38;2;255;105;180m ----");

//PINO 1 //Amarelo
    gotoxy(23, 6);
    printf("\033[38;2;204;204;0m ____");
    gotoxy(21, 7);
    printf("\033[38;2;204;204;0m _(    )_");
    gotoxy(21, 8);
    printf("\033[38;2;204;204;0m |______|");
    gotoxy(22, 9);
    printf("\033[38;2;204;204;0m /    \\");
    gotoxy(21, 10);
    printf("\033[38;2;204;204;0m /    %c \\",248 );
    gotoxy(20, 11);
    printf("\033[38;2;204;204;0m /      \\ \\");
    gotoxy(19, 12);
    printf("\033[38;2;204;204;0m /        \\ \\");
    gotoxy(17, 13);
    printf("\033[38;2;204;204;0m _/____________\\_");
    gotoxy(16, 14);
    printf("\033[38;2;204;204;0m |________________|");

//pino 2 //AZUL
    gotoxy(59, 6);
    printf("\033[1;34m ____");
    gotoxy(57, 7);
    printf("\033[1;34m _(    )_");
    gotoxy(57, 8);
    printf("\033[1;34m |______|");
    gotoxy(58, 9);
    printf("\033[1;34m /    \\");
    gotoxy(57, 10);
    printf("\033[1;34m /    %c \\", 248);
    gotoxy(56, 11);
    printf("\033[1;34m /      \\ \\");
    gotoxy(55, 12);
    printf("\033[1;34m /        \\ \\");
    gotoxy(53, 13);
    printf("\033[1;34m _/____________\\_");
    gotoxy(52, 14);
    printf("\033[1;34m |________________|");

//pino 3  //VERMELHO
    gotoxy(30, 7);
    printf("\033[1;31m __");
    gotoxy(32, 8);
    printf("\033[1;31m )_");
    gotoxy(29, 9);
    printf("\033[1;31m ____|");
    gotoxy(32, 10);
    printf("\033[1;31m  \\");
    gotoxy(32, 11);
    printf("\033[1;31m %c \\",248 );
    gotoxy(34, 12);
    printf("\033[1;31m\\ \\");
    gotoxy(35, 13);
    printf("\033[1;31m\\ \\");
    gotoxy(35, 14);
    printf("\033[1;31m___\\_");
    gotoxy(23, 15);
    printf("\033[1;31m|________________|");

//pino 4  //Verde
    gotoxy(54, 7);
    printf("\033[1;32m __");
    gotoxy(52, 8);
    printf("\033[1;32m _( ");
    gotoxy(52, 9);
    printf("\033[1;32m |____");
    gotoxy(53, 10);
    printf("\033[1;32m / ");
    gotoxy(52, 11);
    printf("\033[1;32m / ", 248);
    gotoxy(51, 12);
    printf("\033[1;32m / ");
    gotoxy(50, 13);
    printf("\033[1;32m / ");
    gotoxy(48, 14);
    printf("\033[1;32m _/__");
    gotoxy(47, 15);
    printf("\033[1;32m |________________|");

//coraÃ§Ã£o 1
    gotoxy(2,2);
	printf("\033[38;2;255;105;180m$$$$  $$$");
	gotoxy(1,3);
	printf("\033[38;2;255;105;180m$$$$$$$$$$$");
	gotoxy(2,4);
	printf("\033[38;2;255;105;180m$$$$$$$$$");
	gotoxy(4,5);
	printf("\033[38;2;255;105;180m$$$$$");
	gotoxy(5,6);
	printf("\033[38;2;255;105;180m$$$");

//coraÃ§Ã£o 2
    gotoxy(2,14);
	printf("\033[38;2;255;105;180m$$$$  $$$");
	gotoxy(1,15);
	printf("\033[38;2;255;105;180m$$$$$$$$$$$");
	gotoxy(2,16);
	printf("\033[38;2;255;105;180m$$$$$$$$$");
	gotoxy(4,17);
	printf("\033[38;2;255;105;180m$$$$$");
	gotoxy(5,18);
	printf("\033[38;2;255;105;180m$$$");

//coraÃ§Ã£o 3
    gotoxy(78,2);
	printf("\033[38;2;255;105;180m$$$$  $$$");
	gotoxy(77,3);
	printf("\033[38;2;255;105;180m$$$$$$$$$$$");
	gotoxy(78,4);
	printf("\033[38;2;255;105;180m$$$$$$$$$");
	gotoxy(80,5);
	printf("\033[38;2;255;105;180m$$$$$");
	gotoxy(81,6);
	printf("\033[38;2;255;105;180m$$$");

//coraÃ§Ã£o 3
    gotoxy(78,14);
	printf("\033[38;2;255;105;180m$$$$  $$$");
	gotoxy(77,15);
	printf("\033[38;2;255;105;180m$$$$$$$$$$$");
	gotoxy(78,16);
	printf("\033[38;2;255;105;180m$$$$$$$$$");
	gotoxy(80,17);
	printf("\033[38;2;255;105;180m$$$$$");
	gotoxy(81,18);
	printf("\033[38;2;255;105;180m$$$");
    printf("\033[1;37m");

    getch();
    system("cls");
}
void telaMenu(){
    int resposta=0;
    system("CLS");

    printf("             %c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c\n",201,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,187);
	printf("             %c                                                         %c\n", 186, 186);
	printf("  $$$$  $$$  %c                                                         %c   $$$$  $$$\n", 186, 186);
	printf(" $$$$$$$$$$$ %c                                                         %c  $$$$$$$$$$$\n", 186, 186);
	printf("  $$$$$$$$$  %c                                                         %c   $$$$$$$$$\n", 186, 186);
	printf("    $$$$$    %c                                                         %c     $$$$$\n", 186, 186);
	printf("     $$$     %c                       LUDO-MANIA                        %c      $$$\n", 186, 186);
	printf("             %c                         ------                          %c\n", 186, 186);
	printf("             %c                          ----                           %c\n", 186, 186);
	printf("             %c                                                         %c\n", 186, 186);
	printf("     ---     %c                     1- CADASTRAR JOGADORES              %c      ---\n", 186, 186);
	printf("             %c                     2- VISUALIZAR RANKING               %c\n", 186, 186);
	printf("             %c                     3- AJUDA                            %c\n", 186, 186);
	printf("             %c                     4- SAIR                             %c\n", 186, 186);
	printf("  $$$$  $$$  %c                                                         %c   $$$$  $$$\n", 186, 186);
	printf(" $$$$$$$$$$$ %c                                                         %c  $$$$$$$$$$$\n", 186, 186);
	printf("  $$$$$$$$$  %c                                                         %c   $$$$$$$$$\n", 186, 186);
	printf("    $$$$$    %c                                                         %c     $$$$$\n", 186, 186);
	printf("     $$$     %c                                                         %c      $$$\n", 186, 186);
	printf("             %c                                                         %c\n", 186, 186);
	printf("             %c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c\n",200,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,188);

//titulo
    gotoxy(36, 6);
    printf("\033[38;2;255;105;180m LUDO-MANIA");
    gotoxy(38, 7);
    printf("\033[38;2;255;105;180m ------");
    gotoxy(39, 8);
    printf("\033[38;2;255;105;180m ----");

//numeraÃ§Ã£o
    gotoxy(34, 10);
    printf("\033[38;2;255;105;180m 1-");
    gotoxy(34, 11);
    printf("\033[38;2;255;105;180m 2-");
    gotoxy(34, 12);
    printf("\033[38;2;255;105;180m 3-");
    gotoxy(34, 13);
    printf("\033[38;2;255;105;180m 4-");

//coraÃ§Ã£o 1
    gotoxy(2,2);
	printf("\033[38;2;255;105;180m$$$$  $$$");
	gotoxy(1,3);
	printf("\033[38;2;255;105;180m$$$$$$$$$$$");
	gotoxy(2,4);
	printf("\033[38;2;255;105;180m$$$$$$$$$");
	gotoxy(4,5);
	printf("\033[38;2;255;105;180m$$$$$");
	gotoxy(5,6);
	printf("\033[38;2;255;105;180m$$$");
//coraÃ§Ã£o 2
    gotoxy(2,14);
	printf("\033[38;2;255;105;180m$$$$  $$$");
	gotoxy(1,15);
	printf("\033[38;2;255;105;180m$$$$$$$$$$$");
	gotoxy(2,16);
	printf("\033[38;2;255;105;180m$$$$$$$$$");
	gotoxy(4,17);
	printf("\033[38;2;255;105;180m$$$$$");
	gotoxy(5,18);
	printf("\033[38;2;255;105;180m$$$");
//coraÃ§Ã£o 3
    gotoxy(75,2);
	printf("\033[38;2;255;105;180m$$$$  $$$");
	gotoxy(74,3);
	printf("\033[38;2;255;105;180m$$$$$$$$$$$");
	gotoxy(75,4);
	printf("\033[38;2;255;105;180m$$$$$$$$$");
	gotoxy(77,5);
	printf("\033[38;2;255;105;180m$$$$$");
	gotoxy(78,6);
	printf("\033[38;2;255;105;180m$$$");
//coraÃ§Ã£o 4
    gotoxy(75,14);
	printf("\033[38;2;255;105;180m$$$$  $$$");
	gotoxy(74,15);
	printf("\033[38;2;255;105;180m$$$$$$$$$$$");
	gotoxy(75,16);
	printf("\033[38;2;255;105;180m$$$$$$$$$");
	gotoxy(77,17);
	printf("\033[38;2;255;105;180m$$$$$");
	gotoxy(78,18);
	printf("\033[38;2;255;105;180m$$$");
    printf("\033[1;37m");

    gotoxy(32, 17);
    printf("Digite sua op%c%co aqui:\033[1;37m", 135, 198);
    scanf("%i", &resposta);

    if(resposta==1){
        system("cls");
        telaCadastrarJogadores();{
        }
    }
    if(resposta==2){
        system("cls");
        telaVisualizarRankig();{
        }
    }
    if(resposta==3){
        system("cls");
        telaAjuda();{
        }
    }
    if(resposta==4){
        system("cls");
        telaAgradecimento();{
        }
    }
}
// struct global (na estrutura) para o void cadastrar
struct Usuario{
	char nome[100];
};
struct Usuario jogador;
struct Usuario jogadores[10];

void telaCadastrarJogadores(){

    char nome[10];
    int resposta=0;
    int cont=0;

    printf("             %c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c\n",201,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,187);
    printf("             %c                                                         %c\n", 186, 186);
    printf("  $$$$  $$$  %c                       LUDO-MANIA                        %c  $$$$  $$$\n", 186, 186);
    printf(" $$$$$$$$$$$ %c                         ------                          %c $$$$$$$$$$$\n", 186, 186);
    printf("  $$$$$$$$$  %c                       JOGADORES                         %c  $$$$$$$$$\n", 186, 186);
    printf("    $$$$$    %c                                                         %c    $$$$$\n", 186, 186);
    printf("     $$$     %c                                                         %c     $$$\n", 186, 186);
    printf("             %c                                                         %c\n", 186, 186);
    printf("             %c                                                         %c\n", 186, 186);
    printf("             %c              (!com menos de 10 caracteres!)             %c\n", 186, 186);
    printf("     ---     %c                                                         %c     ---\n", 186, 186);
    printf("             %c                                                         %c\n", 186, 186);
    printf("             %c           JOGADOR(A) 1:                                 %c\n", 186, 186);
    printf("             %c                                                         %c\n", 186, 186);
    printf("  $$$$  $$$  %c           JOGADOR(A) 2:                                 %c  $$$$  $$$\n", 186, 186);
    printf(" $$$$$$$$$$$ %c                                                         %c $$$$$$$$$$$\n", 186, 186);
    printf("  $$$$$$$$$  %c           JOGADOR(A) 3:                                 %c  $$$$$$$$$\n", 186, 186);
    printf("    $$$$$    %c                                                         %c    $$$$$\n", 186, 186);
    printf("     $$$     %c           JOGADOR(A) 4:                                 %c     $$$\n", 186, 186);
    printf("             %c                                                         %c\n", 186, 186);
    printf("             %c                                                         %c\n", 186, 186);
    printf("             %c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c\n",200,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,188);

    gotoxy(87, 19);
    printf("%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c\n", 201, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 187);
    gotoxy(87, 20);
    printf("%c 5- VOLTA PARA %c\n", 186, 186);
    gotoxy(87, 21);
    printf("%c      O MENU   %c\n", 186, 186);
    gotoxy(87, 22);
    printf("%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c\n", 200, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 188);

//TITULO
    gotoxy(36, 2);
    printf("\033[38;2;255;105;180m LUDO-MANIA");
    gotoxy(38, 3);
    printf("\033[1;37m ------");
    gotoxy(31, 4);
    printf("\033[38;2;255;105;180m CADASTRAR JOGADORES");

//CORA?O 1
    gotoxy(0, 2);
    printf("\033[38;2;255;105;180m  $$$$  $$$  ");
    gotoxy(0, 3);
    printf("\033[38;2;255;105;180m $$$$$$$$$$$ ");
    gotoxy(0, 4);
    printf("\033[38;2;255;105;180m  $$$$$$$$$  ");
    gotoxy(0, 5);
    printf("\033[38;2;255;105;180m    $$$$$    ");
    gotoxy(0, 6);
    printf("\033[38;2;255;105;180m     $$$     ");

//CORA?O 2
    gotoxy(0, 14);
    printf("\033[38;2;255;105;180m  $$$$  $$$  ");
    gotoxy(0, 15);
    printf("\033[38;2;255;105;180m $$$$$$$$$$$ ");
    gotoxy(0, 16);
    printf("\033[38;2;255;105;180m  $$$$$$$$$  ");
    gotoxy(0, 17);
    printf("\033[38;2;255;105;180m    $$$$$    ");
    gotoxy(0, 18);
    printf("\033[38;2;255;105;180m     $$$     ");

//CORA?O 3
    gotoxy(72, 2);
    printf("\033[38;2;255;105;180m  $$$$  $$$  ");
    gotoxy(72, 3);
    printf("\033[38;2;255;105;180m $$$$$$$$$$$ ");
    gotoxy(72, 4);
    printf("\033[38;2;255;105;180m  $$$$$$$$$  ");
    gotoxy(72, 5);
    printf("\033[38;2;255;105;180m    $$$$$    ");
    gotoxy(72, 6);
    printf("\033[38;2;255;105;180m     $$$     ");

//CORA?O 4
    gotoxy(72, 14);
    printf("\033[38;2;255;105;180m  $$$$  $$$  ");
    gotoxy(72, 15);
    printf("\033[38;2;255;105;180m $$$$$$$$$$$ ");
    gotoxy(72, 16);
    printf("\033[38;2;255;105;180m  $$$$$$$$$  ");
    gotoxy(72, 17);
    printf("\033[38;2;255;105;180m    $$$$$    ");
    gotoxy(72, 18);
    printf("\033[38;2;255;105;180m     $$$     ");

//INFORMA?ES DA TELA
    gotoxy(28, 9);
    printf("\033[1;37m(!com menos de 10 caracteres!)");
    gotoxy(25, 12);
    printf("\033[1;31mJOGADOR(A) 1:");
    gotoxy(25, 14);
    printf("\033[1;32mJOGADOR(A) 2:");
    gotoxy(25, 16);
    printf("\033[38;2;204;204;0mJOGADOR(A) 3:");
    gotoxy(25, 18);
    printf("\033[1;34mJOGADOR(A) 4:");
    gotoxy(54, 20);
    printf("\033[1;37m8-PR%cXIMO", 224);

    for(cont=0; cont<=5; cont++){
        gotoxy(24,7);
        printf("\033[1;37mEscolha sua cor: \033[1;37m1-\033[1;31m%c  \033[1;37m2-\033[1;32m%c  \033[1;37m3-\033[38;2;204;204;0m%c  \033[1;37m4-\033[1;34m%c \033[1;37m:", 254, 254, 254, 254);
        scanf("%i", &resposta);
        if (resposta ==1){
            gotoxy(39, 12);
            printf("\033[1;31m%c");
            gets(jogadores[1].nome); // onde vai guardar a informaÃ§Ã£o
            fflush (stdin);
            gets(jogadores[1].nome);
            getch();
        }
        if (resposta==2){
            gotoxy(39, 14);
            printf("\033[1;32m%c");
            gets(jogadores[2].nome); // onde vai guardar a informaÃ§Ã£o
            fflush (stdin);
            gets(jogadores[2].nome);
            getch();
        }
        if (resposta ==3){
            gotoxy(39, 16);
            printf("\033[38;2;204;204;0m%c");
            gets(jogadores[3].nome); // onde vai guardar a informaÃ§Ã£o
            fflush (stdin);
            gets(jogadores[3].nome);
            getch();
        }
        if (resposta==4){
            gotoxy(39, 18);
            printf("\033[1;34m%c");
            gets(jogadores[4].nome); // onde vai guardar a informaÃ§Ã£o
            fflush (stdin);
            gets(jogadores[4].nome);
            getch();
        }
        if (resposta == 5){
           system("CLS");
           telaMenu();
           getch();
        }
        if(resposta ==8){
           system("CLS");
            telaVisualizarNiveis();
            getch();
        }
    }//fecha foR
}
void telaVisualizarNiveis(){
    int linha=0;
    int coluna=0;
    int alternativa=0;

    //L= 93 C= 22
    printf("             %c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c\n",201,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,187);
    printf("             %c                                                               %c\n", 186, 186);
    printf("             %c                           LUDO-MANIA                          %c\n", 186, 186);
    printf("             %c                             -----                             %c\n", 186, 186);
    printf("  $$$$  $$$  %c                            N%cVEIS                             %c  $$$$  $$$\n", 186, 214, 186);
    printf(" $$$$$$$$$$$ %c         _____________________    _____________________        %c $$$$$$$$$$$\n", 186, 186);
    printf("  $$$$$$$$$  %c        |_|_|_|_|_|_|_|_|_|_|_|  |_|_|_|_|_|_|_|_|_|_|_|       %c  $$$$$$$$$\n", 186, 186);
    printf("    $$$$$    %c        |_| @   @ |_| @   @ |_|  |_|_|_  @  @  @  _|_|_|       %c    $$$$$\n", 186, 186);
    printf("     $$$     %c        |_|   @   |_|   @   |_|  |_| |_|_ @  @  _|_| |_|       %c     $$$\n", 186, 186);
    printf("             %c        |_| @   @ |_| @   @ |_|  |_|@  |_|_ @ _|_|  @|_|       %c\n", 186, 186);
    printf("             %c        |_|_ _ _ _|_|_ _ _ _|_|  |_|  @  |_|_|_|  @  |_|       %c\n", 186, 186);
    printf("     ---     %c        |_|_|_|_|_|_|_|_|_|_|_|  |_|@   @ _|_|_ @   @|_|       %c     ---\n", 186, 186);
    printf("             %c        |_| @   @ |_| @   @ |_|  |_|  @ _|_| |_|_ @  |_|       %c\n", 186, 186);
    printf("             %c        |_|   @   |_|   @   |_|  |_|@ _|_|  @  |_|_ @|_|       %c\n", 186, 186);
    printf("  $$$$  $$$  %c        |_| @   @ |_| @   @ |_|  |_|_|_|   @  @  |_|_|_|       %c  $$$$  $$$\n", 186, 186);
    printf(" $$$$$$$$$$$ %c        |_|_ _ _ _|_|_ _ _ _|_|  |_|_|_ _@ _@ _@_ _|_|_|       %c $$$$$$$$$$$\n", 186, 186);
    printf("  $$$$$$$$$  %c        |_|_|_|_|_|_|_|_|_|_|_|  |_|_|_|_|_|_|_|_|_|_|_|       %c  $$$$$$$$$ \n", 186, 186);
    printf("    $$$$$    %c                                                               %c    $$$$$\n", 186, 186);
    printf("     $$$     %c                N%cVEL 1                 N%cVEL 2                %c     $$$\n", 186, 214, 214, 186);
    printf("             %c                                                               %c\n", 186, 186);
    printf("             %c                    Digite aqui sua op%c%co:                     %c\n", 186,135, 198, 186);
    printf("             %c                                                               %c\n", 186, 186);
    printf("             %c                                                               %c\n", 186, 186);
    printf("             %c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c\n",200,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,188);

    gotoxy(15, 24);
    printf("%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c\n", 201, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 187);
    gotoxy(15, 25);
    printf("%c 5- VOLTA PARA %c\n", 186, 186);
    gotoxy(15, 26);
    printf("%c      O MENU   %c\n", 186, 186);
    gotoxy(15, 27);
    printf("%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c\n", 200, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 188);

//TITULO
    gotoxy(40,2);
    printf("\033[38;2;255;105;180m LUDO-MANIA");
    gotoxy(42,3);
    printf("\033[38;2;255;105;180m -----");
    gotoxy(42, 4);
    printf("\033[38;2;255;105;180m N%cVEIS", 214);

    gotoxy(29 ,18);
    printf("\033[38;2;255;105;180m N%cVEL 1", 214);
    gotoxy(53, 18);
    printf("\033[1;30m N%cVEL 2", 214);
    
    gotoxy(54,11);
    printf("\033[1;31m'EM BREVE'");

//coraÃ§ao 1
	gotoxy(2,4);
	printf("\033[38;2;255;105;180m$$$$  $$$");
	gotoxy(1,5);
	printf("\033[38;2;255;105;180m$$$$$$$$$$$");
	gotoxy(2,6);
	printf("\033[38;2;255;105;180m$$$$$$$$$");
	gotoxy(4,7);
	printf("\033[38;2;255;105;180m$$$$$");
	gotoxy(5,8);
	printf("\033[38;2;255;105;180m$$$");
//coraÃ§Ã£o 2
	gotoxy(2,14);
	printf("\033[38;2;255;105;180m$$$$  $$$");
	gotoxy(1,15);
	printf("\033[38;2;255;105;180m$$$$$$$$$$$");
	gotoxy(2,16);
	printf("\033[38;2;255;105;180m$$$$$$$$$");
	gotoxy(4,17);
	printf("\033[38;2;255;105;180m$$$$$");
	gotoxy(5,18);
	printf("\033[38;2;255;105;180m$$$");
//coraÃ§Ã£o 3
	gotoxy(80,4);
	printf("\033[38;2;255;105;180m$$$$  $$$");
	gotoxy(79,5);
	printf("\033[38;2;255;105;180m$$$$$$$$$$$");
	gotoxy(80,6);
	printf("\033[38;2;255;105;180m$$$$$$$$$");
	gotoxy(82,7);
	printf("\033[38;2;255;105;180m$$$$$");
	gotoxy(83,8);
	printf("\033[38;2;255;105;180m$$$");
//coraÃ§Ã£o 4
	gotoxy(80,14);
	printf("\033[38;2;255;105;180m$$$$  $$$");
	gotoxy(79,15);
	printf("\033[38;2;255;105;180m$$$$$$$$$$$");
	gotoxy(80,16);
	printf("\033[38;2;255;105;180m$$$$$$$$$");
	gotoxy(82,17);
	printf("\033[38;2;255;105;180m$$$$$");
	gotoxy(83,18);
	printf("\033[38;2;255;105;180m$$$");

//PINO AMARELO // ELEMENTOS AMARELO (TABULEIRO 2)
    gotoxy(26, 12);
    printf("\033[38;2;204;204;0m3");
    gotoxy(30, 12);
    printf("\033[38;2;204;204;0m3");
    gotoxy(28, 13);
    printf("\033[38;2;204;204;0m3");
    gotoxy(26, 14);
    printf("\033[38;2;204;204;0m3");
    gotoxy(30, 14);
    printf("\033[38;2;204;204;0m3");

	gotoxy(33, 11);
	printf("\033[1;37m%c",254);
    gotoxy(33, 12);
	printf("\033[38;2;204;204;0m%c",254);
    gotoxy(33, 13);
	printf("\033[38;2;204;204;0m%c",254);
    gotoxy(33, 14);
	printf("\033[38;2;204;204;0m%c",254);
    gotoxy(33, 15);
	printf("\033[38;2;204;204;0m%c",254);
    gotoxy(35, 16);
	printf("\033[38;2;204;204;0m%c",254);

//PINO AMARELO // ELEMENTOS AMARELO (TABULEIRO 3)
    gotoxy(50, 9);
    printf("\033[1;30m4");
    gotoxy(50, 11);
    printf("\033[1;30m4");
    gotoxy(50, 13);
    printf("\033[1;30m4");
    gotoxy(52, 12);
    printf("\033[1;30m4");
    gotoxy(52, 10);
    printf("\033[1;30m4");

    gotoxy(48, 16);
	printf("\033[1;30m%c",254);
    gotoxy(50, 15);
	printf("\033[1;30m%c",254);
    gotoxy(52, 14);
	printf("\033[1;30m%c",254);
    gotoxy(54, 13);
	printf("\033[1;30m%c",254);
    gotoxy(56, 12);
	printf("\033[1;30m%c",254);


//PINO VERDE // ELEMENTOS VERDE (TABULEIRO 2)
    gotoxy(36, 12);
    printf("\033[1;32m4");
    gotoxy(40, 12);
    printf("\033[1;32m4");
    gotoxy(38, 13);
    printf("\033[1;32m4");
    gotoxy(36, 14);
    printf("\033[1;32m4");
    gotoxy(40, 14);
    printf("\033[1;32m4");

    gotoxy(43, 12);
	printf("\033[1;32m%c",254);
    gotoxy(41, 11);
	printf("\033[1;32m%c", 254);
    gotoxy(39, 11);
	printf("\033[1;32m%c",254);
    gotoxy(37, 11);
	printf("\033[1;32m%c",254);
    gotoxy(35, 11);
	printf("\033[1;32m%c",254);

//PINO VERDE // ELEMENTOS VERDE (TABULEIRO 3)
    gotoxy(58, 13);
    printf("\033[1;30m3");
    gotoxy(60, 14);
    printf("\033[1;30m3");
    gotoxy(57, 14);
    printf("\033[1;30m3");
    gotoxy(55, 15);
    printf("\033[1;30m3");
    gotoxy(58, 15);
    printf("\033[1;30m3");
    gotoxy(61, 15);
    printf("\033[1;30m3");

    gotoxy(60, 12);
	printf("\033[1;30m%c", 254);
    gotoxy(62, 13);
	printf("\033[1;30m%c",254);
    gotoxy(64, 14);
	printf("\033[1;30m%c",254);
    gotoxy(66, 15);
	printf("\033[1;30m%c",254);
    gotoxy(68, 16);
	printf("\033[1;30m%c",254);

//PINO AZUL //ELEMENTOS AZUL (TABULEIRO 2)
    gotoxy(36, 7);
    printf("\033[1;34m2");
    gotoxy(40, 7);
    printf("\033[1;34m2");
    gotoxy(38, 8);
    printf("\033[1;34m2");
    gotoxy(36, 9);
    printf("\033[1;34m2");
    gotoxy(40, 9);
    printf("\033[1;34m2");

    gotoxy(35, 6);
	printf("\033[1;34m%c",254);
    gotoxy(33, 7);
	printf("\033[1;34m%c",254);
    gotoxy(33, 8);
	printf("\033[1;34m%c",254);
    gotoxy(33, 9);
	printf("\033[1;34m%c",254);
    gotoxy(33, 10);
	printf("\033[1;34m%c",254);

//PINO AZUL  // ELEMENTOS AZUL (TABULEIRO 3)
    gotoxy(66, 9);
    printf("\033[1;30m2");
    gotoxy(66, 11);
    printf("\033[1;30m2");
    gotoxy(66, 13);
    printf("\033[1;30m2");
    gotoxy(64, 12);
    printf("\033[1;30m2");
    gotoxy(64, 10);
    printf("\033[1;30m2");

    gotoxy(68, 6);
	printf("\033[1;30m%c",254);
    gotoxy(66, 7);
	printf("\033[1;30m%c",254);
    gotoxy(64, 8);
	printf("\033[1;30m%c",254);
    gotoxy(62, 9);
	printf("\033[1;30m%c",254);
    gotoxy(60, 10);
	printf("\033[1;30m%c",254);

//PINO VERMELHO // ELEMENTOS VERMELHO(TABULEIRO 2)
    gotoxy(26, 7);
    printf("\033[1;31m1");
    gotoxy(30, 7);
    printf("\033[1;31m1");
    gotoxy(28, 8);
    printf("\033[1;31m1");
    gotoxy(26, 9);
    printf("\033[1;31m1");
    gotoxy(30, 9);
    printf("\033[1;31m1");

    gotoxy(31, 11);
	printf("\033[1;31m%c",254);
    gotoxy(29, 11);
	printf("\033[1;31m%c", 254);
    gotoxy(27, 11);
	printf("\033[1;31m%c",254);
    gotoxy(25, 11);
	printf("\033[1;31m%c",254);
    gotoxy(23, 12);
	printf("\033[1;31m%c",254);

//PINO VERMELHO // ELEMENTOS VERMELHO(TABULEIRO 3)
    gotoxy(55, 7);
    printf("\033[1;30m1");
    gotoxy(58, 7);
    printf("\033[1;30m1");
    gotoxy(61, 7);
    printf("\033[1;30m1");
    gotoxy(56, 8);
    printf("\033[1;30m1");
    gotoxy(59, 8);
    printf("\033[1;30m1");
    gotoxy(58, 9);
    printf("\033[1;30m1");

    gotoxy(48, 6);
	printf("\033[1;30m%c", 254);
    gotoxy(50, 7);
	printf("\033[1;30m%c",254);
    gotoxy(52, 8);
	printf("\033[1;30m%c",254);
    gotoxy(54, 9);
	printf("\033[1;30m%c",254);
    gotoxy(56, 10);
	printf("\033[1;30m%c",254);
    printf("\033[1;37m");

    gotoxy(56, 20);
    scanf("%i", &alternativa);
        if(alternativa==1){
            telaSegundoNivel();
            getch();
        }
        if(alternativa==2){
            gotoxy(26, 21);
            printf("\033[1;31mOp%c%co ainda n%co valida, tente novamente!\033[1;37m", 135, 198, 198); //mostra resposta
            getch();
            system("cls"); // limpa a tela anterior
            telaVisualizarNiveis(); //mostra a tela de novo
            getch();
        }
        if(alternativa==5){
            telaMenu();
            getch();
        }

//FINAL
    gotoxy(1, 29);
    getch();
}
void telaSegundoNivel(){
    system("CLS");

    srand(time(NULL)); //FAZ O DADO FUNCIONAR
    int linha, coluna=0;
    char MATRIZ[87][27];
    int coluna_tela=0;
    int dado, dado1, dado2, dado3, dado4=0; //1=R1, 2=B1, 3=Y1, 4=G1
    int jogo_valendo=1;
    int escolher_jogador=0; //comeÃ§a com o primeiro jogador (o vermelho)
    int opcao=0;
    char nickname1[11];//nomes
    char nickname2[11];
    char nickname3[11];
    char nickname4[11];

        printf("             %c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c\n", 201, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 187);
        printf("             %c                                                         %c\n", 186, 186);
        printf("             %c                        LUDO-MANIA                       %c\n", 186, 186);
        printf("  $$$$  $$$  %c                          ------                         %c  $$$$  $$$\n", 186, 186);
        printf(" $$$$$$$$$$$ %c                                                         %c $$$$$$$$$$$\n", 186, 186);
        printf("  $$$$$$$$$  %c                                                         %c  $$$$$$$$$\n", 186, 186);
        printf("    $$$$$    %c                                                         %c    $$$$$\n", 186, 186);
        printf("     $$$     %c   __________________________________________________    %c     $$$\n", 186, 186);
        printf("             %c  |      __ __ __ __ __ __ __ __ __ __ __ __ __      |   %c\n", 186, 186);
        printf("             %c  |     |__|__|__|__|__|__|__|__|__|__|__|__|__|     |   %c\n", 186, 186);
        printf("             %c  |     |__|           |__|__|__|           |__|     |   %c\n", 186, 186);
        printf("             %c  |     |__|  1     1  |__|__|__|  2     2  |__|     |   %c\n", 186, 186);
        printf("             %c  |     |__|     1     |__|__|__|     2     |__|     |   %c\n", 186, 186);
        printf("             %c  |     |__|  1     1  |__|__|__|  2     2  |__|     |   %c\n", 186, 186);
        printf("     ---     %c  |     |__|__ __ __ __|__|__|__|__ __ __ __|__|     |   %c     ---\n", 186, 186);
        printf("             %c  |     |__|__|__|__|__|        |__|__|__|__|__|     |   %c\n", 186, 186);
        printf("             %c  |     |__|__|__|__|__|        |__|__|__|__|__|     |   %c\n", 186, 186);
        printf("             %c  |     |__|__|__|__|__|__ __ __|__|__|__|__|__|     |   %c\n", 186, 186);
        printf("             %c  |     |__|           |__|__|__|           |__|     |   %c\n", 186, 186);
        printf("             %c  |     |__|  3     3  |__|__|__|  4     4  |__|     |   %c\n", 186, 186);
        printf("  $$$$  $$$  %c  |     |__|     3     |__|__|__|     4     |__|     |   %c  $$$$  $$$\n", 186, 186);
        printf(" $$$$$$$$$$$ %c  |     |__|  3     3  |__|__|__|  4     4  |__|     |   %c $$$$$$$$$$$\n", 186, 186);
        printf("  $$$$$$$$$  %c  |     |__|__ _____ __|__|__|__|__ __ __ __|__|     |   %c  $$$$$$$$$\n", 186, 186);
        printf("    $$$$$    %c  |     |__|__|__|__|__|__|__|__|__|__|__|__|__|     |   %c    $$$$$\n", 186, 186);
        printf("     $$$     %c  |__________________________________________________|   %c     $$$\n", 186, 186);
        printf("             %c                                                         %c\n", 186, 186);
        printf("             %c                                                         %c\n", 186, 186);
        printf("             %c                        N%cVEL 1                          %c\n", 186, 214, 186);
        printf("             %c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c\n", 200, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 188);

    gotoxy(87, 8);
    printf("%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c\n", 201,205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 187);
    gotoxy(87, 9);
    printf("%c                              %c\n", 186, 186);
    gotoxy(87, 10);
    printf("%c    METAS DE CADA JOGADOR:    %c\n", 186, 186);
    gotoxy(87, 11);
    printf("%c                              %c\n", 186, 186);
    gotoxy(87, 12);
    printf("%c      CHEGAR A CASA COM O     %c\n", 186, 186);
    gotoxy(87, 13);
    printf("%c      ELEMENTO BRANCO!!!      %c\n", 186, 186);
    gotoxy(87, 14);
    printf("%c              %c               %c\n", 186, 254, 186);
    gotoxy(87, 15);
    printf("%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c\n", 200,205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 188);

    gotoxy(87, 19);
    printf("%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c\n", 201, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 187);
    gotoxy(87, 20);
    printf("%c 5- VOLTA PARA %c\n", 186, 186);
    gotoxy(87, 21);
    printf("%c      O MENU   %c\n", 186, 186);
    gotoxy(87, 22);
    printf("%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c\n", 200, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 188);

    gotoxy(87, 23);
    printf("%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c\n", 201, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 187);
    gotoxy(87, 24);
    printf("%c  8- SAIR DO  %c\n", 186, 186);
    gotoxy(87, 25);
    printf("%c      JOGO    %c\n", 186, 186);
    gotoxy(87, 26);
    printf("%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c\n", 200,205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 188);

//PINOS VERMELHOS
    gotoxy(27, 11);
    printf("\033[1;31mR1");
    gotoxy(34, 11);
    printf("\033[1;31mR2");
    gotoxy(31, 12);
    printf("\033[1;31mR3");
    gotoxy(34, 13);
    printf("\033[1;31mR4");
    gotoxy(27, 13);
    printf("\033[1;31mR5");

//PINOS AZUIS
    gotoxy(48, 11);
    printf("\033[1;34mB1");
    gotoxy(54, 11);
    printf("\033[1;34mB2");
    gotoxy(51, 12);
    printf("\033[1;34mB3");
    gotoxy(54, 13);
    printf("\033[1;34mB4");
    gotoxy(48, 13);
    printf("\033[1;34mB5");

//PINOS AMARELOS
    gotoxy(27, 19);
    printf("\033[38;2;204;204;0mY1");
    gotoxy(34, 19);
    printf("\033[38;2;204;204;0mY2");
    gotoxy(31, 20);
    printf("\033[38;2;204;204;0mY3");
    gotoxy(34, 21);
    printf("\033[38;2;204;204;0mY4");
    gotoxy(27, 21);
    printf("\033[38;2;204;204;0mY5");

//PINOS VERDES
    gotoxy(48, 19);
    printf("\033[1;32mG1");
    gotoxy(54, 19);
    printf("\033[1;32mG2");
    gotoxy(51, 20);
    printf("\033[1;32mG3");
    gotoxy(54, 21);
    printf("\033[1;32mG4");
    gotoxy(48, 21);
    printf("\033[1;32mG5");

//coraÃ§Ãµes
	gotoxy(2,3);
	printf("\033[38;2;255;105;180m$$$$  $$$");
	gotoxy(1,4);
	printf("\033[38;2;255;105;180m$$$$$$$$$$$");
	gotoxy(2,5);
	printf("\033[38;2;255;105;180m$$$$$$$$$");
	gotoxy(4,6);
	printf("\033[38;2;255;105;180m$$$$$");
	gotoxy(5,7);
	printf("\033[38;2;255;105;180m$$$");

//2Â°coraÃ§Ã£o da esquerda
	gotoxy(2,20);
	printf("\033[38;2;255;105;180m$$$$  $$$");
	gotoxy(1,21);
	printf("\033[38;2;255;105;180m$$$$$$$$$$$");
	gotoxy(2,22);
	printf("\033[38;2;255;105;180m$$$$$$$$$");
	gotoxy(4,23);
	printf("\033[38;2;255;105;180m$$$$$");
	gotoxy(5,24);
	printf("\033[38;2;255;105;180m$$$");

//coraÃ§Ã£o da direita
	gotoxy(74,3);
	printf("\033[38;2;255;105;180m$$$$  $$$");
	gotoxy(73,4);
	printf("\033[38;2;255;105;180m$$$$$$$$$$$");
	gotoxy(74,5);
	printf("\033[38;2;255;105;180m$$$$$$$$$");
	gotoxy(76,6);
	printf("\033[38;2;255;105;180m$$$$$");
	gotoxy(77,7);
	printf("\033[38;2;255;105;180m$$$");

//2Â°coraÃ§Ã£o da direita
	gotoxy(74,20);
	printf("\033[38;2;255;105;180m$$$$  $$$");
	gotoxy(73,21);
	printf("\033[38;2;255;105;180m$$$$$$$$$$$");
	gotoxy(74,22);
	printf("\033[38;2;255;105;180m$$$$$$$$$");
	gotoxy(76,23);
	printf("\033[38;2;255;105;180m$$$$$");
	gotoxy(77,24);
	printf("\033[38;2;255;105;180m$$$");

//elementos vermelho
	gotoxy(23,17);
	printf("\033[1;31m%c",175);
	gotoxy(23,16);
	printf("\033[1;31mE");

	coluna_tela=26;
	for(coluna=26; coluna<30; coluna++){
		linha=16;
		gotoxy(coluna_tela, linha);
		printf("\033[1;31m%c",254);
		coluna_tela= coluna_tela +3;
	}
//elemento em azul
	gotoxy(38,9);
	printf("\033[1;34m%c",175);
	gotoxy(41,10);
	printf("\033[1;34mE");
	coluna_tela=41;
	for(linha=11; linha<15; linha++){
		gotoxy(coluna_tela, linha);
		printf("\033[1;34m%c",254);
		linha + 1;
	}
//elemento em amarelo
	gotoxy(44,23);
	printf("\033[38;2;204;204;0m%c", 175);
	gotoxy(42,22);
	printf("\033[38;2;204;204;0mE");

	coluna_tela=42;
	for(linha=18; linha<22; linha++){
		gotoxy(coluna_tela, linha);
		printf("\033[38;2;204;204;0m%c",254);
		linha + 1;
	}
//elemento verde
	gotoxy(59,14);
	printf("\033[1;32m%c",174);
	gotoxy(59,16);
	printf("\033[1;32mE");

	coluna_tela=47;
	for(coluna=47; coluna<51; coluna++){
		linha=16;
		gotoxy(coluna_tela, linha);
		printf("\033[1;32m%c",254);
		coluna_tela= coluna_tela +3;
	}

//elementos brancos
    gotoxy(38 ,16); //meta do vemelho
    printf("\033[1;37m%c",254);
    gotoxy(45 ,16); //meta do azul
    printf("\033[1;37m%c",254);
    gotoxy(42 ,15); //meta do amarelo
    printf("\033[1;37m%c",254);
    gotoxy(41 ,17); //meta do verde
    printf("\033[1;37m%c",254);

//nomes
    gotoxy(22,6);
    printf("\033[1;31m"); //vermelho
	puts(jogadores[1].nome);
    gotoxy(53,6);
    printf("\033[1;34m"); //azul
	puts(jogadores[2].nome);
    gotoxy(22,25);
    printf("\033[38;2;204;204;0m"); // amarela
	puts(jogadores[3].nome);
    gotoxy(53,25);
    printf("\033[1;32m"); //verde
	puts(jogadores[4].nome);

//dado=(rand() %6)+1; (conta do dado)
    escolher_jogador=4;
    while(jogo_valendo !=0){
        for(jogo_valendo=1; jogo_valendo <= escolher_jogador; jogo_valendo++){ //VERIFICA QUEM TA VEZ DE JOGAR
            dado=(rand() %6)+1;
            gotoxy(87, 16);
            printf("Vez do jogador %i", jogo_valendo);

            if(jogo_valendo == 1){
                gotoxy(22,6);
                printf("\033[1;31m");
                puts(jogadores[1].nome);
                getch();
                gotoxy(37,5);
                dado1=(rand() %6)+1;
                printf("Dado: %i\n", dado1);
                getch();
                if(dado1 == 6){ // se tirar 6 a peÃ§a vermelha vai sair da base
                    gotoxy(27, 11); //sai da base
                    printf("\033[1;31mR1");
                    Sleep(100); // ajuda a nÃ£o ficar dando enter para continuar andando
                    gotoxy(27, 11); //apaga
                    printf("\033[1;31m  ");
                    Sleep(100);

                    coluna_tela=26;
                    for(coluna=26; coluna<= 29; coluna++){//anda as 4 primeiras casas
                        linha=15;
                        gotoxy(coluna_tela, linha);
                        printf("\033[1;31mR1");
                        Sleep(200);
                        gotoxy(coluna_tela, linha);
                        printf("\033[1;37m__");
                        coluna_tela= coluna_tela +3;
                        Sleep(200);
                    }//fecha for
                        gotoxy(38, 14);
                        printf("\033[1;31mR1");//andas as duas ultimas casinhas para completar 6 casas
                        Sleep(200);
                        gotoxy(38, 14);
                        printf("\033[1;37m__");
                        Sleep(200);

                        gotoxy(38, 13);
                        printf("\033[1;31mR1");
                }
            }

            if(jogo_valendo == 2){
                gotoxy(53,6);
                printf("\033[1;34m");
                puts(jogadores[2].nome);
                getch();
                gotoxy(37,5);
                dado2=(rand() %6)+1;
                printf("Dado: %i\n",dado2);
                getch();
                if(dado2 == 6){ // se tirar 6 a peÃ§a azul vai sair da base
                    gotoxy(48, 11);//tira a peÃ§a da base
                    printf("\033[1;34mB1");
                    Sleep(200);
                    gotoxy(48, 11);//apaga
                    printf("\033[1;34m  ");
                    Sleep(200);

                    coluna_tela=44;
                    for(linha=13; linha>=9; linha--){ //anda as 5 primeiras casas
                        gotoxy(coluna_tela, linha);
                        printf("\033[1;34mB1");
                        Sleep(200);
                        gotoxy(coluna_tela, linha);
                        printf("\033[1;37m__");
                        linha-1;
                        Sleep(200);
                    } //FECHA FOR 1
                        gotoxy(47,9);
                        printf("\033[1;34mB1"); //anda mais 1 para fechar as 6 casas
                }
            }
            if(jogo_valendo ==3){
                gotoxy(22,25);
                printf("\033[38;2;204;204;0m");
                puts(jogadores[3].nome);
                gotoxy(37,5);
                dado3=(rand() %6)+1;
                printf("Dado: %i\n",dado3);
                getch();
                if(dado3 == 6){ // se tirar 6 a peÃ§a amarela vai sair da base
                    gotoxy(27, 19);//tira a peÃ§a da base
                    printf("\033[38;2;204;204;0mY1");
                    Sleep(200);
                    gotoxy(27, 19);//apaga
                    printf("\033[38;2;204;204;0m  ");
                    Sleep(200);
                    }
                    coluna_tela=38;
                    for(linha=19; linha<24; linha++){ //anda as 5 primeiras casas
                        gotoxy(coluna_tela, linha);
                        printf("\033[38;2;204;204;0mY1");
                        Sleep(200);
                        gotoxy(coluna_tela, linha);
                        printf("\033[1;37m__");
                        linha-1;
                        Sleep(200);
                    }//FECHAR FOR
                        gotoxy(35, 23);
                        printf("\033[38;2;204;204;0mY1"); //anda mais uma pra completar 6
                }
            }
            if(jogo_valendo == 4){
                gotoxy(53,25);
                printf("\033[1;32m");
                puts(jogadores[4].nome);
                gotoxy(37,5);
                dado4=(rand() %6)+1;
                printf("Dado: %i\n",dado4);
                getch();
                if(dado4 == 6){ // se tirar 6 a peÃ§a verde vai sair da base
                    gotoxy(48, 19); //tira a peÃ§a da base
                    printf("\033[1;32mG1");
                    Sleep(200);
                    gotoxy(48, 19); //apaga
                    printf("\033[1;32m  ");
                    Sleep(200);

                    coluna_tela=50;
                    for(coluna=50; coluna<54; coluna++){//anda as 4 primeiras casas
                        linha=17;
                        gotoxy(coluna_tela, linha);
                        printf("\033[1;32mG1");
                        Sleep(200);
                        gotoxy(coluna_tela, linha);
                        printf("\033[1;37m__");
                        coluna_tela= coluna_tela +3;
                        Sleep(200);
                    }//fecha for
                        gotoxy(59, 18);
                        printf("\033[1;32mG1");//andas as duas ultimas casinhas para completar 6 casas
                        Sleep(200);
                        gotoxy(59, 18);
                        printf("\033[1;37m__");
                        Sleep(200);
                        gotoxy(59, 19);
                        printf("\033[1;32mG1");
                }

            }
        }//for

    if(opcao==5){
        telaMenu();
        getch();
    }
    else if(opcao==8){
        telaAgradecimento();
    }
}
void telaVisualizarRankig(){
    char nickname1[11];
    char nickname2[11];
    char nickname3[11];
    char nickname4[11];
    int volta_menu=0;

    system("CLS");
    printf("             %c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c\n",201,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,187);
    printf("             %c                                                                                            %c\n",186,186);
    printf("             %c                                                                                            %c\n",186,186);
    printf("  $$$$  $$$  %c                                        LUDO-MANIA                                          %c  $$$$  $$$\n",186,186);
    printf(" $$$$$$$$$$$ %c                                          ------                                            %c $$$$$$$$$$$\n",186,186);
    printf("  $$$$$$$$$  %c                                          RANKING                                           %c  $$$$$$$$$\n",186,186);
    printf("    $$$$$    %c                                                                                            %c    $$$$$\n",186,186);
    printf("     $$$     %c                                                                                            %c     $$$\n",186,186);
    printf("             %c        ___________________________________________________________________________         %c\n",186,186);
    printf("             %c       |                                                          Vencedores       |        %c\n",186,186);
    printf("             %c       |      _ 1%c_                                        |                       |        %c\n",186, 248,186);
    printf("     ---     %c       |     |     |                                       | 1%cLugar:              |        %c     ---\n",186,248,186);
    printf("             %c       |     |     |      _ 2%c_                            |                       |        %c\n",186, 248, 186);
    printf("             %c       |     |     |     |     |                           | 2%cLugar:              |        %c\n",186,248,186);
    printf("             %c       |     |     |     |     |      _ 3%c_                |                       |        %c\n",186, 248,186);
    printf("  $$$$  $$$  %c       |     |     |     |     |     |     |               | 3%cLugar:              |        %c  $$$$  $$$\n",186,248,186);
    printf(" $$$$$$$$$$$ %c       |     |     |     |     |     |     |      _ 4%c_    |                       |        %c $$$$$$$$$$$\n",186, 248,186);
    printf("  $$$$$$$$$  %c       |     |     |     |     |     |     |     |     |   | 4%cLugar:              |        %c  $$$$$$$$$\n",186,248,186);
    printf("    $$$$$    %c       |_____|_____|_____|_____|_____|_____|_____|_____|___________________________|        %c    $$$$$\n",186,186);
    printf("     $$$     %c                                                                                            %c     $$$\n",186,186);
    printf("             %c                                                                                            %c\n",186,186);
    printf("             %c                                                                                            %c\n",186,186);
    printf("             %c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c\n",200,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,188);

	gotoxy(15, 24);
    printf("%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c\n", 201, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 187);
    gotoxy(15, 25);
    printf("%c 5- VOLTA PARA %c\n", 186, 186);
    gotoxy(15, 26);
    printf("%c      O MENU   %c\n", 186, 186);
    gotoxy(15, 27);
    printf("%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c\n", 200, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 205, 188);

//titulo
    gotoxy(53, 3);
    printf("\033[38;2;255;105;180m LUDO-MANIA");
    gotoxy(55, 4);
    printf("\033[38;2;255;105;180m ------");
    gotoxy(55, 5);
    printf("\033[38;2;255;105;180m RANKING");
    gotoxy(80,9);
    printf("\033[38;2;255;105;180mVencedores");
    gotoxy(75,11);
    printf("\033[38;2;255;105;180m1%c", 248);
    gotoxy(75,13);
    printf("\033[38;2;255;105;180m2%c", 248);
    gotoxy(75,15);
    printf("\033[38;2;255;105;180m3%c", 248);
    gotoxy(75,17);
    printf("\033[38;2;255;105;180m4%c", 248);
//Nome jogadores
		gotoxy(83,11);
		printf("%c", nickname1[11]);
		gotoxy(83,13);
		printf("%c", nickname2[11]);
		gotoxy(83,15);
		printf("%c", nickname3[11]);
		gotoxy(83,17);
		printf("%c", nickname4[11]);
//CORAÃ‡ÃƒO1
	gotoxy(2,3);
	printf("\033[38;2;255;105;180m$$$$  $$$");
	gotoxy(1,4);
	printf("\033[38;2;255;105;180m$$$$$$$$$$$");
	gotoxy(2,5);
	printf("\033[38;2;255;105;180m$$$$$$$$$");
	gotoxy(4,6);
	printf("\033[38;2;255;105;180m$$$$$");
	gotoxy(5,7);
	printf("\033[38;2;255;105;180m$$$");
//CORAÃ‡ÃƒO2
	gotoxy(2,15);
	printf("\033[38;2;255;105;180m$$$$  $$$");
	gotoxy(1,16);
	printf("\033[38;2;255;105;180m$$$$$$$$$$$");
	gotoxy(2,17);
	printf("\033[38;2;255;105;180m$$$$$$$$$");
	gotoxy(4,18);
	printf("\033[38;2;255;105;180m$$$$$");
	gotoxy(5,19);
	printf("\033[38;2;255;105;180m$$$");
//CORAÃ‡ÃƒO3
	gotoxy(109,3);
	printf("\033[38;2;255;105;180m$$$$  $$$");
	gotoxy(108,4);
	printf("\033[38;2;255;105;180m$$$$$$$$$$$");
	gotoxy(109,5);
	printf("\033[38;2;255;105;180m$$$$$$$$$");
	gotoxy(111,6);
	printf("\033[38;2;255;105;180m$$$$$");
	gotoxy(112,7);
	printf("\033[38;2;255;105;180m$$$");
//CORAÃ‡ÃƒO4
	gotoxy(109,15);
	printf("\033[38;2;255;105;180m$$$$  $$$");
	gotoxy(108,16);
	printf("\033[38;2;255;105;180m$$$$$$$$$$$");
	gotoxy(109,17);
	printf("\033[38;2;255;105;180m$$$$$$$$$");
	gotoxy(111,18);
	printf("\033[38;2;255;105;180m$$$$$");
	gotoxy(112,19);
	printf("\033[38;2;255;105;180m$$$");
    printf("\033[1;37m");

    gotoxy(33, 26);
    printf("  ");
    scanf("%i", &volta_menu);
	if(volta_menu==5){
		telaMenu();
        getch();
	}
}
void telaAjuda(){
int resposta=0;
    int cont=0;
    system("CLS");

    printf("             %c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c\n",201,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,187);
    printf("             %c                                                         %c\n", 186, 186);
    printf("  $$$$  $$$  %c                                                         %c  $$$$  $$$\n", 186, 186);
    printf(" $$$$$$$$$$$ %c                                                         %c $$$$$$$$$$$\n", 186, 186);
    printf("  $$$$$$$$$  %c                                                         %c  $$$$$$$$$\n", 186, 186);
    printf("    $$$$$    %c                                                         %c    $$$$$\n", 186, 186);
    printf("     $$$     %c                       LUDO-MANIA                        %c     $$$\n", 186, 186);
    printf("             %c                          ----                           %c\n", 186, 186);
    printf("             %c                         AJUDA                           %c\n", 186, 186);
    printf("             %c                                                         %c\n", 186, 186);
    printf("     ---     %c                                                         %c     ---\n", 186, 186);
    printf("             %c                      1- SEM SOM                         %c\n", 186, 186);
    printf("             %c                      2- SEM TOQUE                       %c\n", 186, 186);
    printf("             %c                      3- REGRAS GERAIS                   %c\n", 186, 186);
    printf("  $$$$  $$$  %c                      4- REGRAS DE N%cVEIS                %c  $$$$  $$$\n", 186,214, 186);
    printf(" $$$$$$$$$$$ %c                      5- VOLTAR AO MENU                  %c $$$$$$$$$$$\n", 186, 186);
    printf("  $$$$$$$$$  %c                                                         %c  $$$$$$$$$\n", 186, 186);
    printf("    $$$$$    %c                                                         %c    $$$$$\n", 186, 186);
    printf("     $$$     %c                                                         %c     $$$\n", 186, 186);
    printf("             %c                                                         %c\n", 186, 186);
    printf("             %c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c\n",200,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,188);
//TITULO
    gotoxy(36, 6);
    printf("\033[38;2;255;105;180m LUDO-MANIA");
    gotoxy(39, 7);
    printf("\033[38;2;255;105;180m ----");
    gotoxy(38, 8);
    printf("\033[38;2;255;105;180m AJUDA");

//NUMERAÃ‡ÃƒO
    gotoxy(35, 11);
    printf("\033[38;2;255;105;180m 1-");
    gotoxy(35, 12);
    printf("\033[38;2;255;105;180m 2-");
    gotoxy(35, 13);
    printf("\033[38;2;255;105;180m 3-");
    gotoxy(35, 14);
    printf("\033[38;2;255;105;180m 4-");
    gotoxy(35, 15);
    printf("\033[38;2;255;105;180m 5-");
    gotoxy(38, 11);
    printf("\033[1;32m SEM SOM");
    gotoxy(38, 12);
    printf("\033[1;32m SEM TOQUE");

//coraÃ§Ã£o 1
	gotoxy(2,2);
	printf("\033[38;2;255;105;180m$$$$  $$$");
	gotoxy(1,3);
	printf("\033[38;2;255;105;180m$$$$$$$$$$$");
	gotoxy(2,4);
	printf("\033[38;2;255;105;180m$$$$$$$$$");
	gotoxy(4,5);
	printf("\033[38;2;255;105;180m$$$$$");
	gotoxy(5,6);
	printf("\033[38;2;255;105;180m$$$");
//coraÃ§Ã£o 2
    gotoxy(2,14);
	printf("\033[38;2;255;105;180m$$$$  $$$");
	gotoxy(1,15);
	printf("\033[38;2;255;105;180m$$$$$$$$$$$");
	gotoxy(2,16);
	printf("\033[38;2;255;105;180m$$$$$$$$$");
	gotoxy(4,17);
	printf("\033[38;2;255;105;180m$$$$$");
	gotoxy(5,18);
	printf("\033[38;2;255;105;180m$$$");
//coraÃ§Ã£o 3
    gotoxy(74,2);
	printf("\033[38;2;255;105;180m$$$$  $$$");
	gotoxy(73,3);
	printf("\033[38;2;255;105;180m$$$$$$$$$$$");
	gotoxy(74,4);
	printf("\033[38;2;255;105;180m$$$$$$$$$");
	gotoxy(76,5);
	printf("\033[38;2;255;105;180m$$$$$");
	gotoxy(77,6);
	printf("\033[38;2;255;105;180m$$$");
//coraÃ§Ã£o 4
    gotoxy(74,14);
	printf("\033[38;2;255;105;180m$$$$  $$$");
	gotoxy(73,15);
	printf("\033[38;2;255;105;180m$$$$$$$$$$$");
	gotoxy(74,16);
	printf("\033[38;2;255;105;180m$$$$$$$$$");
	gotoxy(76,17);
	printf("\033[38;2;255;105;180m$$$$$");
	gotoxy(77,18);
	printf("\033[38;2;255;105;180m$$$");
    printf("\033[1;37m");

	for(cont=0; cont<=5; cont++){
	    gotoxy(32, 17);
	    printf("\033[1;37mDigite sua op%c%co aqui:\033[1;37m", 135, 198);
	    scanf("%i", &resposta);

	    if(resposta==1){
	        gotoxy(39, 11);
	        printf("\033[1;31mSEM SOM");
	    }
	    if(resposta==2){
	        gotoxy(39, 12);
	        printf("\033[1;31mSEM TOQUE");
	    }
	    if(resposta==3){
	        system("cls");
	        telaRegrasGerais();{
	        }
	    }
	    if(resposta==4){
	        system("cls");
	        telaInstrusoes();{
	        }
	    }
	    if(resposta==5){
	        system("cls");
	        telaMenu();{
	        }
    	}
    }
}
void telaRegrasGerais(){
    int l, c=0;
    int resposta=0;

	printf("\033[1;37m              %c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c\n",201,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,187);
    printf("              %c                                                                     %c\n", 186, 186);
	printf("              %c                             \033[38;2;255;105;180mLUDO MANIA\033[1;37m                              %c\n", 186, 186);
	printf("              %c                              \033[38;2;255;105;180m-------- \033[1;37m                              %c\n", 186, 186);
	printf("              %c                               \033[38;2;255;105;180m ---- \033[1;37m                                %c\n", 186, 186);
	printf("              %c                                                                     %c\n", 186, 186);
	printf("              %c                               \033[38;2;255;105;180mREGRAS\033[1;37m                                %c\n", 186, 186);
    printf("              %c                                                                     %c\n", 186, 186);
	printf(" \033[38;2;255;105;180m $$$$  $$$\033[1;37m   %c - Objetivo: Levar todos os 5, ou 6, pinos at%c o centro, dando a     %c \033[38;2;255;105;180m $$$$  $$$\033[1;37m\n", 186, 130, 186);
	printf("\033[38;2;255;105;180m $$$$$$$$$$$\033[1;37m  %c   volta em todo o tabuleiro antes do seu advers%crio.                %c \033[38;2;255;105;180m$$$$$$$$$$$\033[1;37m\n",186, 160, 186);
	printf(" \033[38;2;255;105;180m $$$$$$$$$\033[1;37m   %c                                                                     %c \033[38;2;255;105;180m $$$$$$$$$\033[1;37m\n", 186, 186);
	printf("\033[38;2;255;105;180m    $$$$$\033[1;37m     %c - Movimenta%c%co: os dados indicaram a quantidade de casas que os     %c   \033[38;2;255;105;180m $$$$$\033[1;37m\n", 186, 135, 198, 186);
	printf(" \033[38;2;255;105;180m    $$$\033[1;37m      %c   pinos devem andar.                                                %c    \033[38;2;255;105;180m $$$\033[1;37m\n", 186, 186);
    printf("              %c                                                                     %c\n", 186, 186);
	printf("              %c - Sorte: se os dados indicarem o n%cmero 6 a algum dos jogadores,    %c\n", 186, 151, 186);
	printf("              %c - este jogador poder%c retirar mais um de seus pinos da casa de      %c\n", 186, 160, 186);
	printf("     ---      %c   partida ou mover novamente o mesmo pino.                          %c     ---\n", 186, 186);
	printf("              %c                                                                     %c\n", 186, 186);
	printf("              %c - Elimina%c%ces: se o pino de jogador chegar a uma casa j%c ocupada o  %c\n", 186, 135, 228, 160, 186);
	printf("              %c   pino do advers%crio que estiver nesta casa, dever%c retorna para a  %c\n", 186, 160, 160, 186);
    printf(" \033[38;2;255;105;180m $$$$  $$$\033[1;37m   %c   casa de partida. Por%cm se os pinos forem do mesmo jogador, nada   %c \033[38;2;255;105;180m $$$$  $$$\033[1;37m\n", 186, 130, 186);
	printf("\033[38;2;255;105;180m $$$$$$$$$$$\033[1;37m  %c   acontece e a partida continua.                                    %c \033[38;2;255;105;180m$$$$$$$$$$$\033[1;37m\n", 186, 186);
	printf("\033[38;2;255;105;180m  $$$$$$$$$\033[1;37m   %c                                                                     %c \033[38;2;255;105;180m $$$$$$$$$\033[1;37m\n", 186, 186);
	printf(" \033[38;2;255;105;180m   $$$$$\033[1;37m     %c - %crea segura: se os pinos de diferentes jogadores chegarem a casa  %c    \033[38;2;255;105;180m$$$$$\033[1;37m\n", 186, 181, 186);
	printf(" \033[38;2;255;105;180m    $$$\033[1;37m      %c   '%c', nenhum pino %c eliminado. Estas s%co as unicas casas onde os   %c     \033[38;2;255;105;180m$$$\033[1;37m\n", 186, 174, 130, 198, 186);
	printf("              %c   advers%crios podem ocupar ao mesmo tempo.                          %c \n", 186, 160, 186);
	printf("              %c                                                                     %c\n", 186, 186);
	printf("              %c  - Entrada final: as casas sinalizas com a letra 'E', indicam a     %c\n", 186, 186);
	printf("              %c    entrada para a trilha final dos pinos, que os leva at%c o centro  %c\n", 186, 130, 186);
	printf("              %c    do tabuleiro.                                                    %c\n", 186, 186);
	printf("              %c                                                                     %c\n", 186, 186);
	printf("              %c                                                                     %c\n", 186, 186);
	printf("              %c                                                                     %c\n", 186, 186);
	printf("              %c  (Aperte '1' para acessar as regras dos niveis)                     %c\n", 186, 186);
	printf("              %c  (Aperte '2' para voltar para a Tela de Ajuda)                      %c\n", 186, 186);
	printf("              %c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c\n",200,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,188);
	getchar();

    scanf("%i", &resposta);
    if(resposta==1){
        system("CLS");
        telaInstrusoes();{
        }
    if(resposta==1){
        system("CLS");
        telaInstrusoes();{
        }
    }
}
}
void telaInstrusoes(){
    int l, c=0;
    int resposta=0;

    printf("\033[1;37m              %c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c\n",201,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,187);
    printf("              %c                                                                     %c\n", 186, 186);
	printf("              %c                             \033[38;2;255;105;180mLUDO MANIA\033[1;37m                              %c\n", 186, 186);
	printf("              %c                              \033[38;2;255;105;180m-------- \033[1;37m                              %c\n", 186, 186);
	printf("              %c                               \033[38;2;255;105;180m ---- \033[1;37m                                %c\n", 186, 186);
	printf("              %c                                                                     %c\n", 186, 186);
	printf("              %c                          \033[38;2;255;105;180m REGRAS DE N%cVEIS\033[1;37m                          %c\n", 186, 214, 186);
	printf("              %c                                                                     %c\n", 186, 186);
	printf(" \033[38;2;255;105;180m $$$$  $$$\033[1;37m   %c - N%cVEL 1: O tabuleiro segue o modelo tradicional de ludo em        %c \033[38;2;255;105;180m $$$$  $$$\033[1;37m\n", 186, 214, 186);
	printf("\033[38;2;255;105;180m $$$$$$$$$$$\033[1;37m  %c   formato de cruz, sua movimenta%c%co tamb%cm segue o modelo           %c \033[38;2;255;105;180m$$$$$$$$$$$\033[1;37m\n",186, 135, 198, 130, 186);
	printf(" \033[38;2;255;105;180m $$$$$$$$$\033[1;37m   %c   tradicional, sendo necess%crio dar a volta em toda a cruz para     %c \033[38;2;255;105;180m $$$$$$$$$\033[1;37m\n", 186, 160, 186);
	printf("\033[38;2;255;105;180m    $$$$$\033[1;37m     %c   poder chegar a trilha final.                                      %c   \033[38;2;255;105;180m $$$$$\033[1;37m\n", 186, 186);
	printf(" \033[38;2;255;105;180m    $$$\033[1;37m      %c                                                                     %c    \033[38;2;255;105;180m $$$\033[1;37m\n", 186, 186);
	printf("              %c - N%cVEL 2: Possui quase a mesma l%cgica do nivel anterior mas, ser%c  %c\n", 186, 214, 149, 160, 186);
	printf("              %c   necess%crio que os pinos percorram todo o caminho ao redor do      %c\n", 186, 160, 186);
	printf("              %c   tabuleiro, nas trilhas que contornam o tabuleiro, antes de        %c\n", 186, 186);
	printf("     ---      %c   chegarem as suas respectivas trilhas finais.                      %c     ---\n", 186, 186);
	printf("              %c                                                                     %c\n", 186, 186);
	printf("              %c - N%cVEL 3: Sua movimenta%c%co foge totalmente do tradicional, os      %c\n", 186, 214, 135, 198, 186);
	printf("              %c   pinos se movimentaram na diagonal e, como no nivel anterior,      %c\n", 186, 186);
    printf(" \033[38;2;255;105;180m $$$$  $$$\033[1;37m   %c   tamb%cm teram que percorrer o caminho ao redor do tabuleiro, neste %c \033[38;2;255;105;180m $$$$  $$$\033[1;37m\n", 186, 130, 186);
	printf("\033[38;2;255;105;180m $$$$$$$$$$$\033[1;37m  %c   nivel os jogadores tamb%cm teram um pino a mais, totalizando 6     %c \033[38;2;255;105;180m$$$$$$$$$$$\033[1;37m\n", 186, 130, 186);
	printf("\033[38;2;255;105;180m  $$$$$$$$$\033[1;37m   %c   pinos para cada jogador. Para que n%co ficasse t%co confuso, as     %c \033[38;2;255;105;180m $$$$$$$$$\033[1;37m\n", 186, 198, 198, 186);
	printf(" \033[38;2;255;105;180m   $$$$$\033[1;37m     %c   %creas que n%co seram percorridas est%co delimitadas no tabuleiro    %c    \033[38;2;255;105;180m$$$$$\033[1;37m\n", 186, 160, 198, 198, 186);
	printf(" \033[38;2;255;105;180m    $$$\033[1;37m      %c   com o seguinte simbolo: %c%c.                                       %c     \033[38;2;255;105;180m$$$\033[1;37m\n", 186, 177, 177, 186);
	printf("              %c                                                                     %c \n", 186, 186);
	printf("              %c                                                                     %c\n", 186, 186);
	printf("              %c     \033[38;2;255;105;180m Para qualquer d%cvida ou sugest%co, estaremos a disposi%c%co.\033[1;37m      %c\n", 186, 151, 198, 135, 198, 186);
	printf("              %c                                                                     %c\n", 186, 186);
	printf("              %c                           \033[38;2;255;105;180m BOM JOGO\033[1;37m                                 %c\n", 186, 186);
	printf("              %c                                                                     %c\n", 186, 186);
	printf("              %c                                                                     %c\n", 186, 186);
	printf("              %c                                                                     %c\n", 186, 186);
	printf("              %c  (Aperte '2' para retornar a tela de menu)                          %c\n", 186, 186);
	printf("              %c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c\n",200,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,188);
	getch();

    scanf("%i", &resposta);
    if(resposta==2){
        system("cls");
        telaMenu();{
        }
    }
}
void telaAgradecimento(){
    int l=0;
    int c=0;

    printf("              %c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c\n",201,205, 205, 205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,187);
    printf("              %c                                                           %c\n", 186, 186);
	printf("  $$$$  $$$   %c                                                           %c   $$$$  $$$\n", 186, 186);
	printf(" $$$$$$$$$$$  %c                                                           %c  $$$$$$$$$$$ \n", 186, 186);
	printf("  $$$$$$$$$   %c                                                           %c   $$$$$$$$$\n", 186, 186);
	printf("    $$$$$     %c                                                           %c     $$$$$\n", 186, 186);
	printf("     $$$      %c                                                           %c      $$$\n",186, 186);
	printf("              %c                                                           %c      \n", 186, 186);
	printf("              %c                                                           %c\n", 186, 186);
	printf("              %c                                                           %c\n", 186, 186);
	printf("     ---      %c                                                           %c      ---\n", 186, 186);
	printf("              %c                                                           %c\n", 186, 186);
	printf("              %c                                                           %c\n", 186, 186);
	printf("              %c                                                           %c\n", 186, 186);
	printf("  $$$$  $$$   %c                                                           %c   $$$$  $$$\n", 186, 186);
	printf(" $$$$$$$$$$$  %c                                                           %c  $$$$$$$$$$$ \n", 186, 186);
	printf("  $$$$$$$$$   %c                                                           %c   $$$$$$$$$\n", 186, 186);
    printf("    $$$$$     %c                                                           %c     $$$$$\n", 186, 186);
	printf("     $$$      %c                                                           %c      $$$\n", 186, 186);
	printf("              %c                           AT%c BREVE!                      %c\n", 186, 144, 186);
	printf("              %c                                                           %c\n", 186, 186);
	printf("              %c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c%c\n",200,205, 205, 205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,205,188);

//titulo  //ROSA
    gotoxy(36,2);
    printf("\033[38;2;255;105;180m O B R I G A D A");
    gotoxy(39 ,4);
    printf("\033[38;2;255;105;180m POR JOGAR");
    gotoxy(34,6);
    printf("\033[38;2;255;105;180m L U D O - M A N I A");
    gotoxy(40 ,7);
    printf("\033[38;2;255;105;180m ------");
    gotoxy(41 ,8);
    printf("\033[38;2;255;105;180m ----");

//PINO 1 //Amarelo
    gotoxy(23, 7);
    printf("\033[38;2;204;204;0m ____");
    gotoxy(21, 8);
    printf("\033[38;2;204;204;0m _(    )_");
    gotoxy(21, 9);
    printf("\033[38;2;204;204;0m |______|");
    gotoxy(22, 10);
    printf("\033[38;2;204;204;0m /    \\");
    gotoxy(21, 11);
    printf("\033[38;2;204;204;0m /    %c \\",248 );
    gotoxy(20, 12);
    printf("\033[38;2;204;204;0m /      \\ \\");
    gotoxy(19, 13);
    printf("\033[38;2;204;204;0m /        \\ \\");
    gotoxy(17, 14);
    printf("\033[38;2;204;204;0m _/____________\\_");
    gotoxy(16, 15);
    printf("\033[38;2;204;204;0m |________________|");

//pino 2 //AZUL
    gotoxy(59, 7);
    printf("\033[1;34m ____");
    gotoxy(57, 8);
    printf("\033[1;34m _(    )_");
    gotoxy(57, 9);
    printf("\033[1;34m |______|");
    gotoxy(58, 10);
    printf("\033[1;34m /    \\");
    gotoxy(57, 11);
    printf("\033[1;34m /    %c \\", 248);
    gotoxy(56, 12);
    printf("\033[1;34m /      \\ \\");
    gotoxy(55, 13);
    printf("\033[1;34m /        \\ \\");
    gotoxy(53, 14);
    printf("\033[1;34m _/____________\\_");
    gotoxy(52, 15);
    printf("\033[1;34m |________________|");

//pino 3  //VERMELHO
    gotoxy(30, 8);
    printf("\033[1;31m __");
    gotoxy(32, 9);
    printf("\033[1;31m )_");
    gotoxy(29, 10);
    printf("\033[1;31m ____|");
    gotoxy(32, 11);
    printf("\033[1;31m  \\");
    gotoxy(32, 12);
    printf("\033[1;31m %c \\",248 );
    gotoxy(34, 13);
    printf("\033[1;31m\\ \\");
    gotoxy(35, 14);
    printf("\033[1;31m\\ \\");
    gotoxy(35, 15);
    printf("\033[1;31m___\\_");
    gotoxy(23, 16);
    printf("\033[1;31m|________________|");

//pino 4  //Verde
    gotoxy(54, 8);
    printf("\033[1;32m __");
    gotoxy(52, 9);
    printf("\033[1;32m _( ");
    gotoxy(52, 10);
    printf("\033[1;32m |____");
    gotoxy(53, 11);
    printf("\033[1;32m / ");
    gotoxy(52, 12);
    printf("\033[1;32m / ", 248);
    gotoxy(51, 13);
    printf("\033[1;32m / ");
    gotoxy(50, 14);
    printf("\033[1;32m / ");
    gotoxy(48, 15);
    printf("\033[1;32m _/__");
    gotoxy(47, 16);
    printf("\033[1;32m |________________|");

//coraÃ§Ã£o 1
    gotoxy(2,2);
	printf("\033[38;2;255;105;180m$$$$  $$$");
	gotoxy(1,3);
	printf("\033[38;2;255;105;180m$$$$$$$$$$$");
	gotoxy(2,4);
	printf("\033[38;2;255;105;180m$$$$$$$$$");
	gotoxy(4,5);
	printf("\033[38;2;255;105;180m$$$$$");
	gotoxy(5,6);
	printf("\033[38;2;255;105;180m$$$");

//coraÃ§Ã£o 2
    gotoxy(2,14);
	printf("\033[38;2;255;105;180m$$$$  $$$");
	gotoxy(1,15);
	printf("\033[38;2;255;105;180m$$$$$$$$$$$");
	gotoxy(2,16);
	printf("\033[38;2;255;105;180m$$$$$$$$$");
	gotoxy(4,17);
	printf("\033[38;2;255;105;180m$$$$$");
	gotoxy(5,18);
	printf("\033[38;2;255;105;180m$$$");

//coraÃ§Ã£o 3
    gotoxy(78,2);
	printf("\033[38;2;255;105;180m$$$$  $$$");
	gotoxy(77,3);
	printf("\033[38;2;255;105;180m$$$$$$$$$$$");
	gotoxy(78,4);
	printf("\033[38;2;255;105;180m$$$$$$$$$");
	gotoxy(80,5);
	printf("\033[38;2;255;105;180m$$$$$");
	gotoxy(81,6);
	printf("\033[38;2;255;105;180m$$$");

//coraÃ§Ã£o 3
    gotoxy(78,14);
	printf("\033[38;2;255;105;180m$$$$  $$$");
	gotoxy(77,15);
	printf("\033[38;2;255;105;180m$$$$$$$$$$$");
	gotoxy(78,16);
	printf("\033[38;2;255;105;180m$$$$$$$$$");
	gotoxy(80,17);
	printf("\033[38;2;255;105;180m$$$$$");
	gotoxy(81,18);
	printf("\033[38;2;255;105;180m$$$");
    printf("\033[1;37m");

    gotoxy(1, 21);
    printf("\033[0;30m");  // cor preta para disfarÃ§ar o termino do programa
    //exit (strcat_s);  //encerra o programa, Ã© uma funÃ§Ã£o da biblioteca stdlib.h
}

main(){

	int opcao_menu;
	int opcao_nivel;
    int opcao=-1;
    int opcao2=0;
    int coluna, linha=0;

	//criando tela 1
	telaApresentacao();

	while(opcao != 0){
		telaMenu();
		scanf("%i", &opcao_menu);
        system("CLS");
		//tela 3
		if(opcao_menu == 1){//coluna=87 linha=21
			telaCadastrarJogadores();
            system("CLS");
            telaVisualizarNiveis();
        }
		if(opcao_menu == 2){
            telaVisualizarNiveis();
            scanf("%i", &opcao_nivel);
            system("CLS");
				if(opcao_nivel == 1){
					telaSegundoNivel();
					getch();
				}
				if(opcao_nivel == 2){
                    printf("\033[1;31mOpcao ainda nao valida, tente novamente!\033[1;37m");
					getch();
				}
				if(opcao_nivel == 3){
                    telaMenu();
                    getch();
				}
			}
		if(opcao_menu == 3){
			telaAjuda();
			getch();
		}
		else if(opcao_menu == 4){
			telaAgradecimento();
			getch();
            break;
		}
	}//while
}//main
