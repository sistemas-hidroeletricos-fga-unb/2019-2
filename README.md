# Aproveitamento Hidrelétrico

## UHE Serra da Mesa

![](https://i.imgur.com/LoajmQf.jpg)
Figura 1: UHE Serra da Mesa (Fonte: Elaboração própria)

A UHE Serra da Mesa fica localizada no Rio Tocantins, próxima ao município de Minaçu-GO. A usina possui 1.275 MW de capacidade instalada divididos em 3 máquinas.
O reservatório é considerado, em volume de água, o maior do país, com capacidade de armazenamento de 54.408 hm³. Seu volume mínimo para operação é de 11.150 hm³. A área alagada é de 1.784 km². E sua altura  mínima de queda é de 83,3 m. 
Esta UHE foi escolhida para que se faça uma avaliação acerca do projeto e averiguar as razões pelas quais o reservatório desta usina manteve-se, nos últimos anos, abaixo da metade de sua capacidade máxima.

UHE | Serra da Mesa
-----|---------------
Proprietário | Furnas Centrais Elétricas S.A
Municípios | Colinas do Sul-TO e Minaçu-GO
Rio | Tocantins
Potência (MW) | 1.275
Área inundada máxima (m²) | 1.784
Volume máximo (hm³) | 54.400

Tabela 1: Dados da UHE Serra da Mesa disponíveis no shapefile disponível no Sigel/ANEEL

## Elaboração de Mapas
Para a elaboração dos mapas foi utilizada a ferramente QGIS 3.8.2 e a base de dados OpenStreetMap;

No software QGIS foi carregado o mapa OpenStreetMap, em seguida foi identificada a área pertinente a Usina Hidrelétrica Serra da Mesa; para a construção do mapa foi utilizada a ferramenta de impressão, nela foram definidos os parâmetros da imagem, bem como adicionada a escala e orientação do mapa.

Para aferição da área da usina foi verificado na tabela de atributos pertencente ao arquivo shapefile, fornecida no Sigel, portal ArcGis da ANEEL, nela estão disponíveis dados da usina que foram detalhados na ÁREA DE CAPTAÇÃO DA USINA HIDRELÉTRICA SERRA DA MESA.

## Cálculos de Aproveitamento Hidrelétrico

### ENERGIA HIDRELÉTRICA MÉDIA DISPONÍVEL
![](https://i.imgur.com/gPjiE7S.png)

### SALTO ENERGÉTICO/TRABALHO ESPECÍFICO
![](https://i.imgur.com/ooOwgM9.png)

### QUEDA DE APROVEITAMENTO

Altura líquida: 0,8.83,3 (20\% de perda) = 66,64 m

Para determinar se é de baixa ou alta queda:


Classificação | Faixa de Altura 
--------------|-----------------
Baixa Queda   | até 50 m
Média Queda   | 50 a 250 m
Alta Queda    | acima de 250 m

Tabela 2: Classificação da queda da usina de acordo com as faixas de altura


Logo a UHE Serra da Mesa é considerada de média queda, considerando perdas de 20\%.

### CÁLCULO DE VAZÃO MÉDIA DE LONGO TERMO

Para definir a vazão média de longo termo, o grupo baseou-se em dados obtidos no sistema hidroweb da Agência Nacional de Águas - ANA, e em boletins do Operador Nacional do Sistema Elétrico. Para tanto, foram usadas estações de medição à montante do reservatório da UHE. Para os dados diários entre 2014 e 2019, a base consultada foi o Boletim Diário da Operação (BDO) do ONS. Deste boletim, foi utilizada a vazão afluente da UHE.
A vazão média foi calculada utilizando a ferramenta de calcular média do excel, foram considerados 2.265 dados diários de vazão, fornecendo o resultado de 487,861 m³/s.

### ÁREA DE CAPTAÇÃO DA USINA HIDRELÉTRICA SERRA DA MESA

![](https://i.imgur.com/fxPYfrM.jpg)
Figura 2: Área de captação da UHE Serra da Mesa

A área inundada da UHE Serra da Mesa é de 1.784 m² disponível na tabela de atributos da shapefile.

### ESCOLHA DO TIPO DE CENTRAL E DO ARRANJO UTILIZADO

Em virtude de ser um projeto existente, serão mantidos o tipo de central e o arranjo utilizado. Será considerada uma central de represamento que, conforme notas de aula, cria uma barragem no rio e a ligação entre a barragem e a casa de máquinas é feita através de um conduto forçado. 

Todos contribuíram para esta entrega.

### ESTIMATIVA DA POTÊNCIA INSTALADA

A potência instalada é potência que a usina tem a obrigação de fornecer, de acordo com os dados do SIGEL/Aneel a potência instalada da Usina Serra da Mesa é de 1.275 MW. Realizamos o cálculo da potência instalada, supondo os rendimentos, afim de verificar se a potência cálculada é próxima aquela que SIGEL fornece. 

Considerando o redimento da turbina 0.9, o redimento do gerador 0.98 e a vazão sendo a maior vazão histórica, que foi de 3.603 m³/s a potência instalada da usina seria de 2.077,47 MW.
![](C:\Users\Amanda\Documents\Capturar.PNG)

Já considerando a vazão média, que é de 487,861 m³/s a potência instalada da usina é de 281,2 MW. 







