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
