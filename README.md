# conceitos-mvc

Nesta aula, trabalharemos com um conceito de desenvolvimento em camadas, o
MVC. Durante o desenvolvimento, é necessário que diversos passos sejam executados para que ele possa ter uma qualidade eficaz, ou seja, é necessário que se
tenha um roteiro que o software precisa seguir de acordo com suas necessidades,
e este passo é chamado de Processo de Software (PRESSMAN; MAXIM, 2016).
Para Sommerville (2011, p. 18), existem diversos processos de software diferentes, mas todos devem incluir quatro atividades que são consideradas fundamentais para a Engenharia de Software:

1. **Especificação de software**. A funcionalidade do software e as restrições a seu funcionamento devem ser definidas.
2. **Projeto e implementação de software**. O software deve ser produzido para atender às especificações.
3. **Validação de software**. O software deve ser validado para garantir
que atenda às demandas do cliente.
4. **Evolução de software**. O software deve evoluir para atender às
necessidades de mudança dos clientes

> Fonte: ALVES, F. Modelos de Aplicação do Back End. In: Bezzera, 2007 **Programação back end II**. 22.ed. Maringa, PR: Centro Universiário de Maringá, 2019. p. 203

Contudo, Pressman e Maxim (2016) afirmam que, para que o desenvolvimento de
software possa alcançar o resultado final, é necessário que se tenha uma arquitetura
de software condizente com o processo. Algumas delas são: **arquitetura centralizada
em dados**; **arquitetura de fluxo de dados**; **arquitetura de chamada e retorno**; **arquitetura orientada a objetos**; **arquitetura em camadas**; e **arquitetura MVC**. 

De acordo com Pressman e Maxim (2016, p. 230):

> A arquitetura de software de um programa ou sistema computacional é
a estrutura ou estruturas do sistema, que abrange os componentes de
software, as propriedades externamente visíveis desses componentes e
as relações entre eles

Dentre as arquiteturas citadas anteriormente, aprofundaremos nossos conhecimentos na arquitetura MVC, sendo esta a mais utilizada para o desenvolvimento
de sistemas Web. Esta, por sua vez, tem por objetivo auxiliar os desenvolvedores
a construir aplicações, separando seus principais componentes. Essa separação
ocorre com a manipulação e armazenamento dos dados (**Model**), as funções que
trabalharão com as entradas dos dados (**Controller**) e a visualização do usuário
(**View**). Estudaremos cada uma dessas camadas ou componentes separadamente.

A camada **Model** contém toda a comunicação com os dados armazenados
que serão visualizados na camada View, que podem estar armazenados em um
banco de dados, em um JSON, em um arquivo XML, em um arquivo, entre outros locais. Toda a manipulação de dados acontece em um SGBD (comandos de
manipulação: create, reader, update e delete), o famoso (CRUD), com um banco
de dados relacional, ou não deve ocorrer nesta camada, ou seja, é ela que conterá
um maior nível de abstração do sistema.

A camada **View** trabalha apenas com a apresentação dos dados da aplicação,
passando ao usuário final uma confiança de que tudo está se realizando no seu terminal. É nesta camada que se tem os frameworks de front-end, templates, entre outros.

Enquanto isso, a camada **Controller** é responsável por administrar todo o
fluxo da aplicação. Nesta camada, é onde ocorre toda a movimentação da aplicação, ou seja, a partir da entrada de uma View, ela resolve qual operação utilizará
da camada Model e, assim, devolverá a sua View correspondente junto aos dados.
Confira, na figura a seguir, o fluxo de dados da arquitetura MVC.

![OrganizacaoMVC](../img/OrganizacaoMVC.png)

> Figura 1 - A organização do MVC / Fonte: Sommerville (2011, p. 109).

De forma análoga, a aplicação do MVC para WEB não é tão diferente, altera-se
apenas o tipo de fluxo, como podemos perceber na Figura 2.

![ArquiteturaDeAplicacoesMVC](../img/ArquiteturaDeAplicacoesMVC.png)

> Figura 2 - Arquitetura de aplicações Web usando o padrão MVC
Fonte: Sommerville (2011, p. 110)


Como em toda arquitetura, o MVC possui algumas vantagens e desvantagens.
Veja, no quadro a seguir, alguns apontamentos:

![VantagensXDesvantagens.png](..img/VantagensXDesvantagens.png)
> Quadro 1 - Vantagens e desvantagens da arquitetura MVC / Fonte: os autores.

Não há uma receita de bolo que indique a melhor arquitetura a se utilizar, pois
sempre que um sistema for desenvolvido, terá, com certeza, a necessidade de
manutenção, como melhorias ou correção de erros, e, também, pode necessitar
de várias atualizações. Assim, o MVC vem a calhar com a manutenção exclusiva
das camadas da aplicação.

> Fonte: ALVES, F. Modelos de Aplicação do Back End. In: Bezzera, 2007 **Programação back end II**. 22.ed. Maringa, PR: Centro Universiário de Maringá, 2019. p. 204-206
