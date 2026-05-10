# Dataset de Consoles Portáteis Retrô (3DS vs PSP)

## Visão Geral
Este mini dataset foi construído como parte da avaliação da disciplina de **Visão Computacional** da Residência em TIC43 (Professor Alyson Bezerra). O objetivo é aplicar os fundamentos de processamento de imagens (resolução, espaços de cor, quantização e formatos) em um cenário real de classificação.

## Classes
O dataset contém 10 imagens originais, divididas em duas classes mutuamente exclusivas que representam paradigmas distintos de design de hardware:
* **Classe A (`classe_A_3DS`):** Nintendo 3DS (Design clamshell ou clip, cor sólida com alto brilho, duas telas).
* **Classe B (`classe_B_PSP`):** Sony PSP (Design em barra, cor sólida e fosca preta, uma tela central).

## Metodologia de Aquisição
Todas as imagens foram capturadas de forma padronizada para facilitar a segmentação por algoritmos de visão computacional:
* **Fundo:** Utilizado papel sulfite branco para criar um fundo infinito de alto contraste.
* **Variação de Iluminação:** O dataset conta com três cenários principais de luz:
  1. Iluminação artificial ligada (luz do ambiente).
  2. Iluminação apagada com janelas fechadas (baixa luminosidade, forçando o aumento do ISO do sensor e a introdução de ruído).
  2. Iluminação natural com janelas abertas (média luminosidade, introduzindo sombras e contraste de sombras no ambiente).
* **Variação de Ângulo:** Capturas incluem visão frontal, perfil, isométrica e detalhes de hardware.
* **Filtros:** Nenhum filtro ou IA de embelezamento foi utilizado durante a captura.

## Estrutura de Metadados
O arquivo `metadata.csv` mapeia cada arquivo (`imgXXX_original.jpg`) às suas respectivas condições de captura (iluminação, ângulo e dispositivo), permitindo análises estratificadas do desempenho de futuros modelos.