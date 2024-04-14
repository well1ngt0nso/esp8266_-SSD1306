# 💻⚡ esp8266_SSD1306 ⚡💻
Repositório destinado a utilização de Esp8266 com display oled SDD1306 já presente na placa, podendo ser facilmente expandido para utilização com o mesmo display externamente ou em alguma variação das placas Arduino e demais ESP's com display na placa ou externo, como veremos aseguir 

* OBJETIVOS: Fundamentos sobre Esp8266, Fudementos de display OLED SSD1306, Compreendendo a placa com display integrado e Utilização e exemplos
* MATERIAL: Esp8266 com display OLED ssd130 integrado (vale para utilização em outras configurações que utilizem display sdd1306), Cabo USB tipo C (isso depende do seu)

### ESSA É A PLACA QUE ESTOU USANDO (ESP8266 OLED SDD1306):
<p align="center">
  <img src="https://github.com/well1ngt0nso/esp8266_SSD1306/assets/58373332/68dac883-39be-4e6b-b7c4-1dd20c64e0fa" width="50%" />
</p>

Escolhi adquirir essa placa porque ela é bem compacta e já possui a integração com o módulo sdd1306, porém decidi escrever esse diretório porque não encontrei quase nehuma documentação sobre uma placa com essa arquitetura, na verdade apenas exemplos separados, de início achei que ia ser bem complicado devido a também não ter encontrado documentação na página do vendedor, vamos lá1

_**⚠️OBS:**_
Caso a sua vesão do microcoontolador seja com módulo integrado, não faça o uoloud de nenhum sketch para o seu Esp8266 antes de anotar ou salvar algumas informações importantes. Mas não se preocupe caso já tenha feito o upload de algo, trataremos nos próximos tópicos

## PARTE  1 - ESP8266 
Então, pessoal, esses conceitos são bem inicias, não é nenhuma aula de programação sobre esp8266, então caso você não queira ou já conheça, basta pular para o próximo tópico [ PARTE 2 - DISPLAY LCD OLED SDD1306](https://github.com/well1ngt0nso/esp8266_SSD1306/tree/main?tab=readme-ov-file#parte-2---display-lcd-oled-sdd1306)

O esp8266 assim como as demais placas da família esp são bem robustas, são bem completas quano comparadas a maioria das variabilidades de microcontroladores existentes no mercado. Sua versatilidade demanda não especificamente de atividades que são restritas ao esp, mas o fato de já vir com integração a circuitos que em outras placas seria necesário um módulo externo. Temho isso como muito bom, claro, dependendo da aplicação. Exemplo: O esp8266 em questão vem com display soldado na placa principal, caso o seu projeto precissase de um display distante não seria "possível", não com a mesma configuração, poderia ser utilizado outro display ou desoldar o existente. Assim... nesses caso acho que você não optaria por um já soldado, o mesmo vale para os demais circuitos que já vem integrado: módudulo wifi, módulo bluethoth...

Ou seja, caso o projeto não necessite de uma manipulação física entre o esp e os circuitos já integrados a placa, vale muito apena! Ainda acrescento, não somente apenas a isso, mas também em relação ao processamento(voltamos já a isso), deixando o texto de lado, vamor ver algo que acho muito interessante: miniaturização
<p align="center">
  <img src="https://github.com/well1ngt0nso/esp8266_SSD1306/assets/58373332/8e96141d-239c-4b54-a67a-3a48f38293ca" width="50%" />
</p>
Essa placa é muito compacta pelo que entrega, se encaixa em quase tudo, falo espcíficamente a essa versão, pois já encontrei outra bem menor (esp32 c3), nese caso agora ela deve se encaixar em tudo, chegou para disputar com os menores Arduinos existentes no mercado. Contudo, como nem tudo são flores, quando maior a miniaturização, menor a capacidade de suporte a saídas e entradas, vejamos uma comparação entre o esp8266 utilizado nesse repositório e o Arduino MEGA:


<p align="center">
  <img src="https://github.com/well1ngt0nso/esp8266_SSD1306/assets/58373332/fe41cf13-182c-45f3-b008-688d8740324e" width="50%" />
 <div align =  "center"><i>Diagrama de distribuição das GPIO's (pinos) no NodeMCU Esp8266</i></div>
</p>

<br/>
<br/>
<br/>



<p align="center">
  <img src="https://github.com/well1ngt0nso/esp8266_SSD1306/assets/58373332/92dfb519-06cd-4e0d-a64d-dff1f62305b3" />
  <div align =  "center"><i>Diagrama de distribuição das GPIO's (pinos) no Arduino Mega</i></div>
</p>


Agora vamos ver uma tabela visual entre o Esp8266 e o Arduino UNO: 

## PARTE 2 - DISPLAY LCD OLED SDD1306: 
O mesmo vale para esse tópico, são apenas conceitos introdutórios, o entendimento em si e programação começam nos tópicos seguintes: 
