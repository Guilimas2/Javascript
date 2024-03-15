# Análise de código javascript
Este projeto consiste em, utilizando dois códigos disponíveis [aqui](https://terminalroot.com.br/2016/12/alguns-codigos-simples-de-javascript-2.html), analisá-los, implementá-los e testa-los. Após os testes, foi preciso identificar o que cada parte do javascript está fazendo e documentar tudo. Toda a documentação está disponível abaixo.


## Atrasando no tempo 
![telainicial](print.jpeg)
* analise do código 💻 [tempo.html](/tempo.html)

 `` script type="text/javascript ``: Esta tag indica que o conteúdo é JavaScript.

``<function timeMsg()>``{...}: Define a função timeMsg(). Esta função configura um temporizador para chamar alertMsg() após 3 segundos.
function alertMsg(){...}: Define a função alertMsg(). Esta função escreve "Terminal Root" no documento.

``<document.write("Terminal Root")>;:`` Esta linha escreve "Terminal Root" diretamente no documento HTML. No entanto, tenha em mente que o uso de document.write() após o documento ter sido carregado pode substituir completamente o conteúdo da página. Isso é considerado uma prática desatualizada e geralmente não é recomendado, pois pode causar problemas de acessibilidade e degradação do desempenho.

``<a href="#" onClick="timeMsg() a>``"Clique aqui a mensagem só aparecerá depois de 3 segundos: Este é um link  que, quando clicado, chama a função timeMsg(). Isso resulta na exibição do texto "Terminal Root" após um atraso de 3 segundos. O href="#" é usado para garantir que o link não redirecione para outra página quando clicado. O onClick="timeMsg()" atribui o evento de clique para chamar a função timeMsg() quando o link é clicado.
* o que o código faz?

O atraso de 3 segundos em JavaScript permite que você adie a execução de uma determinada tarefa por um período de tempo específico. Isso pode ser útil em diferentes cenários, como a exibição de uma mensagem temporizada, a realização de uma animação após um intervalo de tempo ou a implementação de um cronômetro.

# Abrir Pop-Up no Centro da Página 
![telainicial](print2.jpeg)


* analise do código

``<script>``: Indica o início de um bloco de script JavaScript.

``var win = null;:`` Declara uma variável global win e a inicializa como null. Essa variável será usada para armazenar a referência à janela que será aberta.

``function NovaJanela(pagina, nome, w, h, scroll)`` {...}: Define a função NovaJanela() que aceita cinco parâmetros: pagina (URL da página a ser aberta na nova janela), nome (nome da nova janela), w (largura da nova janela), h (altura da nova janela) e scroll (indica se as barras de rolagem devem estar visíveis ou não). Esta função calcula a posição da janela com base nas dimensões da tela e nas dimensões especificadas da nova janela. Em seguida, define as configurações da janela, como localização, barra de ferramentas, etc., e abre a nova janela com as configurações especificadas.

``LeftPosition = (screen.width) ? (screen.width-w)/2 : 0;`` e TopPosition = (screen.height) ? (screen.height-h)/2 : 0;: Calcula as coordenadas horizontais e verticais para posicionar a nova janela no centro da tela, com base nas dimensões da tela (screen.width e screen.height) e nas dimensões especificadas da nova janela (w e h).

``settings = 'location=no,toolbar=no,directories=no,status=no,height='+h+',width='+w+',top='+TopPosition+',left='+LeftPosition+',scrollbars='+scroll+',resizable';:`` Define as configurações da nova janela como uma string concatenada. Essas configurações determinam se elementos como barra de localização, barra de ferramentas, etc., estarão presentes na nova janela, bem como suas dimensões, posição e capacidade de redimensionamento.

``win = window.open(pagina, nome, settings);:`` Abre uma nova janela com a URL especificada em pagina, usando o nome especificado em nome e as configurações definidas em settings. A referência à nova janela é armazenada na variável win.

``</script>``: Indica o fim do bloco de script JavaScript.

``<a href="https://github.com/dashboard" onclick="NovaJanela(this.href,'nomeJanela','820','560','yes');return false">Abrir Pop-Up</a>: Este é um link <a>`` que, quando clicado, chama a função NovaJanela() com os parâmetros apropriados para abrir uma nova janela com a URL especificada ("https://github.com/dashboard"), um nome ("nomeJanela"), largura (820 pixels), altura (560 pixels) e barras de rolagem visíveis. O return false é usado para evitar que o link redirecione o navegador para a URL especificada. Em vez disso, a função NovaJanela() é chamada para lidar com a abertura da nova janela.