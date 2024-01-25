# Pontos considerados

Todos os pontos e observações presentes aqui foram discutidas dentro do [Escolhendo uma hospedagem](../escolhendo-uma-hospedagem/), recomenda-se que leia está página antes de prosseguir.

Esses pontos são apenas para ver a superfície da hospedagem e sumarizar tudo, caso vá escolher alguma, leia todos com calma e veja você mesmo cada opção de hospedagem.

Caso qualquer ponto esteja incorreto favor não hesite em entrar em contato, caso acredita que algum ponto observado deva ser retirado/modificado ou adicionar outro ponto sinta-se livre para sugerir.

## Localização

Aqui será considerado a localização em que a hospedagem atua, sendo considerado os países (Brasil, Estados Unidos, Canadá, etc.), juntamente com qual cidade está localizado (São Paulo, Miami, Montreal, etc.)\
Não existe ponto negativo ou positivo nessa classificação, apenas será considerada incompleta se não especificar a cidade.

## Legalidade

Se a emprese está registrada corretamente com um CNPJ e com o CNAE de atuação correto (CNAE 6311-9/00).\
[Mais informações nessa página](../escolhendo-uma-hospedagem/legais.md).

## Sistema Financeiro

Muitas empresas utilizam algo [WHMCS](https://www.whmcs.com/), um sistema para gerenciar os planos e alocação dos serviços, assim como tem integrações com os métodos de pagamento (Cartão de crédito, Boleto, Paypal, Mercado Pago, etc.).\
É [possível verificar se a empresa está crackeando (Também chamado de "Nulled") esse software](https://www.whmcs.com/members/verifydomain.php/verifydomain.php), que, se caso estiver, poderá significar uma falha de segurança grave, com informações sendo coletadas ilegalmente e com patches de segurança podendo não ser aplicados

Claro, WHMCS não é o único que existe, pode ser Hostbill, PteroBill ou até um sistema próprio.

## Avaliação

Caso a empresa tenha algum local público para avaliação (Discords não são considerados), como, por exemplo, TrustPilot ou ReclameAqui, e que ele esteja citado no website e verificado pela empresa.

## Uptime e SLA

Quanto tempo num ciclo de pagamento o servidor deverá estar online, normalmente sendo uma média de 99%+ e quanto será recompensado, descrito dentro dos termos de serviço.

## Hardware

Será considerado o hardware em que o servidor estará hospedado, sendo os seguintes pontos:

* Processador: Qual a performance do processador considerando o single core em testes sintéticos (Passmark), esse é o número que está depois do processador na lista, procuramos uma performance mínima de 2500 pontos em single core, estará sendo considerado a performance máximos que o processador conseguirá entregar em single core, sem ser a performance que poderá estar sendo recebida dentro da hospedagem.

## Proteção DDoS

Qual proteção está sendo relatada, apenas será considerada caso o provedor esteja publicamente disponível (Ex, Path.net, Cloudflare Magic Transit, TCPShield). Apenas será considerada totalmente caso houver o provedor citado e que esteja consistente a informação sobre.

## Backups off-site

Os backups serem hospedados fora do datacenter em que o servidor está.\
Segurança em casos de falha na máquina ou falha no datacenter por completo.

Caso não esteja citado de nenhum modo, será considerado que o backup é on-site (Na mesma máquina).

## Compartilhamento de recursos

Será considerado se os recursos comprados serão totalmente dedicados ou se serão compartilhados com outros clientes, podendo cair na consideração de overselling.\
Caso tenha algum plano com recursos dedicados citados, já cumprirá essa observação, nem todos os planos precisam bater esse requisito.

## Práticas insustentáveis

Práticas consideradas insustentáveis são as práticas que não funcionarão ao longo termo e/ou que são maleficiais ao cliente, e recomendadas de evitar qualquer empresa que faça as mesmas:

* Planos vitalícios: Planos que só se paga uma vez e nunca mais.
* Planos ilimitados: Planos que relatam qualquer recurso como ilimitado
* Fração de recursos e valores inconsistentes: Caso a fração não seja linear dos recursos e valores em diferentes planos, o que poderá arrecadar em overselling ou recursos não utilizados da máquina

## Transparência

Será considerado o quão transparente a empresa é para o público:

* Página de uptime: Página publicamente com histórico de uptime de todos os nodes e serviços oferecidos.
* Página de recursos: Página com utilização de todos os recursos de todos os nodes e serviços oferecidos, normalmente com a página de uptime.
* Transparência de produtos: Transparência sobre os recursos que terá em cada produto e serviço oferecido.

## Recursos adicionais

Recursos adicionais que poderão se úteis para muitos incluídos no painel, ou não, da hospedagem, como:

* Instalador de versões
* Instalador de modpacks
* Instalador de plugins
* Server Splitter

Recursos considerados comuns não serão considerados, como, por exemplo:

* Acesso FTP
* Banco de dados MySQL
* Gerenciamento de sub usuários

## Template para comparação:

<table><thead><tr><th width="208">Ponto observado</th><th width="240">Informações</th><th>Anotações</th></tr></thead><tbody><tr><td>Localização</td><td>País - Cidade</td><td></td></tr><tr><td>Legalidade</td><td>CNPJ/MEI</td><td></td></tr><tr><td>Sistema Financeiro</td><td>WHMCS Crackeado/HostBill/Próprio</td><td></td></tr><tr><td>Avaliação</td><td>TrustPilot/ReclameAqui</td><td></td></tr><tr><td>Uptime SLA</td><td>SLA - Compensação</td><td></td></tr><tr><td>Hardware</td><td>CPU Modelo</td><td></td></tr><tr><td>Proteção DDoS</td><td>Capacidade</td><td>Provido por X</td></tr><tr><td>Backups on/off-site</td><td>on-site/off-site</td><td></td></tr><tr><td>Compartilhamento de recursos</td><td>Compartilhados/Dedicados</td><td></td></tr><tr><td>Práticas insustentáveis</td><td>- Planos vitalícios<br>- Planos ilimitados<br>- Fração inconsistente</td><td></td></tr><tr><td>Transparência</td><td>- Página de uptime<br>- Página de recursos<br>- Produtos/serviços</td><td></td></tr><tr><td>Adicionais</td><td>- Instalador de versões<br>- Instalador de modpacks<br>- Instalador de mods<br>- Instalador de plugins<br>- Server Splitter</td><td></td></tr></tbody></table>

