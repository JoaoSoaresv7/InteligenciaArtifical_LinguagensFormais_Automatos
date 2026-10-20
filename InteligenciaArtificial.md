# Atividade: agentes inteligentes
Aula 19/10/2026 | Professora Kadidja Valéria | Inteligência artificial
Disciplina: Inteligência Artificial, Linguagens Formais e Autômatos
Estudante: João Vítor Soares Marinho   Turma: Engenharia de Software — Noturno
Resolva os exercícios 2.3, 2.4 e 2.5 do Capítulo 2 sobre agentes inteligentes. Examine a racionalidade, caracterize os ambientes de tarefa usando o modelo PEAS e apresente os conceitos com suas próprias palavras. Use o capítulo fornecido como base e fundamente suas respostas.
Forma de realização sugerida: individual e com consulta. Tempo estimado: 2h30. Prazo: conforme orientação da professora.
## Preparação e metas
Estude os conteúdos referentes à racionalidade, aos ambientes e à estrutura dos agentes. Consulte especialmente a Seção 2.3.2. Ao concluir, você deverá saber diferenciar função de agente e programa de agente, fundamentar as classificações dos ambientes e comparar as principais categorias de agentes.
## Exercício 2.3
Classifique cada afirmativa como verdadeira ou falsa e explique sua escolha com uma justificativa e um exemplo ou contraexemplo. Observe com cuidado as palavras “todo”, “nenhum”, “existe” e “nunca”.
a. Um agente que detecta apenas informações parciais sobre o estado não podem ser perfeitamente racionais.
b. Existem ambientes de tarefa nos quais nenhum agente reativo puro pode comportar-se racionalmente.
c. Existe um ambiente de tarefa em que todo agente é racional.
d. A entrada para o programa é a mesma que a entrada para a função de agente.
e. Toda função de agente é implementável por uma combinação de programa/máquina.
f. Suponha que um agente selecione sua ação uniformemente ao acaso do conjunto de ações possíveis. Existe um ambiente de tarefa determinista em que esse agente é racional.
g. É possível para um dado agente ser perfeitamente racional em dois ambientes de tarefa distintos.
h. Todo agente é racional em um ambiente não observável.
i. Um agente jogador de pôquer perfeitamente racional nunca perde.
Anote as respostas na página seguinte. Apenas marcar V ou F não é suficiente.

---

## Respostas do exercício 2.3
Apresente o conceito que fundamenta cada resposta e explique as condições consideradas no cenário. O contraexemplo precisa realmente demonstrar que a afirmação está incorreta. Aumente os espaços de resposta, se precisar.
a. Resposta: Falso. Justificativa: para ser racional, o agente não precisa observar todas as informações; sua decisão depende das percepções disponíveis.
Um aspirador que atua em dois quadrados e percebe apenas o local onde está pode ser racional usando a regra “sujo → aspirar; limpo → mudar”.
b. Resposta: Verdadeiro. Justificativa: um agente puramente reativo considera somente a percepção presente e não armazena informações anteriores.
No jogo da memória, encontrar os pares depende de recordar as cartas reveladas anteriormente.
c. Resposta: Verdadeiro. Justificativa: quando nenhuma ação muda a medida de desempenho, qualquer agente alcança o mesmo resultado máximo.
Por exemplo, um ambiente com apenas uma ação disponível ou no qual o desempenho permanece igual.
d. Resposta: Falso. Justificativa: a função do agente considera o histórico completo de percepções, enquanto o programa reativo recebe apenas a percepção atual.
No instante t: função f(p1…pt); programa reativo recebe apenas pt.
e. Resposta: Falso. Justificativa: existem funções que não podem ser computadas ou que demandariam memória ilimitada.
Um exemplo é a função que determina se uma máquina de Turing irá parar, questão conhecida como problema da parada.
f. Resposta: Verdadeiro. Justificativa: se todas as ações produzem o mesmo desempenho, selecioná-las aleatoriamente também pode ser uma escolha ótima.
Considere um ambiente determinístico no qual duas portas conduzem ao mesmo prêmio.
g. Resposta: Verdadeiro. Justificativa: a racionalidade depende do ambiente, e uma mesma ação pode ser a melhor opção em dois cenários diferentes.
Um aspirador reativo pode agir racionalmente em dois ambientes que diferem apenas pela condição inicial de limpeza.
h. Resposta: Falso. Justificativa: mesmo sem conseguir observar o ambiente, um agente pode escolher uma ação inferior a outra disponível.
Por exemplo, um aspirador sem sensores que permanece parado pode ter desempenho pior que outro que se desloca e limpa.
i. Resposta: Falso. Justificativa: ser racional significa buscar o melhor desempenho esperado, e não ter vitória garantida.
Uma jogada com 80% de chance de ganhar ainda pode resultar em derrota nos outros 20% dos casos.
### Revisão da argumentação
Confira se você conseguiu distinguir racionalidade de garantia de sucesso, percepção atual de histórico de percepções e função abstrata de implementação computacional.

---

## Exercício 2.4
Examine as sete atividades a seguir. Em cada situação, determine qual é o agente, defina as hipóteses, apresente o PEAS e classifique o ambiente. Copie o modelo de resposta sete vezes e amplie o documento.
1. Jogar futebol.
2. Explorar os oceanos subterrâneos de Titã.
3. Comprar livros usados de IA na Internet.
4. Jogar uma partida de tênis.
5. Praticar tênis contra uma parede.
6. Realizar um salto de altura.
7. Participar de um leilão de um item, realizando lances.
Trate a exploração de Titã como uma situação hipotética. No futebol, explicite se o agente é um jogador ou uma equipe. Use essa mesma definição do agente ao longo de toda a análise.
### Estrutura PEAS de cada atividade
P: critérios usados para medir o sucesso. E: ambiente, objetos e participantes envolvidos. A: recursos utilizados para executar ações. S: meios de captar informações e perceber o ambiente. Em software, inclua entradas e saídas digitais.
### Caracterização do ambiente
Observabilidade: Completamente observável, parcialmente observável ou não observável. Indique a classificação escolhida e explique o motivo.
Número de agentes: Agente único ou multiagente; indique cooperação ou competição quando pertinente. Indique a classificação escolhida e explique o motivo.
Previsibilidade: Determinístico ou estocástico; considere a influência estratégica de outros agentes. Indique a classificação escolhida e explique o motivo.
Dependência entre decisões: Episódico ou sequencial. Indique a classificação escolhida e explique o motivo.
Mudança durante a decisão: Estático, dinâmico ou semidinâmico. Indique a classificação escolhida e explique o motivo.
Natureza dos elementos: Discretos, contínuos ou combinação; considere estados, tempo, percepções e ações. Indique a classificação escolhida e explique o motivo.
Conhecimento do funcionamento: Conhecido ou desconhecido para o agente. Indique a classificação escolhida e explique o motivo.
Modelo: Propriedade: [nome] | Classificação: [escolha] | Justificativa: [uma ou duas frases]. Saber como o ambiente funciona não é o mesmo que conseguir observar todo o seu estado.
## Respostas do exercício 2.4
### Caso 1 — Jogar futebol
Atividade e agente considerado: Jogar futebol; agente: um jogador de linha (colegas e adversários fazem parte do ambiente).
Meta e hipóteses adotadas: Ajudar a equipe a vencer. Hipóteses: partida oficial 11×11, regras conhecidas.
- P — Critérios de desempenho: Gols marcados menos sofridos; passes certos; poucas faltas.
- E — Ambiente: Campo, bola, colegas, adversários, árbitro, relógio, placar.
- A — Atuadores: Pernas e pés (correr, chutar, passar), cabeça, voz e gestos.
- S — Sensores: Visão, audição, tato/propriocepção, placar e tempo.
### Caracterização do ambiente
- Propriedade: Observabilidade | Classificação: Parcialmente observável | Justificativa: o jogador não consegue enxergar todo o campo nem conhecer as intenções dos demais participantes.
- Propriedade: Número de agentes | Classificação: Multiagente (coopera com colegas, compete com adversários) | Justificativa: há diversos participantes, cada um com seus próprios objetivos.
- Propriedade: Previsibilidade | Classificação: Estocástico | Justificativa: o resultado sofre influência das ações imprevisíveis dos demais jogadores e do movimento da bola.
- Propriedade: Dependência entre decisões | Classificação: Sequencial | Justificativa: uma decisão interfere nas ações realizadas posteriormente.
- Propriedade: Mudança durante a decisão | Classificação: Dinâmico | Justificativa: a partida continua acontecendo enquanto o jogador escolhe o que fazer.
- Propriedade: Natureza dos elementos | Classificação: Combinação (predomina contínuo) | Justificativa: posições e tempo variam continuamente, enquanto o placar assume valores discretos.
- Propriedade: Conhecimento do funcionamento | Classificação: Conhecido | Justificativa: o jogador conhece as regras e o comportamento físico da bola.
### Caso 2 — Explorar os oceanos subterrâneos de Titã
Atividade e agente considerado: Explorar o oceano sob o gelo de Titã (hipotético); agente: robô submarino autônomo.
Meta e hipóteses adotadas: Mapear e coletar amostras. Hipóteses: comunicação com a Terra muito atrasada; sem outros agentes.
- P — Critérios de desempenho: Dados e amostras úteis, área mapeada, sobrevivência, energia, não contaminar.
- E — Ambiente: Oceano sob gelo, pressão, correntes, fundo, canal de comunicação.
- A — Atuadores: Propulsores, lastro, perfurador de gelo, braço coletor, transmissor.
- S — Sensores: Sonar, câmeras, sensores de pressão/temperatura/química, giroscópio.
### Caracterização do ambiente
- Propriedade: Observabilidade | Classificação: Parcialmente observável | Justificativa: os sensores alcançam áreas limitadas e há pouco conhecimento sobre o local.
- Propriedade: Número de agentes | Classificação: Agente único | Justificativa: correntes marítimas e gelo não possuem objetivos próprios.
- Propriedade: Previsibilidade | Classificação: Estocástico | Justificativa: correntes, formações de gelo e possíveis falhas deixam os resultados incertos.
- Propriedade: Dependência entre decisões | Classificação: Sequencial | Justificativa: o trajeto escolhido e o consumo de energia influenciam as etapas seguintes.
- Propriedade: Mudança durante a decisão | Classificação: Dinâmico | Justificativa: as correntes e as condições do gelo podem se alterar durante a tomada de decisão.
- Propriedade: Natureza dos elementos | Classificação: Contínuo | Justificativa: Posição, pressão e tempo contínuos.
- Propriedade: Conhecimento do funcionamento | Classificação: Desconhecido | Justificativa: ainda se conhece pouco sobre o oceano de Titã.
### Caso 3 — Comprar livros usados de IA na Internet
Atividade e agente considerado: Comprar livros usados de IA online; agente: software de compras.
Meta e hipóteses adotadas: Obter os títulos com menor custo. Hipóteses: lista e orçamento definidos, vários vendedores.
- P — Critérios de desempenho: Custo total (preço + frete), títulos obtidos, estado do livro, prazo.
- E — Ambiente: Lojas e marketplaces, vendedores, outros compradores, pagamento, entrega.
- A — Atuadores: Buscar, abrir páginas, adicionar ao carrinho, pagar, enviar mensagens.
- S — Sensores: Conteúdo das páginas (preço, fotos, avaliações), status do pedido, e-mails.
### Caracterização do ambiente
- Propriedade: Observabilidade | Classificação: Parcialmente observável | Justificativa: o agente não consegue confirmar diretamente o estoque disponível nem as condições reais do exemplar.
- Propriedade: Número de agentes | Classificação: Multiagente (competitivo) | Justificativa: outros compradores podem tentar adquirir os mesmos exemplares, especialmente quando há apenas uma unidade.
- Propriedade: Previsibilidade | Classificação: Estocástico | Justificativa: os preços e a disponibilidade podem mudar independentemente das ações do agente.
- Propriedade: Dependência entre decisões | Classificação: Sequencial | Justificativa: cada aquisição reduz o dinheiro disponível para as próximas compras.
- Propriedade: Mudança durante a decisão | Classificação: Dinâmico | Justificativa: outro comprador pode adquirir o livro durante o processo de decisão.
- Propriedade: Natureza dos elementos | Classificação: Discreto | Justificativa: Páginas, itens, cliques e valores discretos.
- Propriedade: Conhecimento do funcionamento | Classificação: Conhecido | Justificativa: Sabe como navegar e comprar.
### Caso 4 — Jogar uma partida de tênis
Atividade e agente considerado: Jogar tênis; agente: um tenista (simples).
Meta e hipóteses adotadas: Vencer a partida. Hipóteses: simples contra um adversário, regras oficiais.
- P — Critérios de desempenho: Pontos, games e sets ganhos; poucos erros.
- E — Ambiente: Quadra, rede, bola, adversário, árbitro, vento.
- A — Atuadores: Braço e raquete (golpes), pernas.
- S — Sensores: Visão, audição, tato/propriocepção, placar.
### Caracterização do ambiente
- Propriedade: Observabilidade | Classificação: Parcialmente observável | Justificativa: o jogador não consegue antecipar totalmente a estratégia do oponente nem o comportamento da bola.
- Propriedade: Número de agentes | Classificação: Multiagente (competitivo) | Justificativa: o oponente busca um resultado contrário ao do agente.
- Propriedade: Previsibilidade | Classificação: Estocástico | Justificativa: a reação do adversário, o vento e o quique da bola introduzem incerteza.
- Propriedade: Dependência entre decisões | Classificação: Sequencial | Justificativa: cada rebatida influencia a jogada seguinte e a pontuação.
- Propriedade: Mudança durante a decisão | Classificação: Dinâmico | Justificativa: tanto a bola quanto o adversário estão em movimento.
- Propriedade: Natureza dos elementos | Classificação: Contínuo | Justificativa: Posição, velocidade e tempo contínuos.
- Propriedade: Conhecimento do funcionamento | Classificação: Conhecido | Justificativa: Regras e física conhecidas.
### Caso 5 — Praticar tênis contra uma parede
Atividade e agente considerado: Treinar contra a parede; agente: tenista sozinho.
Meta e hipóteses adotadas: Melhorar técnica. Hipóteses: parede lisa, sem outras pessoas.
- P — Critérios de desempenho: Rebatidas consecutivas e precisão no alvo.
- E — Ambiente: Parede, piso, bola, espaço, vento.
- A — Atuadores: Braço e raquete, pernas.
- S — Sensores: Visão, audição, tato/propriocepção.
### Caracterização do ambiente
- Propriedade: Observabilidade | Classificação: Parcialmente observável | Justificativa: o agente não percebe todos os efeitos da trajetória da bola, embora a situação tenha pouca incerteza.
- Propriedade: Número de agentes | Classificação: Agente único | Justificativa: a parede não toma decisões; ela apenas provoca o rebote conforme as leis físicas.
- Propriedade: Previsibilidade | Classificação: Estocástico (baixa incerteza) | Justificativa: o retorno da bola é quase previsível, mas o vento e o piso podem causar pequenas diferenças.
- Propriedade: Dependência entre decisões | Classificação: Sequencial | Justificativa: a rebatida seguinte depende do golpe anterior.
- Propriedade: Mudança durante a decisão | Classificação: Dinâmico | Justificativa: Bola em movimento.
- Propriedade: Natureza dos elementos | Classificação: Contínuo | Justificativa: Posição, velocidade e tempo contínuos.
- Propriedade: Conhecimento do funcionamento | Classificação: Conhecido | Justificativa: o comportamento físico da bola ao atingir a parede é conhecido.
### Caso 6 — Realizar um salto de altura
Atividade e agente considerado: Salto em altura; agente: atleta, em uma tentativa.
Meta e hipóteses adotadas: Passar o sarrafo na maior altura. Hipóteses: competição, tentativas limitadas, adversários não interferem no salto.
- P — Critérios de desempenho: Altura transposta, tentativas usadas, sem lesão.
- E — Ambiente: Pista, sarrafo, colchão, gravidade, vento, juízes.
- A — Atuadores: Pernas (corrida e impulsão), tronco e braços.
- S — Sensores: Visão, equilíbrio/propriocepção, tato, audição.
### Caracterização do ambiente
- Propriedade: Observabilidade | Classificação: Parcialmente observável | Justificativa: durante a transposição, o atleta pode estar de costas e não consegue acompanhar visualmente o sarrafo.
- Propriedade: Número de agentes | Classificação: Agente único | Justificativa: os demais competidores não interferem diretamente na execução da tentativa.
- Propriedade: Previsibilidade | Classificação: Estocástico | Justificativa: pequenas mudanças na corrida, a ação do vento e o contato com o sarrafo tornam o resultado incerto.
- Propriedade: Dependência entre decisões | Classificação: Episódico | Justificativa: cada salto é considerado como uma tentativa separada.
- Propriedade: Mudança durante a decisão | Classificação: Semidinâmico | Justificativa: o cenário permanece praticamente igual, porém o limite de tempo pode influenciar o desempenho.
- Propriedade: Natureza dos elementos | Classificação: Contínuo | Justificativa: Posição, ângulos e tempo contínuos.
- Propriedade: Conhecimento do funcionamento | Classificação: Conhecido | Justificativa: Regras e física conhecidas.
### Caso 7 — Participar de um leilão de um item, realizando lances
Atividade e agente considerado: Leilão de um item; agente: licitante.
Meta e hipóteses adotadas: Arrematar abaixo do valor que atribui ao item. Hipóteses: leilão inglês (lances crescentes), valor máximo definido.
- P — Critérios de desempenho: Valor do item menos preço pago (zero se perder); nunca passar do limite.
- E — Ambiente: Plataforma, leiloeiro, item, outros licitantes, lance atual, relógio.
- A — Atuadores: Dar lance, esperar ou desistir.
- S — Sensores: Lances dos outros, preço atual, tempo restante, descrição do item.
### Caracterização do ambiente
- Propriedade: Observabilidade | Classificação: Parcialmente observável | Justificativa: o participante não conhece o limite máximo que os demais licitantes estão dispostos a pagar.
- Propriedade: Número de agentes | Classificação: Multiagente (competitivo) | Justificativa: os participantes concorrem pela aquisição de um único produto.
- Propriedade: Previsibilidade | Classificação: Estocástico (estratégico) | Justificativa: o andamento depende de ofertas dos concorrentes, que não podem ser previstas com certeza.
- Propriedade: Dependência entre decisões | Classificação: Sequencial | Justificativa: as ofertas já feitas determinam o preço atual e influenciam as próximas decisões.
- Propriedade: Mudança durante a decisão | Classificação: Dinâmico | Justificativa: outros lances podem surgir a qualquer momento, enquanto o tempo do leilão diminui.
- Propriedade: Natureza dos elementos | Classificação: Discreto | Justificativa: Lances e rodadas discretos.
- Propriedade: Conhecimento do funcionamento | Classificação: Conhecido | Justificativa: Regras do leilão conhecidas.

---

Conclusão do exercício 2 4
Depois de analisar as sete situações, faça uma comparação entre: (1) partida de tênis e prática contra a parede; (2) as informações incompletas na compra de livros usados; (3) a influência de outros agentes no futebol e no leilão.
Resposta: (1) Tênis contra uma pessoa e tênis contra a parede: na partida contra outra pessoa, o ambiente é competitivo, multiagente e estratégico, pois o oponente reage às jogadas; no treino contra a parede, há apenas um agente e o retorno é quase previsível, favorecendo o aperfeiçoamento técnico.
(2) Livros usados: o agente não consegue verificar o estoque real, as condições do livro ou a honestidade do vendedor. Por isso, toma decisões considerando incertezas e utilidade esperada, em vez de seguir apenas regras simples.
(3) Outros agentes: no futebol, existe cooperação entre colegas e competição simultânea contra adversários; no leilão, predomina a competição e cada participante mantém informações privadas. Em ambas as situações, é importante antecipar as possíveis ações dos demais.
## Exercício 2.5
Explique os dez conceitos usando suas próprias palavras, com duas a quatro linhas para cada um, e inclua um exemplo prático. Amplie cada campo conforme necessário.
Agente
Definição: elemento que capta informações do ambiente por sensores e realiza ações por meio de atuadores para alcançar determinadas metas.   Exemplo: Robô aspirador.
Função de agente
Definição: representação abstrata que associa cada histórico de percepções a uma ação.   Exemplo: Para a sequência “A sujo, A limpo, B sujo”, a ação é aspirar.
Programa de agente
Definição: realização prática da função de agente; recebe a percepção presente e produz uma ação como resultado.   Exemplo: Código do aspirador com regras se/senão.
### Racionalidade
Definição: selecionar a ação que oferece o melhor desempenho esperado de acordo com as percepções e os conhecimentos disponíveis, sem assegurar que o objetivo será alcançado.   Exemplo: Levar guarda-chuva com 80% de chance de chuva.
### Autonomia
Definição: grau em que o comportamento se apoia na experiência adquirida pelo próprio agente, em vez de depender apenas do conhecimento previamente programado.   Exemplo: Robô que aprende o mapa da casa.
### Agente reativo
Definição: atua com base somente na percepção do momento, seguindo regras que relacionam condições a ações e sem guardar histórico.   Exemplo: Frenagem automática ao detectar obstáculo.
### Agente baseado em modelo
Definição: conserva uma representação interna das partes do ambiente que não consegue observar diretamente e a atualiza com novas percepções e conhecimentos sobre suas mudanças.   Exemplo: Carro que lembra do veículo no ponto cego.
### Agente baseado em objetivos
Definição: possui uma meta definida e utiliza planejamento ou busca para encontrar um caminho até ela.   Exemplo: App de navegação que planeja a rota.
### Agente baseado em utilidade
Definição: seleciona a ação com maior utilidade esperada, levando em conta incertezas e possíveis conflitos entre objetivos.   Exemplo: GPS que pondera tempo, pedágio e segurança.
### Agente com aprendizagem
Definição: aprimora suas decisões com base na experiência, utilizando mecanismos de aprendizagem e avaliação crítica.   Exemplo: Filtro de spam que aprende com as marcações do usuário.
## Síntese com autômatos
Selecione uma das situações do exercício 2.4. Descreva três estados internos, três percepções, três ações e duas regras no formato estado atual + percepção → próximo estado e ação. Descreva de que maneira o estado interno armazena informações anteriores e apresente uma limitação desse modelo simplificado.

Resposta: caso 5 (tênis contra a parede).
Estados internos: E1 = aguardando a bola; E2 = bola em ida (já rebati); E3 = bola de volta. Percepções: P1 = bola pela direita; P2 = bola pela esquerda; P3 = bola parada/fora. Ações: A1 = forehand; A2 = backhand; A3 = recolher e reposicionar.
Regras: R1: E3 + P1 → E2 e A1. R2: E2 + P3 → E1 e A3.
O estado interno registra em que etapa do ciclo a bola está — por exemplo, se já foi rebatida ou está retornando —, algo que a percepção isolada do momento não revela.
Limitação: a representação com poucos estados discretos deixa de considerar variáveis contínuas, como velocidade, efeito da bola e cansaço do jogador.
## Entrega e avaliação
A entrega deve conter identificação, as nove análises do exercício 2.3, os sete casos completos do exercício 2.4, os dez conceitos do exercício 2.5, a síntese e as referências. Nome sugerido: NomeSobrenome_Atividade_AgentesInteligentes. Formato e prazo conforme orientação da professora.
Atividade 1,0 ponto (A2) : exercício 2.3: 30%; exercício 2.4: 40%; exercício 2.5: 20%; síntese, organização e referências: 10%.
Material-base: Capítulo 2 — Agentes inteligentes, arquivo disponibilizado para a aula de 19/10/2026. Referências: RUSSELL, S.; NORVIG, P. Inteligência Artificial, capítulo 2 — Agentes inteligentes (material-base disponibilizado para a aula). Anotar aqui outras fontes consultadas, se houver.
