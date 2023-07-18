# Trabalho Prático 2 da disciplina Técnicas de Programação para Plataformas Emergentes

### Componentes:
- Álvaro Henrique de Sousa Gouvea 18/0012002
- Carla Rocha Cangussú 17/0085023
- Daniel Porto de Souza 18/0149687
- Hugo Rocha

O presente trabalho tem como objetivo destrinchar cinco das nove características de um bom projeto de software citadas por Fowler. As cinco características que serão detalhadas a seguir são, boa documentação, extensibilidade, ausência de duplicidade e modularidade 

## Boa documentação

Descrição da característica: Uma boa documentação de um projeto de software é essencial para o seu sucesso a longo prazo. Ela serve como um guia detalhado e compreensível sobre o funcionamento do software, facilitando o entendimento, manutenção, colaboração e expansão do projeto. A documentação deve ser pequena porque o projeto deve ser simples. Isto é, deve ser claro, organizado e objetivo. 

2. Efeitos no código:  
Estrutura:  A boa documentação promove uma estrutura mais organizada e bem definida do projeto. Isso ocorre porque a documentação geralmente inclui diagramas, fluxos de trabalho e uma descrição geral da arquitetura, ajudando a esclarecer como os diferentes componentes do sistema se encaixam.  
Ao apresentar uma visão geral da estrutura, a documentação facilita o entendimento dos relacionamentos entre módulos e partes do código, tornando mais fácil para os desenvolvedores navegarem pelo projeto e localizarem as informações relevantes.

Claridade:  A documentação clara garante que as funcionalidades, APIs e comportamentos do software sejam bem compreendidos. Isso evita ambiguidades e interpretações errôneas que podem levar a erros de implementação ou uso inadequado.

Coesão: A documentação adequada pode enfatizar a coesão dentro do projeto. Quando os componentes são bem documentados, seus propósitos e responsabilidades ficam mais claros. Isso encoraja os desenvolvedores a seguir o princípio de "alta coesão", onde cada módulo possui uma função específica e bem definida, reduzindo assim o acoplamento entre diferentes partes do código.  
A coesão aprimorada geralmente resulta em um código mais organizado e mais fácil de manter, pois as responsabilidades são distribuídas de forma mais eficiente.

Acoplamento: A documentação pode afetar o acoplamento, que é o grau de dependência entre as partes do software. Quanto mais clara e detalhada a documentação, mais fácil é entender como diferentes módulos interagem entre si.  
Ao compreender os pontos de acoplamento, os desenvolvedores podem tomar decisões mais informadas para reduzir o acoplamento indesejado e promover um design mais flexível e modular.  
Além disso, a documentação que explica os requisitos de interface e os contratos entre módulos ajuda a evitar problemas de compatibilidade e alterações incompatíveis que podem surgir devido a mudanças não documentadas.

3. Relação com mau cheiros definidos por Fowler: uma boa documentação atua como uma aliada no processo de identificação, prevenção e correção de maus cheiros de código. Os maus cheiros de código são sintomas de problemas potenciais no design e implementação do software, indicando a necessidade de refatoração.   
Pode-se observar que quando a documentação é insuficiente ou programadores tendem  a preencher a lacuna escrevendo comentários em excesso no código para explicar partes complexas ou obscuras. Esses comentários podem se tornar rapidamente obsoletos e não refletir mais o código atual, resultando em informações incorretas. Uma boa documentação fornece explicações claras e detalhadas, reduzindo a necessidade de comentários excessivos e melhorando a compreensão geral do código.  
Outro problema que pode ser gerado pela falta de uma boa documentação é criação de métodos ou classes muito complexas, uma vez que não há uma  visão clara dos objetivos de uma classe/método. Com uma boa documentação é fácil identificar métodos ou classes excessivamente complexas, e assim os desenvolvedores podem simplificar a lógica, dividir tarefas complexas em etapas mais simples e, assim, melhorar a legibilidade do código.  

4. Exemplo de operação de refatoração capaz de levar o projeto de código é ter uma boa documentação é a ”Extração de Método". Essa técnica envolve a criação de um novo método a partir de um trecho de código existente, agrupando a lógica relacionada em uma única função com um nome significativo. Isso não apenas torna o código mais claro e legível, mas também pode ter um impacto positivo na qualidade da documentação do projeto.   
A extração de método torna mais fácil para outros desenvolvedores entenderem o propósito e o funcionamento da função, melhorando a colaboração no projeto e ajudando na manutenção futura. Além disso, ao usar bons nomes de métodos e argumentos, a documentação fica mais legível, facilitando a compreensão do código e evitando a necessidade de comentários excessivos.

## Extensibilidade

1. Descrição da característica: A extensibilidade é uma característica de um sistema de software que permite que ele seja facilmente estendido ou adaptado para incluir novas funcionalidades ou se ajustar a mudanças futuras. Em termos de estrutura, a extensibilidade geralmente envolve a criação de componentes modulares e de baixo acoplamento, permitindo que as partes do sistema sejam modificadas ou estendidas independentemente umas das outras.

2. Efeitos no código:  
Estrutura: A extensibilidade geralmente resulta em uma estrutura modular, onde as funcionalidades são organizadas em componentes independentes e reutilizáveis. Isso facilita a compreensão e a manutenção do código.

Claridade: Componentes extensíveis são projetados para serem facilmente compreensíveis e modificáveis. Isso envolve o uso de nomes descritivos,	separação clara de responsabilidades e um design limpo.

Coesão: A extensibilidade tende a promover a alta coesão, onde cada componente é responsável por uma única tarefa ou conjunto de tarefas relacionadas. Isso melhora a modularidade e facilita a manutenção do código.

Acoplamento: A extensibilidade busca reduzir o acoplamento entre os componentes, permitindo que eles sejam estendidos ou substituídos sem afetar outras partes do sistema. Isso resulta em um código mais flexível e menos propenso a efeitos colaterais indesejados.


3. Relação com os "maus-cheiros de código" de Fowler: Os "maus-cheiros de código" são padrões ou práticas de programação que indicam a presença de problemas ou deficiências no código-fonte. A extensibilidade pode ajudar a mitigar ou evitar muitos desses maus-cheiros, pois um código extensível e projetado com foco na manutenção e em evitar  armadilhas comuns.  
Por exemplo, um mau-cheiro comum e a "Classe Deus" (God Class), que é uma classe que realiza muitas tarefas diferentes e tem muitas responsabilidades. A extensibilidade pode ser usada para dividir essa classe em componentes menores e mais focados, melhorando a coesão e tornando o código mais modular e fácil de entender.

4. Operação de refatoração para alcançar a extensibilidade: Lima operação de refatoração que pode ajudar a tornar um projeto de código mais extensível e a "Extração de Método" (Extract Method). Essa operação envolve a identificação de blocos de código repetitivos ou lógica complexa e a extração desses trechos em métodos separados e reutilizados.  
Ao extrair métodos, você pode criar componentes independentes que podem ser estendidos ou substituídos individualmente, melhorando a extensibilidade geral do código. Além disso, a extração de métodos pode melhorar a clareza e coesão do código, tornando-o mais legível e fácil de manter.

## Ausência de duplicidade no código

1. Descrição da característica: A ausência de duplicidade e um princípio de design de código que visa eliminar a repetição de lógica ou código idêntico ou semelhante. Quando há duplicidade, qualquer alteração ou correção precisa ser feita em vários lugares, o que aumenta a complexidade e o risco de introduzir erros.

2. Efeitos no código:  
Estrutura: A ausência de duplicidade geralmente resulta em um código mais estruturado, onde a lógica e organizada de forma clara e consistente. O código é dividido em partes reutilizáveis e independentes, facilitando sua compreensão e manutenção.

Claridade: Eliminar a duplicidade torna o código mais legível e compreensível, pois não há repetição desnecessária de trechos de código. Isso facilita a identificação e o entendimento da funcionalidade específica implementada.

Coesão: Ao remover a duplicidade, a coesão do código é aprimorada. As responsabilidades são atribuídas de forma clara e as partes do código se concentram em tarefas específicas. Isso torna o código mais modular e facilita a manutenção.

Acoplamento: A ausência de duplicidade pode ajudar a reduzir o acoplamento entre as partes do código. Quando o mesmo trecho de código é usado em vários lugares, as alterações de um local podem afetar outros. Eliminando a duplicidade, e possível diminuir a dependência entre diferentes partes do sistema.


3. Relação com os "maus-cheiros de código" de Fowler: A duplicidade no código e frequentemente associada a maus­ cheiros de código identificados por Martin Fowler, coma "Duplicated Code" (Código Duplicado) e "Long Method" (Método Longo). Esses maus-cheiros indicam problemas potenciais de manutenção, clareza e flexibilidade no código.  
A duplicidade torna o código difícil de manter, pois qualquer alteração precisa ser feita em vários lugares. Além disso, a repetição desnecessária aumenta a complexidade e dificulta a compreensão da lógica do programa.

4. Operação de refatoração para alcançar a ausência de duplicidade: Uma operação de refatoração que pode ser aplicada para eliminar a duplicidade é a "Extract Method" (Extração de Método). Essa operação envolve identificar trechos de código duplicados e agrupá-los em um único método, que pode ser chamado de vários lugares onde o código duplicado estava presente.  
Ao extrair métodos e eliminar a duplicidade, o código se torna mais conciso, legível e fácil de manter. Além disso, a extração de método ajuda a melhorar a coesão e reduzir o acoplamento entre as partes do código.  
Outra operação de refatoração relacionada é a "Extract Class" (Extração de Classe), que envolve agrupar funcionalidades relacionadas em uma nova classe. Isso pode ajudar a eliminar a duplicidade ao centralizar a implementação de funcionalidades comuns em um único local. 

