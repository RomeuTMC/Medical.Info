# Políticas e procedimentos de segurança 
Este documento descreve os procedimentos de segurança e políticas gerais para o projeto. nele você verá como proceder caso tenha alguma falha, Relatar um Bug, a nossa Política de Divulgação, e outros detalhes sobre esta política.
## Relatando um Bug 
A equipe e a comunidade levam a sério todos os bugs de segurança nos projetos. Obrigado por melhorar a segurança, e agradecemos seus esforços e a divulgação responsável e faremos todos os esforços para reconhecer suas contribuições. 

Relate bugs de segurança enviando um e-mail para o mantenedor líder. O mantenedor líder reconhecerá seu e-mail e enviará uma resposta mais detalhada, indicando as próximas etapas no tratamento de seu relatório. Após a resposta inicial, a equipe de segurança fará o possível para mantê-lo informado sobre o progresso para uma correção e um anúncio completo, e pode solicitar informações ou orientações adicionais. 

Relate bugs de segurança em módulos de terceiros para a pessoa ou equipe que mantém o módulo.

### Divulgação de falhas de maneira pública
A equipe é responsável pela gestão deste processo. Espera-se que os membros desta equipe mantenham todas as informações às quais tenham acesso privilegiado, em sigilo. Isso inclui concordar em não notificar ninguém fora da equipe sobre problemas que ainda não foram divulgados publicamente, incluindo a existência de problemas, expectativas de lançamentos futuros e correção de quaisquer problemas que não sejam no processo de seu trabalho como um membro.

### Como faço para enviar um relatório de bug bom? 
Bugs são rastreados como problemas no GitHub. Depois de determinar a qual repositório seu bug está relacionado, crie um problema nesse repositório e forneça as seguintes informações preenchendo o modelo. Explique o problema e inclua detalhes adicionais para ajudar os mantenedores a reproduzir o problema:

- Use um título claro e descritivo para identificar o problema. Descreva as etapas exatas que reproduzem o problema com o máximo de detalhes possível. Por exemplo, comece explicando como você iniciou o aplicativo, o instalou, por exemplo qual comando exatamente você usou no terminal, ou como você iniciou de outra forma. 
- Ao listar as etapas, não diga apenas o que você fez, mas explique como fez. Por exemplo, se você moveu o cursor para o final de uma linha, explique se você usou o mouse, ou um atalho de teclado ou um comando e, em caso afirmativo, qual? 
- Forneça exemplos específicos para demonstrar as etapas. Inclua links para arquivos ou projetos do GitHub, ou fragmentos de cópia / cola, que você usa nesses exemplos. Se você estiver fornecendo snippets no problema, use blocos de código Markdown. 
- Descreva o comportamento que você observou após seguir as etapas e indique qual é exatamente o problema com esse comportamento. Explique qual comportamento você esperava ver em vez disso e por quê. Inclua capturas de tela e GIFs animados se possivel, que mostram que você está seguindo as etapas descritas e demonstram claramente o problema. Se você usar o teclado enquanto segue as etapas, grave o GIF com o Resolvedor de Atalho mostrado. 
- Se estiver relatando um travamento, inclua um relatório de travamento com um rastreamento de pilha do sistema operacional. No macOS, o relatório de travamento estará disponível no Console.app em "Informações de diagnóstico e uso"> "Relatórios de diagnóstico do usuário". Inclua o relatório de falha do problema em um bloco de código, um anexo de arquivo ou coloque-o em uma essência e forneça um link para essa essência. 
- Se o problema estiver relacionado ao desempenho ou à memória, inclua uma captura do perfil da CPU em seu relatório. 
- Se o painel de ferramentas do desenvolvedor do Chrome puder ser mostrado, inclua dados da console dele, e tente executar no Modo de segurança ou atualizar a página e o cache. A menos para ver se isso corrige o problema. Se o problema não foi desencadeado por uma ação específica, descreva o que você estava fazendo antes de o problema acontecer e compartilhe mais informações usando as diretrizes abaixo.

Forneça mais contexto respondendo a estas perguntas: 
- É possivel Você reproduzir o problema no modo de segurança?
- O problema começou a acontecer recentemente (por exemplo, após a atualização para uma nova versão) ou sempre foi um problema? 
- Se o problema começou a acontecer recentemente, você pode reproduzir o problema em uma versão mais antiga? Qual é a versão mais recente em que o problema não acontece? Você pode baixar versões anteriores.
- Você pode reproduzir o problema de forma confiável? Caso contrário, forneça detalhes sobre a frequência com que o problema ocorre e em que condições normalmente ocorre. Se o problema estiver relacionado ao trabalho com arquivos (por exemplo, abrir e editar arquivos), o problema ocorre para todos os arquivos e projetos ou apenas para alguns? 
- O problema ocorre apenas ao trabalhar com arquivos locais ou remotos (por exemplo, em unidades de rede), com arquivos de um tipo específico (por exemplo, apenas arquivos de um determinado formato), com arquivos grandes ou arquivos com determinado tamanho? Há algo mais especial sobre os arquivos que você está usando?
- Qual é o nome e a versão do sistema operacional, navegador e servidor que você está usando? 
- Você está executando em uma máquina virtual? Em caso afirmativo, qual software VM você está usando e quais sistemas operacionais e versões são usados ​​para o host e o convidado? 