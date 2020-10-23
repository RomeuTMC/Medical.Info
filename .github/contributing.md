# Contribua com o projeto
Se você quer contribuir com nosso projeto, siga essas sugestões, que vão ajudar muito a equipe e também você a ter seu esforço aceito e fazendo parte do produto.
Seguir as regras e diretivas desse guia, vai ajudar a ter seus pull requests aceitos mais rapidamente, além de permitir que a equipe consiga avaliar mais rapidamente uma grande quantidade de código.

## Sua primeira contribuição 
Não sabe por onde começar a contribuir? Você pode começar examinando os problemas para iniciantes e para quem procura ajuda: 

De uma olhada nas issues e veja se o que você quer e pode fazer e que já não esta sendo discutido ou feito, se estiver em andamento, ótimo, você ainda pode participar da discussão e dar suas ideias, caso não esteja em andamento, você pode criar uma nova issue para discutirmos ou se preferir pode também mandar diretamente um pull request, só não esqueça de descrever muito bem o que você quer mudar/adicionar.

- Problemas para iniciantes - problemas que devem exigir apenas algumas linhas de código e um ou dois testes. 
- Problemas procurados por ajuda são problemas que devem ser um pouco mais envolvidos do que problemas de iniciante. Ambas as listas de problemas são classificadas pelo número total de comentários. Embora não seja perfeito, o número de comentários é um indicador razoável do impacto que uma determinada mudança terá. 
- Funcionalidades são novos recursos que podem fazer parte de uma nova versão ou feature do projeto, ou mesmo ser implementado como um plugin para o projeto em questão.

## Como Contribuir
Todas as mudanças de código acontecem por meio de solicitações pull. As solicitações pull são a melhor maneira de propor alterações na base de código (usamos o Github Flow). Acolhemos ativamente suas solicitações pull, para contribuir, siga esses passos: 
1. Faça um fork do repositório e crie seu branch a partir do master. 
2. Se você adicionou um código que deve ser testado, adicione testes. 
3. Se você mudou APIs, atualize a documentação também. 
4. Certifique-se de que o conjunto de testes seja aprovado. 
5. Certifique-se de que seu código seja executado sem falhas. 
6. Emita essa solicitação pull!

## Muito importante
Sempre que incluir ou modificar algo, junto com sua pull request, coloque também um arquivo de exemplo de uso se aplicavel, e testes que você tenha feito, para garantir que nenhuma funcionalidade seja conflitante.

### Variaveis, Constantes, Funções e Outros Nomes
Inicialmente todas as variáveis e funções eram escritas em ingles porque fica um código mais idiomaticamente homogêneo, mas para quem esta iniciando na linguagem é fácil confundir variáveis com palavras reservadas, então para resolver esse problema adotamos o português para nomes de variáveis. Fora do âmbito desse material é uma boa pratica nomear as variáveis em ingles.

Usamos a notação **CamelCase**, que é uma convenção de nomenclatura em que a primeira letra de cada palavra em uma palavra composta é maiúscula, exceto para o primeiro caractere que indicam o seu tipo. Os desenvolvedores de software costumam usar camelCase ao escrever o código-fonte.

Um prefixo da **Notação Húngara** também é usado, para identificar o tipo da variável, Como o PHP e outras linguagens como JavaScript não tem tipos de dados rigidamente definidos, nada na linguagem em si ajuda um programador a lembrar os tipos de variáveis. A notação húngara visa remediar isso, fornecendo ao programador conhecimento explícito do tipo de dados de cada variável.

Usamos como convenção, que o primeiro ou primeiros caractere do nome da variável indica o seu tipo, por exemplo: wNome significa que ela é word ou seja, que contém texto e que pode ser composta por palavras separadas. iIdade indica que é um inteiro (integer). Veja abaixo os mnemonicos utilizados e que podem ser vistos em diversas documentações sobre a notação húngara.

| Mnemonico | Descrição | Exemplo |
|--|--|--|
| b | Boolean / Boleano | bValidado - Verdadeiro ou Falso |
| rg | Range - Um valor de faixa | rgTipo - Pode ser uma sequencia de números, ou palavras que limitam um grupo de dados, tipo um conjunto, geralmente do tipo array ou lista unidimensionais |
| ch | Char - Cadeia de Caracteres | chPais - Abreviação do Nome de Pais |
| w | Words - Cadeia de Caracteres separadas por espaço | wNome - Nome Completo com sobrenome |
| t | Text - Texto ou Html ou Markdown | Texto longo, com paragrafos e mascação de estilo markdown, html, ou texto puro |
| c | Count - Contador | cI - Contador para um laço, ou iterações, é sempre maior ou igual a zero |
| f | Float - Numeros decimais ou pontos flutuantes | fPorcento - Um valor de porcentagem |
| n | Numerico - Numero real, com ou sem valor decimal | nValor - Valor do Produto |
| i | Inteiro - Numero | iIdade - Numero não fracionario, positivo, zero ou negativo |
| p | Ponteiro - Um valor que aponta para outro | pArgument - Um argumento passado obrigatóriamente por referência, ou que aponta a uma posição de outra variável |
| arr | Array - Um array multidimensional ou não com um conjunto de tipos de dados | Uma listagem ou subconjunto, com multiplas dimensões ou não, no formato chave:valor onde valor também pode ser um conjunto |
| j | JSON - Conjunto JSON | Um Conjunto seguindo a estrutura JSON |
| x | XML - Conjunto XML | Um conjunto seguindo a estrutura XML |
| a | Archive - Um ponteiro para um Arquivo | aFoto - Ponteiro para um arquivo no sistema de arquivos local |
| u | Url | Endereço seguindo o padrao web proto://address/caminho/caminhox/file.ext |
| m | Mail | Endereço seguindo o padrão web de email nome@dominio.com |
| bb | Blob - Binario | Sequencia binária como um arquivo de imagem ou outro formato, em base64 |
| h | Hash | Hash de um conteúdo, pode ter um subtipo ex. hsha1Senha - Senha no formato sha1, ou hmd5Senha senha no formato md5 |
| rgb | Cor | #RRGGBBAA ou #RGBA ou #RRGGBB ou #RGB Parametro de cor no formato web, com ou sem transparência |
| cd | Coordenada X,Y | Uma notação de coordenada no formato X,Y ou |
| ht | Humam Time - Um Timestamp em Formato Humano | htDataNascimento - Pode ser data ou hora ou ambos, de maneira inteligivel a umanos, por exemplo dd-mm-yyyy |
| st | Sistem Time - Um Timestamp padrão UNIX | stCadastro - Data e Hora completos padrão UNIX |
| d | Date - Formato de Data | dNascimento - Formato de data, completa ou abreviada |
| t | Time - Formato de Hora | tConsulta - Um Horario no padrão hh:mm:ss completo ou não |
| _g | Global - Escopo| Usado para definir algo que possua o escopo GLOBAL DB_g - Ponteiro do Banco de Dados|
| _s | Static - Escopo | Usado para métodos estáticos |
| _p | Public - Escopo | Usado para Métodos públicos |

### Padrões de codificação - Identação e Boas Práticas
Você é livre para utilizar o código da maneira que preferir, e utilizar os padrões e nomenclaturas e realizar uma cópia (fork) do projeto adaptando-o ao seu estilo, desde que siga as diretrizes da licença, e mantenha os créditos de cada autor em cada parte do código utilizado.

Quando você estiver fazendo alguma edição, que possa ser submetida ao repositório oficial através de um pull request, seguimos alguns padrões, também não só de nomenclatura, como algumas regras para melhorar o fluxo de trabalho da equipe. São eles:

- Desenvolva apenas em seu branch. 
- Faça rebase com o master antes de criar pull requests.
- Faça rebase do master em seu branch diariamente, ou sempre que finalizar uma edição.
- Faça squash dos seus commits que não estão completos (Work In Progress).

Quando você estiver codificando, não idente (recue) o código usando tabulação (configure para substituir a tabulação por 3 espaços), dessa maneira seu código fica legível e dentro dos principais padrões aceitos.

Não use underscore (_) fora do nome de constantes. Nem nome de variavel igual a nome de função ou de constantes nem use palavras em idiomas diferentes, convencionamos que as variavéis, constantes e nomes de funções e métodos são escritos em portugues sem acentuação gráfica. Porém, aceitamos seus nomes em Inglês como um segundo idioma.

Use uma linha em branco, para espaçar o inicio/fim de uma função, método ou classe dentro de um mesmo arquivo fonte. Da mesma maneira, coloque em um mesmo arquivo conteúdos relacionados, agrupados pela funcionalidade ou racionalidade.

Evite funções que repitam o código, se existe alguma repetição, pense em refatorar o código, e não sobrecarregar uma determinada função.

Evite uso de retornos e tipos null (nulos) prefira uso de valores como false. Em exceções, use as clausulas de finalização para fechar buffers de saida, conexões abertas e mesmo entrada e saída em arquivos.

Utilize sempre os recursos das versões mais recentes do repositório estable das linguagens, e de outros recursos, evite a utilização de versões antigas e versões beta ou futuras.

Testes e depuração fazem parte e devem estar presentes em todas as funcionalidades.

## Documentando o código
Quando for documentar o seu código, o faça no próprio corpo do arquivo, utilize um cabeçalho, onde todas as funções, autor, requisitos sejam claros. Utilize os comentários de linha e de bloco para colocar comentários no meio de um código.

Todos nós pensamos que nosso código faz sentido - especialmente se ele funcionar - mas outra pessoa talvez não. Para combater isso, todos nós precisamos melhorar os comentários do código-fonte. Dessa forma, quem vier acompanhar o projeto terá um caminho claro para entender e melhorar / consertar nosso código. Os princípios básicos de comentar seu código são simples: Faça-os breves; Mantenha-os relevantes; Use-os liberalmente, mas não em excesso; Se você puder manter isso em mente, você estará indo muito bem.

Os principais são que nem sempre você será o único trabalhando no projeto, e você não pode garantir o quão experiente a próxima pessoa será. Mesmo se você escrever um bom código, há uma chance de confusão e ambiguidade.

### Crie Tutoriais
Caso tenha adicionado uma funcionalidade, crie tutoriais para ensinar como instalar, utilizar e os recursos dessa funcionalidade.

Se criou uma API, não se esqueça de colocar na documentação, e adicionar exemplos de chamadas em algumas linguagens, utilização de parâmetros e opcionais.

Como padrão, utilizamos as ferramentas do [POSTMAN API Documentation Tool](https://www.postman.com/api-documentation-tool/). Para criar os exemplos de chamadas e as documentações para a API's em geral.

### Documentação do Bloco de Cabeçalho e Comentários
Se você olhar em alguns arquivos, o código não começa imediatamente porque há um grande cabeçalho no arquivo que descreve qual é o seu propósito, autores, datas e detalhes simples. Mantenha a coerência e seja básico. Comentários de cabeçalho são úteis no código-fonte para explicações simples sobre o que esperar desse arquivo.

Um changelog pode ser adicionado, no cabeçalho, o que pode ser removido, e é util, principalmente se você incluiu uma nova função, mais ainda faltam subsistemas para ela, que possam ser incluídos por outra pessoa, ou que você possa incluir em outro commit.

Antes de declarar uma função ou método, você pode especificar os dados específicos para aquele bloco de código, como métodos, variáveis entradas e saídas. Isso se aplica a qualquer declaração.

Um comentário de linha, pode ser muito útil, para identificar um padrão ou algo esperado como uma formatação (99) 99999-9999 ou variações dela que podem ser aceitas.

### Não se prolongue demais
Uma das características que é importante manter são exemplos curtos e de fácil entendimento, tente fazer com que os exemplos caibam em uma tela, tudo bem se não for possível, apenas mantenha isso em mente.

Exemplos rápidos, curtos, diretos e de fácil entendimento são nossa meta.

## Sugestão de melhorias 
Esta seção o orienta no envio de uma sugestão de aprimoramento para o produto, incluindo recursos completamente novos e pequenos aprimoramentos na funcionalidade existente. 

Seguir essas diretrizes ajuda os mantenedores e a comunidade a entender sua sugestão e encontrar sugestões relacionadas. Antes de criar sugestões de melhorias, verifique na lista de implementações, pois você pode descobrir que não precisa criar uma, pois ela já pode estar lá. 

Ao criar uma sugestão de melhoria, inclua o máximo de detalhes possível. Preencha um modelo, incluindo as etapas que você imagina que realizaria se o recurso que está solicitando existisse.

Mais importante, verifique se você está usando a versão mais recente e se pode obter o comportamento ou funcionalidade desejado alterando as configurações ou atualizando. Verifique se já existe um pacote que fornece esse aprimoramento, ou algum plugin. 

Faça uma pesquisa rápida para ver se a melhoria já foi sugerida. Se tiver, adicione um comentário ao que já existe em vez de abrir um novo, dessa maneira, podemos ver quais as sugestões são mais pedidas.

### Como faço para enviar uma boa sugestão de aprimoramento? 
Depois de determinar a qual é sua sugestão de aprimoramento, crie um problema nesse repositório e forneça as seguintes informações: 
- Use um título claro e descritivo para o problema para identificar a sugestão. 
- Forneça uma descrição passo a passo do aprimoramento sugerido com o máximo de detalhes possível.
- Forneça exemplos específicos para demonstrar as etapas. Inclua fragmentos de cópia / cola ​​que você usa nesses exemplos, como blocos de código Markdown. 
- Descreva o comportamento atual e explique qual comportamento você esperava ver e por quê. 
- Inclua capturas de tela e GIFs animados que ajudam a demonstrar as etapas ou apontam a parte à qual a sugestão está relacionada.
- Você pode usar um outro software para explicar esse aprimoramento, como seria útil para a maioria dos usuários e não é algo que pode ou deve ser implementado como um pacote diferente.
- Liste alguns outros aplicativos onde existe esse aprimoramento. Especifique qual versão.

## Notas Adicionais 
### Etiquetas de emissão e solicitação de pull 
Esta seção lista os rótulos que usamos para nos ajudar a rastrear e gerenciar problemas e solicitações de pull. A maioria dos rótulos são usados ​​em todos os repositórios, mas alguns são específicos. 

A pesquisa do GitHub facilita o uso de rótulos para encontrar grupos de problemas ou solicitações de pull de seu interesse. Por exemplo, você pode estar interessado em questões abertas.

Incentivamos você a ler sobre outros filtros de pesquisa que o ajudarão a escrever consultas mais específicas. Os rótulos são agrupados livremente por sua finalidade, mas não é necessário que cada problema tenha um rótulo de cada grupo ou que um problema não possa ter mais de um rótulo do mesmo grupo. 

Abra um problema se tiver sugestões para novos rótulos e se notar que alguns rótulos estão faltando em alguns repositório.

### Licenças de código
Todos os códigos enviados por você, que sejam incluídos no projeto, estarão licenciados sobre a mesma licença do projeto, disponível no arquivo LICENSE na raiz do projeto.

