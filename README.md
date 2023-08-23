# TF1800-Alarm Manager
 Alarm Manager to TF1800 TC3 PLC-HMI

Para adicionar os alarmes ao seu projeto copiar os seguintes itens:

1)	Copiar as estruturas da pasta DUT
2)	Pasta FB: Copiar as bibliotecas: FB_GerenciadorAlarmes e FB_DataHora
3)	Pasta GVL: Copiar a GVL_Alarmes
4)	Pasta POUS: Copiar o programa PrgAlarmes. Depois realizar a chamada deste programa no MAIN.
5)	Pasta VISU: Copiar as telas:
  a.	Tela_Alarmes
  b.	Tela_Historico
  c.	Lista_Imagens
  d.	Lista de Mensagens: Neste local que você irá escrever todas as mensagens de alarmes e eventos. 
    i.	Mensagem 0 – não usar
    ii.	Mensagens 1 a 100 – são os alertas e aparecem na cor amarelo na lista de alarmes
    iii.	Mensagem de 101 a 200 – alarmes e aparecem na cor vermelha na lista de alarmes

6)	Copiar a pasta Images para dentro da pasta do projeto.
7)	Adicionar a biblioteca Tc2_Utilities. Para isso clicar com o botão direito do mouse sobre References e selecionar a opção: Add Library. Depois ir em System -> IPC-Series -> Tc2_Utilities.
8) Para acionamento dos alarmes você deve usar a ACT_ALARMS e ACT_WARNINGS. Toda vez que ativar um Alarmes [xx], sua respectiva mensagem irá aparecer. Se não houver mensagem configurada ele retorna o número do array.
Se preferir pode alterar a linguagem.

 
