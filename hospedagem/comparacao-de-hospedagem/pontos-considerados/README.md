# Pontos considerados

Todas as observações presentes aqui foram discutidas dentro do [Escolhendo uma hospedagem](../../escolhendo-uma-hospedagem/).

Essas observações <mark style="color:red;">não são feitos para determinar a qualidade uma hospedagem</mark>, apenas a sua <mark style="color:green;">transparência, legalidade e consistência de informações de maneira</mark> <mark style="color:green;"></mark><mark style="color:green;">**superficial**</mark>. A decisão da hospedagem para o seu servidor não deve ser feita apenas a partir dessa documentação, pesquise por conta própria e chegue as suas conclusões.

Caso qualquer observação esteja incorreta, favor não hesite de entrar em contato.

## Todos os pontos considerados

### Localização

A localização em que a hospedagem atua, sendo considerado os países (Brasil, Estados Unidos, Canadá, etc.), juntamente com qual cidade está localizado (São Paulo, Miami, Montreal, etc.)\
Não existe ponto negativo ou positivo nessa classificação, apenas será considerada incompleta se não especificar a localização exata (Ex. apenas ter o país, ao invés da cidade).

### Legalidade

Se a emprese está registrada corretamente com um CNPJ e com o CNAE de atuação correto (CNAE 6311-9/00).\
[Mais informações nessa página](../../escolhendo-uma-hospedagem/legais.md).

### Sistema Financeiro

Um sistema para gerenciar os planos e alocação dos serviços, assim com integrações para os métodos de pagamento (Cartão de crédito, Boleto, Paypal, Mercado Pago, etc.).\
O software mais comum para esse próprio é o WHMCS, é possível [verificar se a empresa está autorizada a utilizar esse software](https://www.whmcs.com/members/verifydomain.php/verifydomain.php), muitas vezes, se não estiver, é resultado de algum crack, o que poderá significar uma falha de segurança grave, com informações sendo coletadas ilegalmente e com patches de segurança podendo não ser aplicados

Claro, WHMCS não é o único que existe, pode ser Hostbill, PteroBill ou até um sistema próprio.

### Avaliação

Caso a empresa tenha algum local público para avaliação (Discords não são considerados), como, por exemplo, TrustPilot ou ReclameAqui, e que ele esteja citado no website e verificado pela empresa.

### Uptime e SLA

Quanto tempo num ciclo de pagamento o servidor deverá estar online, normalmente sendo uma média de 99.5%+ e quanto será recompensado, descrito dentro dos termos de serviço.

Caso o Uptime e SLA seja abaixo de 99.5%, ou não esteja citado nos termos, ele será considerado incompleto.

### Hardware

Será considerado o hardware em que o servidor estará hospedado, sendo os seguintes pontos:

* Processador: Qual a performance do processador considerando o single core em testes sintéticos (Passmark), esse é o número que está depois do processador na lista, procuramos uma performance mínima de 2500 pontos em single core, estará sendo considerado a performance máxima que o processador conseguirá entregar em um núcleo, sem ser a performance que poderá estar sendo recebida dentro da hospedagem (Devido a divisão de recursos e alocação).
* Armazenamento: Como não é possível fazer um teste de performance do armazenamento ou verificar as informções, caso a empresa cite que utiliza HDD ou não utilize SSD, será considerado como incompleto essa observação.

### Rede

Será considerado dois pontos principais:

* Qual proteção DDoS está sendo relatada, apenas será considerada o provedor, e deve estar, publicamente disponível, como, por exemplo, Path.net, Cloudflare Magic Transit, TCPShield.
* Se a empresa possui ASN, isto é, se a empresa tem os seus próprios endereços IPs, apenas sendo considerado por motivos informacionais, não acarretando ranking ou pontuação.
* Qual a banda de rede da máquina/node dos servidores, apenas sendo meramente informacional, não acarretando ranking ou pontuação.

### Backups on-site ou off-site

Backups on-site significa que estão dentro da mesma máquina ou do mesmo datacenter em que estão os servidores dos clientes, um backup ser off-site significaria que os backups estão fora do datacenter em que os servidores estão, assim, tendo maior garantia caso dê problemas que afetarão o datacenter por completo.

Caso não esteja citado de nenhum modo, será considerado que o backup é on-site (Na mesma máquina).

### Compartilhamento de recursos

Se os recursos comprados serão totalmente dedicados ou se serão compartilhados com outros clientes, podendo cair na consideração de overselling.\
Caso tenha algum plano com recursos dedicados citados, já cumprirá essa observação, nem todos os planos precisam bater esse requisito.

Essa informação deverá ser pública, e totalmente clara, no website. Além de apenas ser considerada caso os planos de recursos dedicados estão tão facilmente disponíveis quanto os compartilhados.

### Práticas insustentáveis

Práticas consideradas insustentáveis são as práticas que não funcionarão ao longo termo e/ou que são maleficiais ao cliente, e recomendadas de evitar qualquer empresa que faça as mesmas:

* Planos vitalícios: Planos que só se paga uma vez e nunca mais.
* Planos ilimitados: Planos que relatam qualquer recurso como ilimitado, mais comum entre "RAM Ilimitada", porém, processador ou armazenamento ilimitado também estará contando nessa categoria.
* Fração de recursos e valores inconsistentes: Caso a fração não seja linear dos recursos e valores em diferentes planos, o que poderá arrecadar em overselling ou recursos não utilizados da máquina, exemplo:
  * Um plano de 4GB de ram ter 200% de CPU e 8GB de disco, enquanto um plano de 8GB de ram ter 500% de CPU e 24GB de disco. \
    O plano de 8GB de ram, nesse caso, deveria ter 400% de CPU e 16GB de disco.
  * Um plano de 4GB de ram custar R$40, porém, um plano de 8GB de ram custar R$60.\
    O plano de 8GB de ram, nesse caso, deveria custar R$80

### Uptime e utilização

Será considerado se a empresa tem os seguintes recursos:

* Página de uptime: Página disponível publicamente com histórico de uptime de todos os nodes e serviços oferecidos.
* Página de recursos: Página com utilização de todos os recursos de todos os nodes e serviços oferecidos, normalmente com a página de uptime junto, alguns exemplos são:
  * [status.bloom.host](https://status.bloom.host)
  * [status.pebblehost.com](https://status.pebblehost.com)

### Recursos adicionais

Recursos adicionais que poderão se úteis para muitos incluídos no painel, ou não, da hospedagem, alguns exemplos:

* Instalador de versões
* Instalador de modpacks
* Instalador de plugins
* Server Splitter

Recursos básicos não serão considerados, como, por exemplo:

* Acesso SFTP
* Banco de dados MySQL
* Gerenciamento de sub usuários

## Sistema de pontuação

Com um sistema de pontuação é mais fácil de organizar em ordem as hospedagens, assim as que mais completam a lista ficam no topo, e as que menos no final.

Existem 3 classificações possíveis, porém, nem todas as observações podem ser classificadas como parciais:

* <mark style="color:green;">Verde</mark>: Cumpriu totalmente a observação&#x20;
* <mark style="color:orange;">Laranja</mark>: Cumpriu parcialmente a observação&#x20;
* <mark style="color:red;">Vermelho</mark>: Não cumpriu a observado

E os pontos referentes a cada observação:

<table><thead><tr><th width="208">Ponto observado</th><th width="240">Informações</th><th>Anotações</th></tr></thead><tbody><tr><td>Localização</td><td>País - Cidade</td><td>Não vale pontuação</td></tr><tr><td>Legalidade</td><td>CNPJ/MEI</td><td><mark style="color:red;">Sem Registro</mark> = 0 pontos<br><mark style="color:orange;">MEI</mark> = 15 pontos<br><mark style="color:green;">CNPJ</mark> = 30 pontos</td></tr><tr><td>Sistema Financeiro</td><td>WHMCS/HostBill/Próprio</td><td><mark style="color:red;">Crackeado/Não tem</mark> = 0 pontos<br><mark style="color:green;">Autorizado/Próprio</mark> = 20 pontos</td></tr><tr><td>Avaliação</td><td>TrustPilot/ReclameAqui</td><td><mark style="color:red;">Não existente/Não citado</mark> = 0 pontos<br><mark style="color:orange;">Citado mas não verificado</mark> = 5 pontos<br><mark style="color:green;">Citado e verificado</mark> = 10 pontos<br><br>O limite para essa observação é 10 pontos, e apenas um website de avaliação precisa existir.<br>Caso tenha mais do que um, será somado a pontuação e dividido pela quantidade de websites de avaliação presentes.</td></tr><tr><td>Uptime SLA</td><td>SLA - Compensação</td><td><mark style="color:red;">Não citado o SLA e/ou compensação</mark> = 0 pontos<br><mark style="color:orange;">SLA e compensação citada porém é abaixo de 99.5%</mark> = 5 pontos<br><mark style="color:green;">SLA e compensação citada e acima ou igual a 99.5%</mark> = 10 pontos</td></tr><tr><td>Hardware</td><td>CPU Modelo</td><td><mark style="color:red;">Processador a baixo de 2500 pontos no single core (Passmark) ou uso de HDD</mark> = 0 pontos<br><mark style="color:green;">Processador a cima de 2500 pontos no single core (Passmark)</mark> = 25 pontos<br><br>Caso tenha mais de um processador será somado a quantidade de pontos de todos os processador e dividido pela quantidade de processadores.</td></tr><tr><td>Rede</td><td>Proteção DDoS<br>ASN (Informacional)<br>Banda (Informacional)</td><td><mark style="color:red;">Citado/Não existente</mark> = 0 pontos<br><mark style="color:green;">Citado com provedor</mark> = 15 pontos<br><br>Caso tenha mais de uma camada de proteção citada na mesma localização e estar incompleto, será somado os pontos e divididos para calcular o total da localização.<br>Caso tenha mais de uma localização, será somado e dividido os pontos de cada localização pelo total de localizações.</td></tr><tr><td>Backups on/off-site</td><td>on-site/off-site</td><td><mark style="color:red;">On-site</mark> = 0 pontos<br><mark style="color:green;">Off-site</mark> = 10 pontos</td></tr><tr><td>Compartilhamento de recursos</td><td>Compartilhados/Dedicados</td><td><mark style="color:red;">Compartilhados</mark> = 0 pontos<br><mark style="color:green;">Dedicados</mark> = 10 pontos<br><br>Apenas um plano da hospedagem precisa ser dedicado para bater esse requisito, não todos.</td></tr><tr><td>Práticas insustentáveis</td><td>- Planos vitalícios<br>- Planos ilimitados<br>- Fração inconsistente</td><td>+10 pontos <mark style="color:green;">por cada prática não realizada</mark> (30 pontos totais)</td></tr><tr><td>Transparência</td><td>- Página de uptime<br>- Página de recursos</td><td>- <mark style="color:green;">Página de uptime</mark> = 5 pontos<br>- <mark style="color:green;">Página de recursos</mark> = 10 pontos</td></tr><tr><td>Adicionais</td><td>- Instalador de versões<br>- Instalador de modpacks<br>- Instalador de mods<br>- Instalador de plugins<br>- Server Splitter</td><td>- <mark style="color:green;">Server Splitter</mark> = 5 pontos<br>- <mark style="color:green;">Loja Inclusa</mark> = 5 pontos<br>- <mark style="color:green;">Backup de databases</mark> = 4 pontos<br>- <mark style="color:green;">Instalador de modpacks</mark> = 4 pontos<br>- <mark style="color:green;">Outros</mark> = 2 ponto<br><br>Caso a loja esteja inclusa, ela deverá ser de graça durante todo o período em que se pagar a hospedagem e deve estar citado o fornecedor.<br><br>Essa observação tem um limite de 35 pontos.</td></tr></tbody></table>

O total de pontos que uma empresa pode tirar é de **210.**

### **Conversão para uma nota de 0 a 10**

A pontuação será convertida em uma nota de 0 a 10 para ficar de mais fácil visualização, além de ser mais fácil caso for adicionado mais observações ou o peso de alguma for alterado.

É possível converter a pontuação para uma nota de 0 a 10 utilizando uma regra de 3, o cálculo ficaria desta forma:

`(<Pontuação>*10)/<Pontuação Máxima>=Nota`

Por exemplo, uma empresa conseguiu 160 pontos com o máximo de 190 pontos:

(`160*10)/190=Nota` -> `1600/190=Nota` -> **8.421**

Apenas será considerada a primeira casa decimal, nesse caso, se tornando **8.4**

### Informações não presentes publicamente

Caso alguma informação que esteja sendo avaliada não esteja presente publicamente (Website da empresa ou termos de serviço/privacidade) não será considerada na pontuação, mesmo que tenha sido encontrada mediante a contato com o suporte, porém, ainda serão adicionadas na comparação.

Por que isso? Pois visamos uma comunidade mais transparente, com empresas relatando exatamente o que receberemos pelo nosso dinheiro, sem ter que comprar algo para saber o que receberá, desde o processador, o limite dos recursos, a proteção e a localização.

{% content-ref url="modelo-de-comparacao.md" %}
[modelo-de-comparacao.md](modelo-de-comparacao.md)
{% endcontent-ref %}
