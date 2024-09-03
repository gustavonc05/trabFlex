Neste README, você encontrará uma explicação detalhada de cada atributo do Flexbox. Para visualizar exemplos práticos de como esses atributos funcionam, abra o arquivo exemplos.html.


Display: flex
Descrição: Define um container flexível que organiza seus itens filhos (chamados de "flex items") em uma única linha ou coluna.
Características:
Itens filhos são dispostos em linha (por padrão) ou em coluna.
Itens podem crescer, encolher e se reorganizar de acordo com o espaço disponível, utilizando propriedades como justify-content, align-items, e flex-direction.
Ideal para layouts dinâmicos e responsivos.

Display: block
Descrição: Um elemento com display: block ocupa toda a largura disponível e começa em uma nova linha, forçando o próximo elemento a ser posicionado abaixo dele.
Características:
Ocupa 100% da largura do seu container pai, por padrão.
Respeita margens, preenchimento (padding) e bordas.

Display: inline
Descrição: Elementos com display: inline ocupam apenas o espaço necessário para o seu conteúdo, e não começam em uma nova linha.
Características:
Ocupa apenas a largura do conteúdo.
Outros elementos inline podem ser posicionados ao lado dele na mesma linha.
Não respeita largura (width) e altura (height).

Flex-direction: 
row: Alinha os itens ao longo do eixo horizontal, começando da esquerda para a direita. Este é o comportamento padrão de um container flexível.
row-reverse: Alinha os itens ao longo do eixo horizontal, mas na direção inversa, da direita para a esquerda.
column: Alinha os itens ao longo do eixo vertical, começando de cima para baixo.
column-reverse: Alinha os itens ao longo do eixo vertical, mas na direção inversa, de baixo para cima.

Flex-wrap:
nowrap: Os itens flexíveis são dispostos em uma única linha, sem permitir que eles quebrem para uma nova linha, mesmo que ultrapassem o limite do container. Este é o comportamento padrão.
wrap: Os itens flexíveis podem quebrar para uma nova linha se não houver espaço suficiente no container, com as linhas adicionais sendo posicionadas abaixo das anteriores.
wrap-reverse: Funciona como wrap, permitindo que os itens quebrem para novas linhas, mas as linhas adicionais são posicionadas acima das anteriores, invertendo a ordem vertical.

Flex-flow:
flex-flow: É uma propriedade abreviada no Flexbox que combina flex-direction e flex-wrap, permitindo definir a direção dos itens flexíveis e se eles devem quebrar para uma nova linha ou coluna.

Justify-content:
justify-content: Define o alinhamento dos itens flexíveis ao longo do eixo principal, controlando a distribuição do espaço entre eles.
flex-start: Alinha os itens ao início do eixo principal.
flex-end: Alinha os itens ao final do eixo principal.
center: Centraliza os itens ao longo do eixo principal.
space-between: Distribui os itens igualmente ao longo do eixo principal, com o primeiro item no início e o último item no final, e o espaço restante distribuído entre os itens.
space-around: Distribui os itens igualmente ao longo do eixo principal, com espaço igual ao redor de cada item (metade do espaço em cada extremidade).
space-evenly: Distribui os itens com espaços iguais entre eles e nas extremidades do container ao longo do eixo principal.
safe: Garantia de que o conteúdo se ajustará dentro da área visível, evitando que ele seja cortado ou sobreponha outros elementos. Usar safe assegura que qualquer ajuste no layout será feito de maneira a não prejudicar a visibilidade do conteúdo ou causar problemas de usabilidade.
unsafe: Permite que o conteúdo possa ser cortado ou sobrepor outros elementos se necessário. Usar unsafe pode resultar em partes do conteúdo se tornando invisíveis ou não acessíveis, mas pode permitir um layout mais flexível ou otimizado em certas situações.

Align-items:
align-items: Define o alinhamento dos itens flexíveis ao longo do eixo cruzado (perpendicular ao eixo principal), controlando como os itens são posicionados dentro do container flexível.
stretch: Expande os itens para preencher o container ao longo do eixo cruzado, ocupando toda a altura ou largura disponível.
flex-start: Alinha os itens ao início do eixo cruzado.
flex-end: Alinha os itens ao final do eixo cruzado.
center: Centraliza os itens ao longo do eixo cruzado.
baseline: Alinha os itens ao longo da linha de base do texto, alinhando as linhas de base dos itens, que é útil para alinhamento tipográfico.

Align-content:
align-content: Define o alinhamento das linhas de itens flexíveis dentro do container ao longo do eixo cruzado (perpendicular ao eixo principal), afetando o espaço entre as linhas.
flex-start: Alinha as linhas de itens ao início do eixo cruzado.
flex-end: Alinha as linhas de itens ao final do eixo cruzado.
center: Centraliza as linhas de itens ao longo do eixo cruzado.
space-between: Distribui as linhas de itens igualmente ao longo do eixo cruzado, com o espaço entre as linhas sendo uniforme e sem espaço extra nas extremidades.
space-around: Distribui as linhas de itens igualmente ao longo do eixo cruzado, com espaço igual ao redor de cada linha, incluindo espaço extra nas extremidades.

Gap:
gap: Define o espaço entre itens em um container flexível ou grid. Aplica um espaçamento uniforme entre todas as linhas e colunas dos itens.
row-gap: Define o espaço específico entre linhas de itens em um container flexível ou grid. Controla o espaçamento vertical entre as linhas.
column-gap: Define o espaço específico entre colunas de itens em um container flexível ou grid. Controla o espaçamento horizontal entre as colunas.

Order:
order: Controla a ordem de exibição dos itens flexíveis dentro de um container. Itens com valores de order menores aparecem antes dos itens com valores maiores. O valor padrão é 0, e itens com o mesmo valor de order são exibidos na ordem em que aparecem no código HTML.

Flex-grow:
flex-grow: Define a capacidade de um item flexível de crescer em relação aos outros itens dentro do container flexível. Um valor maior faz com que o item ocupe mais espaço disponível no container. Se todos os itens tiverem o mesmo valor de flex-grow, eles crescerão igualmente. O valor padrão é 0, o que significa que o item não crescerá além do seu tamanho inicial.

Flex-shrink:
flex-shrink: Define a capacidade de um item flexível de encolher quando há falta de espaço no container flexível. Um valor maior faz com que o item encolha mais em relação aos outros itens. Se todos os itens tiverem o mesmo valor de flex-shrink, eles encolherão igualmente. O valor padrão é 1, o que permite que o item encolha se necessário. Um valor de 0 indica que o item não encolherá.

Flex-basis:
flex-basis: Define o tamanho inicial de um item flexível antes de qualquer espaço adicional ser distribuído de acordo com flex-grow e flex-shrink. É o tamanho preferido do item ao longo do eixo principal antes que o espaço disponível seja ajustado. O valor pode ser uma largura ou altura específica, como pixels ou porcentagens, ou auto, que faz com que o tamanho inicial seja determinado pelo tamanho do conteúdo do item.

Align-self:
align-self: Permite que o alinhamento de um item flexível ao longo do eixo cruzado seja ajustado individualmente, sobrepondo o alinhamento definido pelo container com align-items.
auto: O item flexível usa o valor de alinhamento do container flexível, conforme definido por align-items.
flex-start: Alinha o item ao início do eixo cruzado.
flex-end: Alinha o item ao final do eixo cruzado.
center: Centraliza o item ao longo do eixo cruzado.
baseline: Alinha o item ao longo da linha de base do texto, alinhando as linhas de base dos itens.
stretch: Faz com que o item se estique para preencher o espaço disponível ao longo do eixo cruzado.
