# Projeto Hidroelétrico UHE Serra da Mesa

## Aproveitamento Hidrelétrico

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

### Elaboração de Mapas
Para a elaboração dos mapas foi utilizada a ferramente QGIS 3.8.2 e a base de dados OpenStreetMap;

No software QGIS foi carregado o mapa OpenStreetMap, em seguida foi identificada a área pertinente a Usina Hidrelétrica Serra da Mesa; para a construção do mapa foi utilizada a ferramenta de impressão, nela foram definidos os parâmetros da imagem, bem como adicionada a escala e orientação do mapa.

Para aferição da área da usina foi verificado na tabela de atributos pertencente ao arquivo shapefile, fornecida no Sigel, portal ArcGis da ANEEL, nela estão disponíveis dados da usina que foram detalhados na ÁREA DE CAPTAÇÃO DA USINA HIDRELÉTRICA SERRA DA MESA.

### Cálculos de Aproveitamento Hidrelétrico

#### ENERGIA HIDRELÉTRICA MÉDIA DISPONÍVEL
![](https://i.imgur.com/gPjiE7S.png)

#### SALTO ENERGÉTICO/TRABALHO ESPECÍFICO
![](https://i.imgur.com/ooOwgM9.png)

#### QUEDA DE APROVEITAMENTO

Altura líquida: 0,8.83,3 (20\% de perda) = 66,64 m

Para determinar se é de baixa ou alta queda:


Classificação | Faixa de Altura 
--------------|-----------------
Baixa Queda   | até 50 m
Média Queda   | 50 a 250 m
Alta Queda    | acima de 250 m

Tabela 2: Classificação da queda da usina de acordo com as faixas de altura


Logo a UHE Serra da Mesa é considerada de média queda, considerando perdas de 20\%.

#### CÁLCULO DE VAZÃO MÉDIA DE LONGO TERMO

Para definir a vazão média de longo termo, o grupo baseou-se em dados obtidos no sistema hidroweb da Agência Nacional de Águas - ANA, e em boletins do Operador Nacional do Sistema Elétrico. Para tanto, foram usadas estações de medição à montante do reservatório da UHE. Para os dados diários entre 2014 e 2019, a base consultada foi o Boletim Diário da Operação (BDO) do ONS. Deste boletim, foi utilizada a vazão afluente da UHE.
A vazão média foi calculada utilizando a ferramenta de calcular média do excel, foram considerados 2.265 dados diários de vazão, fornecendo o resultado de 487,861 m³/s.

#### ÁREA DE CAPTAÇÃO DA USINA HIDRELÉTRICA SERRA DA MESA

![](https://i.imgur.com/fxPYfrM.jpg)
Figura 2: Área de captação da UHE Serra da Mesa

A área inundada da UHE Serra da Mesa é de 1.784 m² disponível na tabela de atributos da shapefile.

#### ESCOLHA DO TIPO DE CENTRAL E DO ARRANJO UTILIZADO

Em virtude de ser um projeto existente, serão mantidos o tipo de central e o arranjo utilizado. Será considerada uma central de represamento que, conforme notas de aula, cria uma barragem no rio e a ligação entre a barragem e a casa de máquinas é feita através de um conduto forçado. 

Todos contribuíram para esta entrega.

#### ESTIMATIVA DA POTÊNCIA INSTALADA

Define-se potência instalada como a potência registrada nas placas de identificação do gerador, de acordo com os dados do SIGEL/Aneel a potência instalada da Usina Serra da Mesa é de 1.275 MW. Realizamos o cálculo da potência instalada, supondo os rendimentos, afim de verificar se a potência cálculada é próxima aquela que SIGEL fornece. 

![](https://i.imgur.com/knlPXJB.png)

![](https://i.imgur.com/B6NjcXF.png)

Considerando o redimento da turbina 0.9, o redimento do gerador 0.98 e a vazão sendo a maior vazão histórica, que foi de 4.359 m³/s a potência instalada da usina seria de 2.511,66 MW.

![](https://i.imgur.com/WjO2pgi.png)

Já considerando a vazão média, que é de 487,861 m³/s a potência instalada da usina é de 281,2 MW. 

## PROJETO HIDROLÓGICO



### DIAGRAMA DE MASSAS DE RIPPL
Com o uso do diagrama de massas é possível prever a confiabilidade de um reservatório hídrico a partir do volume máximo acumulado em um reservatório obtido a partir da série histórica de vazões, podendo-se estimar o volume de água no reservatório para o ano seguinte.

Se traçarmos retas tangentes aos pontos de máximo e mínimo da curva de massas, podemos obter o nível de segurança de um reservatório apresentado pela diferença entre a tangente do ponto de mínimo para a do ponto de máximo.

A partir da curva obtida é possível concluir que o reservatório da UHE Serra da Mesa é muito confiável, uma vez que seus pontos de mínimos e máximo são muito próximos, principalmente levando em consideração a ordem de grandeza dos dados (bilhões de litros).

![](https://i.imgur.com/PtUnivc.png)
Figura 3: Diagrama de Rippl da Usina Serra da Mesa entre os anos de 2014 a 2018

 Para elaboração desta curva foi utilizada a série diária de vazões, portanto, foi multiplicada pelo tempo em segundos de um dia (24x3600).

### FLUVIOGRAMA
Utilizando os dados de vazão média diária entre fevereiro de 2014 e setembro de 2019, foi possível traçar o gráfico que mostra o comportamento das vazões do rio.

![](https://i.imgur.com/6BPCnKq.png)
Figura 4: Fluviograma da Usina Serra da Mesa entre os anos de 2014 a 2018

### CURVA DE DURAÇÃO DE VAZÕES
Para elaborar o gráfico da curva de duração foram seguidas as instruções das notas de aula, utilizando as vazões médias mensais e verificando quantas vezes determinada vazão foi equalizada ou superada e, logo após, dividindo esse número pelo total de vazões no histórico.


![](https://i.imgur.com/w0l2TpJ.png)
Figura 5: Curva de duração da Usina Serra da Mesa entre os anos de 2014 a 2018

### CURVA DE DURAÇÃO DE POTÊNCIAS
Como descrito nas notas de aula, para se obter a curva de duração de potências multiplicaram-se os valores do eixo das ordenadas da curva acima pela queda de aproveitamento definida anteriormente (66,64 metros), pela aceleração da gravidade (9,98m/s²) e pelo rendimento considerado de 90%. 

![](https://i.imgur.com/Jtdh9s7.png)

Figura 6: Curva de duração de potência da Usina Serra da Mesa entre os anos de 2018 a 2019

### PERÍODO CRÍTICO
O período crítico de um reservatório compreende os meses que estão entre os níveis máximo e mínimo do ano civil, não incluindo o mês de nível máximo ou de mínimo. O período crítico da UHE Serra da Mesa são os meses de março a agosto, como pode ser visto no gráfico abaixo, não foram considerados os anos de 2014 e 2019 pelos dados do ano civil estarem incompletos.

![](https://i.imgur.com/LkUzVbr.png)

Figura 7: Período crítico da UHE Serra da Mesa

### PERÍODO SECO E PERÍODO ÚMIDO
O período seco é dado pelos meses do ano hidrológico correspondentes ao período crítico e o período úmido são os meses restantes. O ano hidrológico o estado de Goiás, onde fica localizada a UHE Serra da Mesa, inicia-se em outubro de um ano e termina em setembro do ano seguinte. O período seco no estado de Goiás inicia em abril perdurando até a primeira quinzena de outubro, enquanto o período seco compreende a segunda quinzena de outubro até março do ano seguinte. No gráfico abaixo pode-se observar os períodos seco e úmido do reservatório da UHE Serra da Mesa, sendo que o mês de outubro foi incluído integralmente no período úmido para facilitar a visualização.

![](https://i.imgur.com/irgwYAL.png)

Figura 8: Períodos seco e úmido no ano hidrológico da UHE Serra da Mesa

Não há sobreposição completa entre os períodos úmido e seco com o período crítico pois não há correspondência perfeita entre os índices de precipitação, que definem o ano hidrológico, com a vazão do rio. Considerando que o rio Tocantins abrange vários estados, esta pode ser uma das razões por não ocorrer da forma ideal.

![](https://i.imgur.com/pnA6bXv.png)

Figura 9: Sobreposição do período crítico para as estações seca e úmida no ano hidrológico

### VALORES EXTREMOS
Os valores extremos de vazões são analisados de forma semelhante, sendo os dados totais de onde serão extraídos que diferenciam o cálculo dos mesmos. Para definição das vazãos máximas utilizam-se dados de ano hidrológico enquanto para vazões mínimas recorre-se a dados do ano civil. No gráfico abaixo é possível observar os valores máximos e mínimos para cada ano hidrológico.

![](https://i.imgur.com/S9GuVq6.png)

Figura 10: Valores de máximo e mínimo para cada ano hidrológico

Enquanto o mês de setembro sempre foi correspondente ao valor de mínimo de todos os anos hidrológicos, os valores de máximo variam entre os meses de fevereiro, março e abril, justificando ainda a dificuldade na determinação do período crítico e sua correspondência exata ao período seco.

### ESTIMATIVA DA VAZÃO DE PROJETO 

De acordo com a Aneel a energia firme de uma usina hidrelétrica corresponde à máxima produção contínua de energia que pode ser obtida, supondo a ocorrência da seqüência mais seca registrada no histórico de vazões do rio onde ela está instalada. Como os dados diários de vazões do ano de 2014 até 2019 da Usina Serra da Mesa variam muito, estimou-se que a vazão firme é de 100 m³/s, pois é uma faixa de vazão baixa e que ocorre considerávelmente.

Como visto anteriormente a vazão média é 427,861 m³/s então essa será considerada nossa vazão necessária, aplicando então a seguinte metodologia:

![](https://i.imgur.com/5a2VhTz.png)

Com isso, a vazão do projeto deve ser menor ou igual a vazão média de longo tempo, que de acordo com a curva de vazões é de 400,17 m³/s.

### REGIONALIZAÇÃO DE VAZÃO

Para o cálculo da vazão regionalizada utilizou-se o método de Conti-Varlet de acordo com o livro texto utilizado no curso. Abaixo é apresentada a adaptação do gráfico da curva de Rippl para a utilização do método mencionado.

![](https://imgur.com/A91vXKj.png)

A partir da linha segmentada em azul foram feitos os cálculos das vazões regionalizadas parciais utilizando a seguinte fórmula:

![](https://imgur.com/jSDsxu4.png)

Onde Qr é a vazão regionalizada. 
Assim, tem-se que a vazão regionalizada total é:

![](https://imgur.com/NPNZXc3.png)

Visto que as vazões da Usina Serra da Mesa variam excessivamente durante os anos, com isso torna necessária então a construção de um reservatório para que se possa reter o excesso d'água dos períodos de grandes vazões para ser utilizado nas épocas de seca. A vazão firme da usina é de 100 m³/s, contudo de acordo com os dados diários, o menor valor chegou a 2 m³/s. 

A vazão de projeto é de 400,17 m³/s, 4 vezes maior que a vazão firme, visto isso, há necessidade de regularização de vazão em períodos de seca. O método utilizado é possível verificar as vazões que serão regularizadas bem como o tempo de duração e verificou-se que o total de vazão regularizada é alto comparado com a vazão de projeto.

##PROJETO DO CONDUTO
### FORMA GEOMÉTRICA DE SEÇÃO PARA O CANAL EM QUESTÃO, DIÂMETRO HIDRÁULICO DA SEÇÃO, VELOCIDADE DA ÁGUA NO CANAL, VAZÃO DE ÁGUA NO CANAL

A forma geométrica do canal é semi circular, como na figura abaixo.

![](https://imgur.com/BKguSph.png)
Figura 11: área de seção do canal

O diâmetro hidráulico é dado pela relação entre a área molhada e o perímetro molhado, como mostrado abaixo:

![](https://imgur.com/GQNiCyn.png)

Considerando a profundidade do canal “h” igual a 1,5 metros temos que o diâmetro hidráulico é 3 metros. 
Se tratando da velocidade da água no canal utilizou-se a fórmula de Chezy abaixo, a dedução se encontra nas notas de aula do curso.

![](https://imgur.com/4IGCH4G.png)

Assim, a vazão no canal é igual a

![](https://imgur.com/i0mh4Ay.png)

### DETERMINAÇÃO DE LINHAS PIEZOMÉTRICA E DE ENERGIA EM DESENHO ESQUEMÁTICO DO SISTEMA HIDROMECÂNICO EQUIVALENTE

### DETERMINAÇÃO DO SEMIPERÍODO DA ONDA DE PRESSÃO PARA DIMENSIONAMENTO DO CONDUTO FECHADO.

### DETERMINAÇÃO DE VALORES DE GOLPE DE ARÍETE POSITIVO MÁXIMO E ACEITÁVEL.


## PROJETO DA TURBINA

### CONDIÇÕES DE OPERAÇÃO DA TURBINA E ESPECIFICAÇÃO DA POTÊNCIA MECÂNICA DA TURBINA

Foram feitas medições de vazão e altura de queda na bancada hidrelétrica do laboratório de termofluidos.
Para cálculo da vazão referente ao vertedouro analisado foi utilizada sua fórmula empírica, mostrada abaixo:

![](https://imgur.com/GKMAktf.png)

Sendo 'h' a variação de altura da margem superior da coluna d'água formada, até o ponto mais baixo da saida do vertedouro em metros (0,12m). Assim, a vazão no vertedouro é:

![](https://imgur.com/eQUYzyl.png)

Tendo uma queda de 2 MCA foi calculada a potência da bancada da seguinte forma:

![](https://imgur.com/wdPBh1S.png)

Posteriormente reduziu-se a vazão sendo 'h' proporcionalmente diminuido para 11,5cm e repetiu-se os passos anteriores

![](https://imgur.com/Xn9RZ9J.png)
![](https://imgur.com/utwA2Y1.png)

Adiante, foi examinado o comportamento da central quando conectada à lâmpadas incandescentes e assim variou-se a rotação da máquina. Notou-se que a potência de iluminação das mesmas varia de acordo com a variação da rotação.

Calculou-se a potência mecânica da turbina novamente, para valores de “h” igual a 14cm e queda (“H”) de 1,75mca. Utilizando a formulação descrita acima, a vazão e a potência do novo experimento são iguais a 0,01026 m³/s e 176,3 W respectivamente.

Foi feito também o cálculo  da potência elétrica do sistema, utilizando os mesmos dados de vazão e altura:

![](https://imgur.com/34RKruf.png)

Onde, U= tensão (110V) e R= resistência da lâmpada (269 ohm). Sendo assim,

![](https://imgur.com/tMjJXwg.png)

Pode-se notar que a potência elétrica é muito menor que a potência mecânica, isso se dá devido às perdas de rendimento ao longo do processo. De acordo com Stephen J. Chapman, "as perdas elétricas se dão por aquecimento resistivo que ocorre nos enrolamentos do estator (armadura) e do rotor (campo) da máquina. As perdas mecânicas em uma máquina são as perdas associadas aos efeitos mecânicos. Há dois tipos básicos de perdas mecânicas: atrito e ventilação. Perdas por atrito são causadas pelo atrito dos rolamentos da máquina, ao passo que as perdas por ventilação são causadas pelo atrito entre as partes móveis da máquina e o ar contido dentro do motor. Essas perdas variam com o cubo da velocidade de rotação da máquina."

### LEVANTAMENTO DA POTÊNCIA TRANSMITIDA PARA O CENTRO DE CARGA

A potência elétrica do sistema foi determinada a partir da fórmula acima descrita, envolvendo a relação de tensão e resistência da lâmpada. Assim, foram feitos vários testes variando a tensão, que podem ser visualizadas abaixo:

![](https://imgur.com/0F6khDL.png)

### ESTIMATIVA DO FATOR DE CAPACIDADE DA TURBINA
Foi analisado o fator de capacidade (FC) da usina relacionada à bancada hidrelétrica do laboratório de termofluidos de acordo com a formulação abaixo. Para tal iniciou-se as aferições com uma tensão de 220 Volts com as três lâmpadas, tendo assim a carga máxima disponível conectada ao sistema.

![](https://imgur.com/o1A0v0c.png)

![](https://imgur.com/bTw36N0.png)

![](https://imgur.com/SI600ag.png)

Onde, a potência instalada (Poti) é constante para a usina e a potência gerada (Potg) varia de acordo com a variação de tensão e “R” é a resistência da lâmpada. 

Para carga máxima (3 lâmpadas):

![](https://imgur.com/oG5JKpx.png)

![](https://imgur.com/qPsK7Uf.png)

Após, foram retiradas lâmpadas de forma a diminuir a carga, assim o fluxo de energia também deve ser controlado pois acontece um aumento de potência devido à elevação da tensão. Pôde-se perceber, de acordo com os resultados mostrados abaixo, o aumento do fator de capacidade:

Para 2 lâmpadas:

![](https://imgur.com/fDQfPYw.png)

![](https://imgur.com/Y0rGyF1.png)

Para 1 lâmpada: 

![](https://imgur.com/wUvskEk.png)

![](https://imgur.com/Ti4qCf2.png)

Foram feitas novas medições com tensão igual a 180V, 200V e 310V, para fins de comparação.

Para 1 lâmpada com tensão igual a 180V:

![](https://imgur.com/dSAADdt.png)

![](https://imgur.com/cLmaih9.png)

Para 2 lâmpadas com tensão em 220V:

![](https://imgur.com/T03v7aW.png)

![](https://imgur.com/YcVc2o6.png)

Para 1 lâmpada com tensão em 310V:

![](https://imgur.com/PE6Zmqk.png)

![](https://imgur.com/RYw4MNM.png)

O fator de capacidade acima de 100% simboliza que a carga está muito baixa e o controle do fluxo de energia se faz necessário, sendo assim a potência instalada não está sendo plenamente utilizada. 
Dessa forma conclui-se que o fator de capacidade não é um bom indicador para a geração de energia.
