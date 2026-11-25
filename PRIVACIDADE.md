# Política de Privacidade — Quem Não Me Segue

Extensão para Google Chrome e navegadores compatíveis (Microsoft Edge, Brave e outros baseados em Chromium).  
Vigente a partir de 25 de novembro de 2026 · Versão da extensão coberta: 1.5.0 e posteriores.

**Resumo em poucas linhas**

- A extensão só **lê** as listas de “seguindo” e “seguidores” da conta do Instagram que já está aberta no seu navegador. Ela **não segue, não deixa de seguir, não curte, não comenta** e não faz nenhuma outra ação na sua conta.
- **Nunca pedimos, lemos ou guardamos a sua senha.**
- **Todos os dados ficam somente no seu navegador**, no seu computador. Nada é enviado para servidores do desenvolvedor ou de terceiros. O desenvolvedor não tem acesso a nenhum dado seu.
- A extensão só se comunica com o próprio Instagram (`instagram.com`) e com os servidores de imagem dele, para baixar as fotos de perfil.
- Não há anúncios, rastreadores, ferramentas de análise (analytics), contas de usuário nem cobrança. A extensão é **totalmente gratuita**.
- Para apagar tudo, basta remover a extensão do navegador.


## 1. Quem somos e a quem se aplica

“Quem Não Me Segue” (“a extensão”) é uma extensão de navegador gratuita, de desenvolvedor independente, publicada na Chrome Web Store. Esta política explica, de forma completa, quais informações a extensão usa, como, para quê e onde elas ficam. Ela se aplica a todas as pessoas que instalam e usam a extensão.

Esta política foi escrita em conformidade com a Lei Geral de Proteção de Dados Pessoais (Lei nº 13.709/2018 — LGPD) e com a Política de Dados do Usuário do Programa para Desenvolvedores da Chrome Web Store.

## 2. Princípio: tudo fica no seu navegador

A extensão foi construída para funcionar **inteiramente no seu computador**. Não existe servidor, banco de dados ou serviço em nuvem do desenvolvedor. Todo o processamento — ler as listas, comparar quem segue quem, montar o relatório, baixar as fotos, gerar o CSV — acontece dentro do seu navegador. Os resultados são guardados no armazenamento local da própria extensão (`chrome.storage.local`), que só pode ser lido pela extensão no seu navegador.

Por isso, **o desenvolvedor não coleta, não recebe, não vê e não tem como acessar** nenhuma informação sua ou dos perfis que aparecem nas suas listas.

## 3. Quais dados a extensão usa

Para cumprir sua única finalidade, a extensão lida com as informações abaixo. Todas são obtidas do Instagram, com a sua sessão, e guardadas apenas no seu navegador.

| Dado                                                                               | Exemplo                                                                                                                                                                                              | Por que é necessário                                                                                                  |
|------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------|
| Identificador numérico da sua conta do Instagram                                   | `1234567890`                                                                                                                                                                                         | Saber de qual conta buscar as listas e separar os resultados caso você use mais de uma conta no mesmo navegador.      |
| Seu @usuário, nome de exibição, foto de perfil e quantidade de seguidores/seguindo | @seu.perfil · 70 seguindo · 165 seguidores                                                                                                                                                           | Mostrar no painel e no relatório de qual conta é a análise e calcular o progresso.                                    |
| Lista de perfis que você segue                                                     | Para cada perfil: identificador numérico, @usuário, nome de exibição, link da foto de perfil, se é verificado e se é privado                                                                         | Comparar com a lista de seguidores e montar a lista de quem não te segue de volta.                                    |
| Lista dos seus seguidores                                                          | Os mesmos campos acima                                                                                                                                                                               | Comparar com quem você segue e detectar quem deixou de te seguir entre uma verificação e outra.                       |
| Miniaturas das fotos de perfil                                                     | Imagem de 96×96 pixels                                                                                                                                                                               | Exibir as fotos no relatório. Os links originais do Instagram expiram em poucos dias e não abrem fora do site.        |
| Histórico de quem deixou de te seguir                                              | @usuário, nome, foto, data e hora em que foi detectado, se você ainda segue a pessoa, se ela voltou a seguir                                                                                         | Mostrar o histórico e enviar o aviso de “deixou de te seguir”.                                                        |
| Preferências e estado da extensão                                                  | Monitoramento ligado/desligado, intervalo escolhido, data da próxima verificação, progresso de uma verificação em andamento                                                                          | Funcionamento do monitoramento e possibilidade de pausar e continuar uma verificação.                                 |
| Registros técnicos de segurança                                                    | Horários das últimas consultas (última hora), horário até quando as consultas estão pausadas, última mensagem de erro do Instagram (até 160 caracteres), identificador da aba usada nas verificações | Respeitar o limite de consultas por hora, pausar quando o Instagram pedir e mostrar ao usuário o motivo de uma falha. |

Na classificação da Chrome Web Store, esses dados se enquadram em **“Informações de identificação pessoal”** (nomes e @usuários de perfis) e **“Conteúdo do site”** (listas e imagens lidas do Instagram).

## 4. Dados que a extensão NÃO usa

- **Senhas, códigos de verificação ou qualquer credencial.** A extensão nunca pede, lê, digita ou guarda sua senha.
- **Mensagens diretas (Direct), conversas, comentários ou e-mails.**
- **Publicações, stories, curtidas ou qualquer conteúdo do seu feed.**
- **Histórico de navegação.** A extensão só funciona no instagram.com e não registra quais outros sites você visita.
- **Atividade do usuário:** cliques, teclas digitadas, movimentos do mouse ou rolagem.
- **Localização**, endereço IP, dados de saúde, dados financeiros ou de pagamento.
- **Dados de outras redes sociais ou de outros sites.**

## 5. Como os dados são obtidos

Quando você clica em “Verificar agora”, abre o painel no Instagram ou deixa o monitoramento ligado, a extensão faz, dentro de uma aba do instagram.com, as mesmas consultas de leitura que o próprio site faz quando você abre as listas de “seguindo” e “seguidores” do seu perfil. Essas consultas usam a sessão que você já tem aberta no navegador.

As consultas são feitas de forma lenta e controlada (veja a seção [Segurança](#12-segurança-e-proteção-da-sua-conta)). A extensão só lê informações da **sua própria conta**: ela não consulta listas de outras pessoas.

Com o monitoramento ligado, a extensão mantém uma aba do instagram.com fixada no navegador e repete a verificação no intervalo escolhido por você (6, 12 ou 24 horas). O monitoramento vem **desligado** e só funciona se você ligar.

## 6. Para que os dados são usados

Os dados são usados **exclusivamente** para a única finalidade da extensão:

- mostrar a lista de perfis que você segue e que não te seguem de volta;
- avisar quando alguém deixar de te seguir e manter o histórico disso;
- permitir buscar, filtrar, ordenar e exportar essas listas.

Os dados **não** são usados para publicidade, criação de perfis de comportamento, venda, análise de crédito, treinamento de inteligência artificial ou qualquer outra finalidade.

## 7. Onde e por quanto tempo ficam guardados

**Onde:** somente no armazenamento local da extensão no seu navegador (`chrome.storage.local`), no seu computador. Esse espaço é isolado: sites, outras extensões e o desenvolvedor não têm acesso a ele.

**Por quanto tempo:**

- A lista de “não me seguem de volta” é **substituída** a cada nova verificação; só a mais recente fica guardada.
- A lista de seguidores usada para comparação também é substituída a cada verificação.
- O histórico de quem deixou de te seguir guarda no máximo os **500 registros mais recentes**; os mais antigos são apagados automaticamente.
- As miniaturas de foto são apagadas automaticamente quando o perfil deixa de aparecer nas listas.
- Os registros de horário das consultas guardam apenas a **última hora**.
- O progresso de uma verificação é apagado quando ela termina.
- Todo o resto fica guardado até você **remover a extensão**, o que apaga tudo de forma imediata e definitiva.

Os dados permanecem salvos ao fechar e reabrir o navegador. Se você usar a sincronização do Chrome, os dados da extensão **não** são sincronizados com outros computadores, porque a extensão usa somente o armazenamento local, e não o armazenamento sincronizado.

## 8. Compartilhamento com terceiros

**Nenhum dado é vendido, alugado, compartilhado ou transferido** para o desenvolvedor ou para terceiros. Não existem parceiros, anunciantes, provedores de análise ou serviços de nuvem envolvidos.

A única comunicação externa é com o próprio Instagram, para ler as listas e as fotos, conforme a seção a seguir. O Instagram é operado pela Meta Platforms, Inc., e o uso que ela faz dos seus dados é regido pela <a href="https://privacycenter.instagram.com/policy" rel="noopener">Política de Privacidade do Instagram</a>.

## 9. Conexões de rede feitas pela extensão

Para total transparência, esta é a lista completa de endereços com os quais a extensão se comunica:

| Endereço                                                                            | Para quê                                                                                                                                                   |
|-------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `https://www.instagram.com/api/v1/friendships/…/following/`                         | Ler a lista de perfis que você segue.                                                                                                                      |
| `https://www.instagram.com/api/v1/friendships/…/followers/`                         | Ler a lista dos seus seguidores.                                                                                                                           |
| `https://www.instagram.com/graphql/query/`                                          | Plano alternativo de leitura das mesmas listas, usado só se o anterior falhar.                                                                             |
| `https://www.instagram.com/api/v1/friendships/show_many/`                           | Somente em contas com muitos seguidores: consultar, em lotes, se os perfis que você segue te seguem de volta. É uma consulta de leitura e não altera nada. |
| `https://www.instagram.com/api/v1/users/…/info/` e `/api/v1/accounts/current_user/` | Ler o @usuário e os totais de seguidores/seguindo da sua conta.                                                                                            |
| `https://*.cdninstagram.com/` e `https://*.fbcdn.net/`                              | Servidores de imagem do Instagram: baixar as fotos de perfil para gerar as miniaturas.                                                                     |

A extensão **não** faz nenhuma outra conexão: não acessa servidores próprios, não carrega scripts externos e não envia estatísticas de uso.

## 10. Permissões do navegador e por que são necessárias

| Permissão                                                         | Uso                                                                                                                                                  |
|-------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------|
| `storage`                                                         | Guardar os resultados, o histórico e as preferências no seu navegador.                                                                               |
| `unlimitedStorage`                                                | Contas com milhares de perfis e as miniaturas de foto podem passar do limite padrão de armazenamento local. Os dados continuam só no seu computador. |
| `alarms`                                                          | Agendar as verificações do monitoramento (opcional) e esperar automaticamente quando o Instagram pede uma pausa.                                     |
| `notifications`                                                   | Avisar quando alguém deixar de te seguir ou quando uma verificação não puder ser concluída.                                                          |
| Acesso a `https://www.instagram.com/*`                            | Executar a extensão somente no Instagram, para ler as listas com a sua sessão e mostrar o painel lateral.                                            |
| Acesso a `https://*.cdninstagram.com/*` e `https://*.fbcdn.net/*` | Baixar as fotos de perfil exibidas no relatório.                                                                                                     |

A extensão não pede acesso a nenhum outro site, ao seu histórico, aos seus favoritos, aos seus downloads ou às suas abas em geral.

## 11. Cookies e sessão do Instagram

A extensão **não cria cookies** e não usa cookies de rastreamento. Para que as consultas funcionem, o próprio navegador envia ao Instagram os cookies da sessão que você já tem aberta, exatamente como acontece quando você usa o site.

A extensão lê apenas dois valores que o Instagram deixa visíveis para a página: o identificador numérico da sua conta (`ds_user_id`), para saber de qual conta são as listas, e o código de proteção do site (`csrftoken`), que é reenviado somente ao próprio Instagram junto com as consultas, como o site faz. Esses valores **não são guardados nem enviados a nenhum outro lugar**. O cookie de login (`sessionid`) é protegido pelo navegador e não pode ser lido pela extensão.

## 12. Segurança e proteção da sua conta

### Proteção dos seus dados

- Sem servidor próprio: não existe um banco de dados que possa vazar ou ser invadido.
- Os dados ficam no armazenamento isolado da extensão, protegido pelo próprio navegador.
- O código não carrega scripts de terceiros nem bibliotecas externas.
- Os textos vindos do Instagram são tratados antes de aparecer na tela, para impedir a execução de código malicioso.

### Proteção da sua conta do Instagram

Ações em massa, como deixar de seguir muitos perfis de uma vez, são o que mais leva o Instagram a bloquear contas. Por isso a extensão:

- é **somente leitura**: não segue, não deixa de seguir, não curte, não comenta e não envia mensagens;
- faz as consultas em **ritmo de pessoa**: intervalo aleatório de 2,5 a 6 segundos entre consultas e pausa de 25 a 50 segundos a cada 12 consultas;
- respeita um **limite de 200 consultas por hora** e espera sozinha se chegar a ele;
- **para imediatamente** se o Instagram pedir uma pausa, salva o progresso e bloqueia novas consultas por 2 horas;
- para e avisa o usuário se o Instagram pedir uma verificação de segurança;
- permite no máximo uma verificação por vez, mesmo com várias abas abertas;
- no monitoramento, verifica no máximo a cada 6 horas (24 horas para contas com mais de 3.000 seguidores), com horário levemente variado.

Mesmo com esses cuidados, os termos do Instagram não autorizam expressamente ferramentas de terceiros que façam leituras automáticas. Por isso a extensão oferece também o modo “exportação oficial” (seção 13), que não faz nenhuma consulta ao Instagram.

## 13. Modo “exportação oficial”

O Instagram permite que você baixe um arquivo com as suas listas de seguidores e seguindo. Nesse modo, você escolhe o arquivo (`.zip` ou `.json`) no seu computador e a extensão o lê **somente na memória da página**, sem fazer nenhuma consulta ao Instagram. O conteúdo do arquivo **não é guardado**: ele é descartado ao fechar ou recarregar a página. A extensão lê apenas os arquivos de seguidores e de seguindo e ignora todo o resto do arquivo exportado.

## 14. Arquivos que você gera (CSV, PDF, área de transferência)

Quando você clica em “Baixar CSV”, “Imprimir / PDF” ou “Copiar @usuários”, o arquivo ou o texto é gerado no seu computador e salvo onde você escolher, ou copiado para a sua área de transferência. A partir daí, esse arquivo fica sob a sua responsabilidade. A extensão não envia esses arquivos para lugar nenhum e não lê a sua área de transferência.

## 15. Seus direitos e como apagar os dados

Como todos os dados ficam apenas no seu navegador, você tem controle total sobre eles:

- **Ver os dados:** tudo o que a extensão guarda aparece no popup, no painel e na página de relatório.
- **Exportar:** use “Baixar CSV” na lista ou no histórico.
- **Parar a coleta:** desligue o monitoramento a qualquer momento; nenhuma verificação é feita sem que você peça ou ative o monitoramento.
- **Apagar tudo:** remova a extensão em `chrome://extensions` → “Remover”. O navegador apaga imediata e definitivamente todos os dados da extensão.

Os direitos previstos no art. 18 da LGPD (confirmação, acesso, correção, eliminação, portabilidade e informação sobre compartilhamento) podem ser exercidos diretamente por você pelos meios acima, já que o desenvolvedor não possui nenhuma cópia dos seus dados. Em caso de dúvida, use o canal de [contato](#20-contato).

Sobre os dados de terceiros (nomes e @usuários dos perfis das suas listas): eles são informações que o próprio Instagram já mostra a você nas suas listas. A extensão apenas os organiza no seu navegador, para o seu uso pessoal, e nunca os publica ou compartilha.

## 16. Crianças e adolescentes

A extensão não é direcionada a crianças. O uso do Instagram segue a idade mínima definida pelo próprio Instagram (13 anos). A extensão não coleta nenhum dado para o desenvolvedor, de nenhuma faixa etária.

## 17. Conformidade com a Chrome Web Store

O uso de informações recebidas pela extensão segue a <a href="https://developer.chrome.com/docs/webstore/program-policies/user-data-faq" rel="noopener">Política de Dados do Usuário da Chrome Web Store</a>, incluindo os requisitos de **Uso Limitado** (*Limited Use*). Em especial:

- os dados são usados somente para oferecer e melhorar a única finalidade da extensão, que é visível para o usuário;
- os dados não são transferidos a terceiros;
- os dados não são usados para publicidade, incluindo publicidade personalizada;
- os dados não são usados para determinar crédito ou para fins de empréstimo;
- nenhuma pessoa lê os dados do usuário.

## 18. Relação com o Instagram e a Meta

A extensão é um projeto independente e **não tem vínculo** com o Instagram nem com a Meta Platforms, Inc., que não a endossam nem a patrocinam. Instagram é marca registrada da Meta Platforms, Inc. O seu uso do Instagram continua sujeito aos Termos de Uso e à Política de Privacidade do Instagram.

## 19. Alterações nesta política

Se a extensão passar a usar os dados de outra forma, esta política será atualizada **antes** da mudança entrar em vigor, com nova data no topo da página. Mudanças relevantes também serão informadas na página da extensão na Chrome Web Store. O histórico completo de alterações desta página pode ser consultado no repositório público onde ela está hospedada.

## 20. Contato

Dúvidas, pedidos ou relatos de problemas de privacidade podem ser enviados pelo canal público de suporte da extensão no GitHub:  
<a href="https://github.com/morenoksksks-ctrl/quem-nao-me-segue/issues" rel="noopener">github.com/morenoksksks-ctrl/quem-nao-me-segue/issues</a>

Ao abrir um pedido, não inclua senhas nem dados pessoais. Nunca pediremos a sua senha do Instagram.

Quem Não Me Segue · Política de Privacidade · Última atualização: 25 de novembro de 2026
