# atrasando no tempo 
![telainicial](print.jpeg)
* analise do código 💻

## `` script type="text/javascript ``: Esta tag indica que o conteúdo é JavaScript.

``<function timeMsg()>``{...}: Define a função timeMsg(). Esta função configura um temporizador para chamar alertMsg() após 3 segundos.
function alertMsg(){...}: Define a função alertMsg(). Esta função escreve "Terminal Root" no documento.

``<document.write("Terminal Root")>;:`` Esta linha escreve "Terminal Root" diretamente no documento HTML. No entanto, tenha em mente que o uso de document.write() após o documento ter sido carregado pode substituir completamente o conteúdo da página. Isso é considerado uma prática desatualizada e geralmente não é recomendado, pois pode causar problemas de acessibilidade e degradação do desempenho.

``<a href="#" onClick="timeMsg() a>``"Clique aqui a mensagem só aparecerá depois de 3 segundos: Este é um link  que, quando clicado, chama a função timeMsg(). Isso resulta na exibição do texto "Terminal Root" após um atraso de 3 segundos. O href="#" é usado para garantir que o link não redirecione para outra página quando clicado. O onClick="timeMsg()" atribui o evento de clique para chamar a função timeMsg() quando o link é clicado.
* o que o código faz?

O atraso de 3 segundos em JavaScript permite que você adie a execução de uma determinada tarefa por um período de tempo específico. Isso pode ser útil em diferentes cenários, como a exibição de uma mensagem temporizada, a realização de uma animação após um intervalo de tempo ou a implementação de um cronômetro.