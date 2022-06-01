# 100 Days Of Code - Log

O log do meu desafio #100DaysOfCode. Iniciado em [24 de abril, domingo, 2022].

### Dia 21: 18 de maio de 2022

**Progresso do dia:** Passei uma props de um componente para outro. Eu não sabia bem como fazer, mas sabia que eu já tinha visto em algum lugar. Fiz alguns testes e pegou. A ideia era mostrar o nome de um usuário específico no modal de pagamento.

**Aprendizados:** Passei props na função PaymentModal {PaymentModal(props)}, no próprio modal, passei um props.name. E na lista de usuários UserList, dentro do PaymentModal que já tá importado, chamei name=user.name. Tô percebendo que a minha grande dificuldade com React é entender onde que as coisas vão. Ainda parece tudo meio alienígena.

**Github:** [Repositório](https://github.com/sarahrubia/app-pagamentos)
**Github:** [Github Pages](https://sarahrubia.github.io/app-pagamentos/)

### Dia 22: 19 de maio de 2022

**Progresso do dia:** Hoje eu só quebrei a cabeça. Nossa, fiquei um tempão pensando como criar um modal dentro de um modal. Depois pensei que não deve ser um modal dentro de um modal, mas uma atualização do modal. Como que faz isso? Vi várias coisas e não cheguei a uma conclusão. Aí eu fui assistir uns plantões de dúvidas do curso, pra ver se alguém tava tendo o mesmo problema que eu. E, sim, tinha gente que nem sabia por onde começar, como eu. Resolveram a dúvida da pessoa? Não hahaha. 

**Aprendizados:** Depois eu achei um [vídeo](https://www.youtube.com/watch?v=x9UEDRbLhJE) que nem é sobre modal, mas sobre usar o método POST, algo que eu também preciso fazer. E algumas coisas começaram a fazer sentido. Foi um dia de reflexões, muito mais do que programações.

**Github:** [Repositório](https://github.com/sarahrubia/app-pagamentos)
**Github:** [Github Pages](https://sarahrubia.github.io/app-pagamentos/)

### Dia 23: 20 de maio de 2022

**Progresso do dia:** Fiz um request API com axios e o método POST, mas não consegui integrar isso com a interface do modal. Tô com dificuldade. E aí tem um array de objetos com dados de cartões de crédito que eu preciso adicionar em um elemento Select dentro do formulário no modal, que depois vai fazer essa requisição aí que eu não integrei a nada. Será que eu tô entendendo direito?

**Aprendizados:** Requisição API do método POST com axios.

**Github:** [Repositório](https://github.com/sarahrubia/app-pagamentos)
**Github:** [Github Pages](https://sarahrubia.github.io/app-pagamentos/)

### Dia 23: 23 de maio de 2022

**Progresso do dia:** Eu acordei de madrugada pensando "e se eu fizesse um loop for desse jeito?", anotei e fiz os testes hoje. Criei uma função para adicionar os cartões (cards) como <option> no <select>. Mas eu não consigo adicioná-lo na página/no modal. Quando tento, acho que a página ainda não renderizou e fica dando selectCard is null. Quando a página já está renderizada e eu atualizo o navegador com o modal aberto, os cartões aparecem no <select> (ainda aparecem errado porque tá renderizando por usuário, aí aparece 33 vezes kkkk mas uma coisa de cada vez). Fiquei com a questão: como faço para os cartões aparecerem no momento que a página renderiza? Em que lugar eu adiciono essa função e como a chamo?  

Comecei a assistir o curso [ReactJS Tutorial for Beginners](https://youtube.com/playlist?list=PLC3y8-rFHvwgg3vaYJgHGnModB54rxOk3), senti que ainda me falta entender porque algumas coisas acontecem.

**Aprendizados:** Popular select com options usando js. Comecei a entender sobre a renderização da página, em que momento as coisas passam a aparecer nela. Pedi a ajuda do Dobrado e do Juaox, que me indicaram trabalhar com State pra fazer alterações no que está sendo renderizado.

Ainda tô pensando no React com a cabeça de JavaScript xD

**Github:** [Repositório](https://github.com/sarahrubia/app-pagamentos)
**Github:** [Github Pages](https://sarahrubia.github.io/app-pagamentos/)

### Dia 24: 25 de maio de 2022

**Progresso do dia:** Um colega me explicou como popular o <select> com <option> usando map() no React, basicamente era fazer o map com o array de objetos dentro do return, retornando as tags <option> com o conteúdo mapeado. Fiquei com raiva porque era algo tão bobo e eu tava quebrando a cabeça, dificultando tudo como sempre hahaha. Agora eu preciso pegar os dados do usuário, o valor do input e os dados do cartão selecionado pra enviar pelo método POST. Parece que tem que usar state/setState, mas eu ainda não tô amiga dessas coisas. Consegui fazer o método POST num componente de classe, mas não sei como fazer num componente funcional.

**Aprendizados:** Popular select com options usando map no retorno da função.

**Github:** [Repositório](https://github.com/sarahrubia/app-pagamentos)
**Github:** [Github Pages](https://sarahrubia.github.io/app-pagamentos/)

### Dia 25: 26 de maio de 2022

**Progresso do dia:** Acho que eu passo mais tempo olhando pra esse código do que fazendo, de fato, alguma coisa hahaha. Levei algumas dúvidas pro plantão de dúvidas da Newtab Academy com relação ao uso de state/setState, e como colocar mais de um onChange em um componente, que eu não sabia se era possível. Na minha cabeça, o React parece menos flexível do que ele é. Ainda não consegui me acostumar com essa fera. Mas vamo que vamo!

**Aprendizados:** Eu descobri que o onChange de um componente pode receber várias funções. E que um componente pode receber dados de vários lugares. Eu acabo me prendendo ao que está dentro do componente.

**Github:** [Repositório](https://github.com/sarahrubia/app-pagamentos)
**Github:** [Github Pages](https://sarahrubia.github.io/app-pagamentos/)

### Dia 26: 27 de maio de 2022

**Progresso do dia:** Mais um dia, a mesma questão dos dias anteriores. Algo de errado não está certo e eu ainda não sei o que é. Tô bem frustrada, mas acho que faz parte. 

**Github:** [Repositório](https://github.com/sarahrubia/app-pagamentos)
**Github:** [Github Pages](https://sarahrubia.github.io/app-pagamentos/)

### Dia 27: 30 de maio de 2022

**Progresso do dia:** Finalmente saiu! Acho que eu tava definindo o state e o setState certinho, mas, por algum motivo, eu tinha que chamar o state, tipo: setState({...state, outros objetos}). Eu não entendi muito bem porque, mas depois disso funcionou. A partir daí eu consegui criar o objeto e enviar pelo método POST pra verificar se a transação foi aprovada ou não. Agora tô com uns probleminhas de formatação na máscara de valor... Ai, ai... Bom demais programar.

**Aprendizados:** Estou entendendo melhor o state e o setState.

**Github:** [Repositório](https://github.com/sarahrubia/app-pagamentos)
**Github:** [Github Pages](https://sarahrubia.github.io/app-pagamentos/)

### Dia 28: 31 de maio de 2022

**Progresso do dia:** Então, a máscara de valor monetário... Eu tentei usar um codigozinho em JavaScript e a formatação até funcionou, só que usando o evento onKeyDown, o backspace não pega, e no onKeyUp o backspace pega, mas fica repetindo as teclas. E, pelo que eu entendi, o onkeypress não funciona no React. Ok. Encontrei um componente React que faz toda a formatação direitinho (react-intl-currency-input), fiz a importação dele e tá pegando. Só que, na hora de fazer a requisição pelo método POST, o valor vai formatado errado. Mas acho que eu queria mesmo era pegar o valor numérico do input e não a string. Tentei converter de algumas formas, mas não pegou. 

**Aprendizados:** Importar componentes prontos, como o react-intl-currency-input, e utilizá-lo na aplicação.

**Github:** [Repositório](https://github.com/sarahrubia/app-pagamentos)
**Github:** [Github Pages](https://sarahrubia.github.io/app-pagamentos/)

### Dia 29: 01 de junho de 2022

**Progresso do dia:** Removi o componente de valor monetário e substituí por um código em JavaScript puro pra fazer a formatação da moeda. Ao invés de usar os "onKey", sugeriram que eu usasse o onChange, depois disso tudo funcionou perfeitamente. Como agora eu tinha mais liberdade pra mexer com os valores inseridos, formatados ou não, criei um setState para o valor em string e outro em float, assim, consegui mostrar no input o valor formatado e, ao fazer a requisição POST, consegui mandar o valor numérico.

**Aprendizados:** Acho que, finalmente, o state/setState/useState estão fazendo sentido pra mim. 

**Github:** [Repositório](https://github.com/sarahrubia/app-pagamentos)
**Github:** [Github Pages](https://sarahrubia.github.io/app-pagamentos/)
