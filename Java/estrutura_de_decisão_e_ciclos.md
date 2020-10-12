#### **Estruturas de seleção**

Em Portugol, trabalhamos com três tipos de repetição: Simples, Composta e Múltipla Escolha.
Em Java, o formato é muito semelhante ao que vimos em Portugol, mudando só o fato das decisões dependerem de Expressões Condicionais.

**Seleção Simples:** Estrutura de comparação simples, sendo executado o valor somente com os testes retornando valores verdadeiros (true).

Portugol                                                               Java

se(condição){comandos}                  if(condição){comandos}



**Exemplo:**

numero = 42;
divisor = 1;

while (divisor <= numero) {
resto = numero % divisor;
if (resto == 0) {
printf("Divisor encontrado: %d \n", divisor);
}
divisor = divisor + 1;



**Seleção Composta:** Usada para comparação,podendo retornar valores diferentes,sendo eles verdadeiros(true) ou falsos(false).
      Portugol                                                                    Java
se(condição){                                                          if(condição){
comandos comandos
     }senao{                                                                   }else{
    comandos                                                               comandos
         }                                                                                   }

**Exemplo:**

#include <iostream.h>
void main( )

{
int x;
cin >> x;
cout << "o número é " << x << "\n";
If (x%2==0)
{
cout << "O valor é PAR\n";
}
else
{
cout << "O valor é IMPAR\n";
}
}
}

**Seleção Múltipla Escolha:** Esta é uma estrutura de decisão do tipo CASO, de forma que uma ou mais condições possam ser testadas. Assim, cada decisão pode ser associada a um comando diferente.
                  Portugol                                                                         Java
            escolha(variável){                                                    switch(variável){
               caso valor1:                                                               case valor1:
                comandos                                                                  comandos
                      pare                                                                            break;
               caso valor2:                                                                 case valor2:
                comandos                                                                   comandos
                   pare                                                                             break;
             casocontrario                                                                  default;
                comando                                                                    comandos
                         }                                                                                  }



**Exemplo:**

case valor1:

comandos;
break;
case valor2:
comandos;
break;

comandos;
}

####                                        **Estruturas de Repetição**

Estas estruturas permitem repetir diversas vezes um mesmo trecho do programa. De maneira análoga às estruturas de decisão, as estruturas de repetição dependem do teste de uma condição.
**São três os tipos de estruturas de repetição:**
*Teste no inicio;*
*Teste no final;*
*Com variável de controle;*
Vocês vão ver que quase não há diferença na linguagem do Portugol para o Java.

**Tipo de teste**                                         Portugol                                                                      Java
**C/ TESTE INICIO**                                 ENQUANTO(CONDIÇÃO){                                       WHILE(CONDIÇÃO){
                                                                  COMANDOS;}                                                             COMANDOS;}
**C/ TESTE FINAL**                                        FACA{COMANDOS;                                                 DO{COMANDOS;
                                                            }ENQUANTO(CONDIÇÃO)                                         }WHILE(CONDIÇÃO)
**C/ VARIAVEL DE CONTROLE**          PARA(VALOR INICIAL; VALOR                           FOR(VALOR INICIAL;VALOR
                                                                      FINAL;INCREMENTO/                                      FINAL;INCREMENTO/
                                                                 DECREMENTO){COMANDOS;}                     DECREMENTO){COMANDOS;}



**Exemplo:**

int main(){
int i, n;
float s=0, x;

printf (“n=”);
scanf (“%d”,&n);
for (i=1; i <= n; i++){
printf (“X= ”);
scanf (“%f”,&x);
s = s + x;
}
printf (“média=%.2f”,s/n);
return 0;
}



Autora: Karolyna Gomes