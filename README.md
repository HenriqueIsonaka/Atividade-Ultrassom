Construção do carrinho: atividade 5
===================================
Este trabalho foi feito em dupla por Gean Santos e Henrique Isonaka

*OBS: ignorar commits que não começam com "Commit atividade 5" e ignorar primeiro commit 5(1)

Teste introdutório: testar código do input capture (presente nos tutoriais do notion)

Evidência do teste:

<img width="426" height="240" alt="Gif input capture" src="https://github.com/user-attachments/assets/7a97c103-b359-49c9-93dd-4198856d24ce" />


Commit 1


Objetivo: utilizar o ultrassom para identificar a distância entre ele e um obstáculo à sua frente e definir se ele está a mais de 20 cm de distância ou não

Resultado: O sensor consegue detectar a distância entre ele e o obstáculo e definir se ele está ou não a mais de 20 cm de distância, imprimindo essas informações constantemente no monitor serial por meio da placa freedom. É importante ressaltar que o ultrassom não consegue definir a distância entre ele e um obstáculo diretamente: é necessária uma função para converter o intervalo de tempo entre o início e o fim do pulso de echo.

<img width="234" height="150" alt="589920266-428acc03-ce4e-4f18-bba5-c763aa42c3aa" src="https://github.com/user-attachments/assets/84b5d03f-89ed-4d44-95ac-cfc85a861d0d" />


Commit 2

O sensor ultrassônico foi instalado no carrinho por meio de um suporte de papelão e cola quente, ficando na sua parte frontal. O código do ultrassom foi convertido em um arquivo de biblioteca para ser implementado no código do carrinho de forma mais simples e consistente.

Objetivo: fazer com que o carrinho parasse de andar ao detectar um obstáculo a 20 cm de distância.

Resultado: Carrinho parava de executar a função de andar para frente ao detectar um obstáculo a 20 cm ou menos de distância.

<img width="426" height="240" alt="Gif carrinho parando" src="https://github.com/user-attachments/assets/5881e620-a7ba-488a-826b-fb454d27b5ec" />



Commit 3

Para a competição, seria necessário fazer o carrinho parar completamente o mais próximo possível dos 20 cm de distância de um obstáculo

Dessa forma, a partir de vários testes feitos com a superfície da lousa branca, na qual ele seria testado, foi estimada a distância que o carrinho percorreria após receber o comando de parar de andar por conta da inércia do seu movimento. Essa distância, baseando-se no carrinho com velocidade máxima, foi de 26.5 cm, sendo que dessa forma, conclui-se que o carrinho anda 6.5 cm após parar com o comando de andar para frente.

Resultado: O carrinho, quando em velocidade máxima, parava muito próximo dos 20 cm nos testes, no entanto, essa distância aumentava a medida que a velocidade em que o carrinho estava ao identificar um obstáculo diminuia.
