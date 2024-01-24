# Misc

### Misc

#### Arquivo: [spigot.yml](https://www.spigotmc.org/wiki/spigot-configuration/)

**Configuração: merge-radius**

```
Bons valores iniciais:

      item: 3.5
      exp: 4.0
```

Isso decide a distância entre os itens e exp orbs a serem mesclados, reduzindo a quantidade de itens processado no chão. Definir isso muito alto levará à ilusão de itens ou orbes de exp desaparecendo conforme eles se fundem. Definir isso muito alto quebrará algumas farms, além de permitir que os itens se teletransportem através de blocos. Não há verificações feitas para impedir que os itens se fundam através das paredes. Exp só é mesclado na criação.

**Configuração: hopper-transfer**

`Bom valor inicial: 8`

Tempo em ticks que os funis esperarão para mover um item. Aumentar isso ajudará a melhorar o desempenho se houver muitos hoppers em seu servidor, mas interromperá os relógios baseados em hopper e possivelmente os sistemas de classificação de itens se estiver muito alto.

**Configuração: hopper-check**

`Bom valor inicial: 8`

Tempo em ticks entre funis verificando um item acima deles ou no inventário acima deles. Aumentar isso ajudará no desempenho se houver muitos funis em seu servidor, mas interromperá os relógios baseados em funis e os sistemas de classificação de itens que dependem de fluxos de água.

#### Arquivo: [paper-world configuration](https://docs.papermc.io/paper/reference/world-configuration)

**Configuração: alt-item-despawn-rate**

```
Bons valores iniciais:

      enabled: true
      items:
        cobblestone: 300
        netherrack: 300
        sand: 300
        red_sand: 300
        gravel: 300
        dirt: 300
        grass: 300
        pumpkin: 300
        melon_slice: 300
        kelp: 300
        bamboo: 300
        sugar_cane: 300
        twisting_vines: 300
        weeping_vines: 300
        oak_leaves: 300
        spruce_leaves: 300
        birch_leaves: 300
        jungle_leaves: 300
        acacia_leaves: 300
        dark_oak_leaves: 300
        mangrove_leaves: 300
        cactus: 300
        diorite: 300
        granite: 300
        andesite: 300
        scaffolding: 600
```

Esta lista permite que você defina um tempo alternativo (em ticks) para remover certos tipos de itens descartados mais rápido ou mais lento que o padrão. Esta opção pode ser usada em vez de plugins de limpeza de itens junto com o <mark style="color:yellow;">`merge-radius`</mark> para melhorar o desempenho.

**Configuração: redstone-implementation**

`Bom valor inicial: ALTERNATE_CURRENT`

Substitui o sistema redstone por versões mais rápidas e alternativas que reduzem as atualizações de blocos redundantes, diminuindo a quantidade de lógica que seu servidor precisa calcular. O uso de uma implementação não vanilla pode apresentar pequenas inconsistências com redstone muito técnico, mas os ganhos de desempenho superam em muito os possíveis problemas de nicho. Uma opção de implementação não vanilla também pode corrigir outras inconsistências de redstone causadas pelo CraftBukkit.\
\
A implementação <mark style="color:yellow;">`ALTERNATE_CURRENT`</mark> é baseada no mod [Alternate Current](https://modrinth.com/mod/alternate-current). Mais informações sobre esse algoritmo podem ser encontradas em sua página de recursos.

**Configuração: hopper.disable-move-event**

`Bom valor inicial: false`

<mark style="color:yellow;">`InventoryMoveItemEvent`</mark> não dispara a menos que haja um plug-in escutando ativamente esse evento. Isso significa que você só deve definir isso como verdadeiro se tiver esse(s) plug-in(s) e não se importar com o fato de eles não serem capazes de agir nesse evento. **Não defina como true se quiser usar plugins que escutam esse evento, por exemplo plugins de proteção!**

**Configuração: hopper.ignore-occluding-blocks**

`Bom valor inicial: true`

Determina se os funis irão ignorar contêineres dentro de blocos completos, por exemplo, funil minecart dentro de areia ou bloco de cascalho. Manter isso ativado interromperá algumas engenhocas, dependendo desse comportamento.

**Configuração: tick-rates.mob-spawner**

`Bom valor inicial: 2`

Esta opção permite configurar com que frequência os geradores devem ser processadores. Valores mais altos significam menos lag se você tiver muitos spawners, embora se definido muito alto (em relação ao atraso de seus spawners), as taxas de spawn de mob diminuirão.

**Configuração: optimize-explosions**

`Bom valor inicial: true`

Definir isso como <mark style="color:yellow;">`true`</mark> substitui o algoritmo de explosão vanilla por um mais rápido, com um custo de pequena imprecisão ao calcular o dano da explosão. Isso geralmente não é perceptível.

**Configuração: treasure-maps.enabled**

`Bom valor inicial: false`

A geração de mapas do tesouro é extremamente cara e pode travar um servidor se a estrutura que ele está tentando localizar estiver em uma chunk não gerado. Só é seguro habilitar isso se você pré-gerou seu mundo e definiu uma borda de mundo vanilla.

**Configuração: treasure-maps.find-already-discovered**

```
Bons valores iniciais:
      loot-tables: true
      villager-trade: true
```

O valor padrão desta opção força os mapas recém-gerados a procurar estruturas inexploradas, que geralmente estão em blocos ainda não gerados. Definir isso como <mark style="color:yellow;">`true`</mark> faz com que os mapas possam levar às estruturas que foram descobertas anteriormente. Se você não mudar isso para <mark style="color:yellow;">`true`</mark>, você pode ter problemas com o servidor travando ou travando ao gerar novos mapas do tesouro. <mark style="color:yellow;">`villager-trade`</mark> é para mapas negociados por aldeões e <mark style="color:yellow;">`loot-tables`</mark> refere-se a qualquer coisa que gere loot dinamicamente, como baús de tesouro, baús de masmorras, etc.

**Configuração: tick-rates.grass-spread**

`Bom valor inicial: 4`

Tempo em ticks entre o servidor tentando espalhar grama ou micélio. Isso fará com que grandes áreas de terra demorem um pouco mais para se transformar em grama ou micélio. Definir isso para cerca de <mark style="color:yellow;">`4`</mark> deve funcionar bem se você quiser diminuí-lo sem que a taxa de propagação diminuída seja perceptível.

**Configuração: tick-rates.container-update**

`Bom valor inicial: 1`

Tempo em ticks entre as atualizações do contêiner. Aumentar isso pode ajudar se as atualizações de contêiner causarem problemas para você (isso raramente acontece), mas torna mais fácil para os jogadores experimentarem a dessincronização ao interagir com inventários (itens fantasmas).

**Configuração: non-player-arrow-despawn-rate**

`Bom valor inicial: 20`

Tempo em ticks após o qual as flechas disparadas por mobs devem desaparecer após atingir algo. Os jogadores não podem pegá-los de qualquer maneira, então você também pode definir isso para algo como <mark style="color:yellow;">`20`</mark> (1 segundo).

**Configuração: creative-arrow-despawn-rate**

`Bom valor inicial: 20`

Time in ticks after which arrows shot by players in creative mode should disappear after hitting something. Players can't pick these up anyway, so you may as well set this to something like `20` (1 second).

**Configuração: nether-ceiling-void-damage-height**

`Bom valor inicial: 127`

Se esta opção for maior que <mark style="color:yellow;">`0`</mark>, os jogadores acima do nível definido y serão danificados como se estivessem no vazio. Isso impedirá que os jogadores usem o teto do nether. Vanilla nether tem 128 blocos de altura, então você provavelmente deve configurá-lo para <mark style="color:yellow;">`127`</mark>. Se você modificar a altura do nether de alguma forma, você deve definir isso como <mark style="color:yellow;">`[sua_altura_do_nether] - 1`</mark>.

#### Arquivo: [pufferfish.yml](https://docs.pufferfish.host/setup/pufferfish-fork-configuration/)

**Configuração: disable-method-profiler**

`Bom valor inicial: true`

Esta opção desativará alguns perfis adicionais feitos pelo jogo. Essa criação de perfil não é necessária para ser executada na produção e pode causar lag adicional.

#### Arquivo: [purpur.yml](https://purpurmc.org/docs/Configuration/)

**Configuração: dolphin.disable-treasure-searching**

`Good starting value: true`

Impede que os golfinhos realizem buscas de estruturas semelhantes aos mapas do tesouro.

**Configuração: teleport-if-outside-border**

`Good starting value: true`

Permite que você teletransporte o jogador para o spawn do mundo se ele estiver fora da fronteira do mundo. Útil, pois a fronteira do mundo vanilla pode ser contornada e o dano que causa ao jogador pode ser mitigado.
