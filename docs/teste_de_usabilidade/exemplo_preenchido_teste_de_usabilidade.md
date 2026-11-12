# Relatório de Teste de Usabilidade (Exemplo Preenchido)

**Nome do Sistema:** LabReserve — Sistema de Gestão e Agendamento de Laboratórios Acadêmicos

**Versão Avaliada:** v1.2 - MVP Funcional (Ambiente de Homologação)

**Equipe Responsável:** 
* Ana Clara Souza (Moderadora)
* Lucas Mendes (Observador e Cronometrista)
* Mariana Oliveira (Relatora e Analista de Dados)

**Data de Realização:** 10/11/2026

## 1. Visão Geral do Sistema e Objetivos do Teste

* **Propósito do Sistema:** Aplicação web desenvolvida para permitir que docentes e monitores de uma instituição de ensino superior consultem a disponibilidade e realizem reservas de laboratórios de informática e equipamentos audiovisuais, substituindo o controle manual feito por planilhas.
* **Objetivos da Avaliação:** Verificar se os docentes conseguem realizar o fluxo completo de busca, reserva e cancelamento de salas de forma autônoma, sem necessidade de suporte técnico, além de identificar gargalos de navegação na grade de horários.

## 2. Perfil dos Participantes e Ambiente de Teste

### 2.1. Perfil dos Participantes

O público-alvo definido para o teste são docentes e monitores acadêmicos com diferentes níveis de familiaridade digital que utilizam laboratórios regularmente em suas disciplinas. Foram recrutados 5 participantes voluntários externos à equipe de desenvolvimento.

| ID | Idade | Ocupação / Área | Familiaridade com Tecnologia (Baixa/Média/Alta) | Experiência com sistemas similares? |
| :--- | :--- | :--- | :--- | :--- |
| **P1** | 48 | Professor (Engenharia Civil) | Média | Não (usa apenas planilhas) |
| **P2** | 29 | Professora (Design Gráfico) | Alta | Sim (Google Agenda / Moodle) |
| **P3** | 55 | Professor (Direito) | Baixa | Não |
| **P4** | 22 | Monitora (Ciência da Computação) | Alta | Sim (Sistemas acadêmicos) |
| **P5** | 37 | Professora (Biologia) | Média | Sim (Sistema antigo da instituição) |

### 2.2. Ambiente e Ferramentas Utilizadas

* **Dispositivo / Sistema Operacional:** Notebook Lenovo ThinkPad, Windows 11, tela 14" (resolução 1920x1080), mouse óptico externo.
* **Navegador / Plataforma:** Google Chrome (versão 130.0) em aba anônima (para evitar cache).
* **Ferramentas de Apoio:** OBS Studio (gravação de tela e áudio do protocolo *Think Aloud*), Google Forms (aplicação do questionário SUS pós-teste) e cronômetro digital.

## 3. Protocolo e Cenários de Tarefas

* **Tarefa 1 (T1) - Consulta de Disponibilidade:**
  * *Cenário:* "Você precisa ministrar uma aula prática extra na próxima quarta-feira (18/11) no período da manhã, das 08h00 às 10h00, para uma turma de 30 alunos. Verifique no sistema quais laboratórios de informática estão livres nesse horário e comportam toda a turma."
  * *Critério de Sucesso:* O participante filtra ou localiza a grade da data correta e identifica verbalmente o "Laboratório 03 (Capacidade: 35 lugares)" como opção válida.

* **Tarefa 2 (T2) - Realização de Reserva com Equipamento:**
  * *Cenário:* "Agora que você encontrou o laboratório ideal para a aula de quarta-feira (18/11, das 08h00 às 10h00), realize a reserva da sala para a disciplina 'Algoritmos I' e solicite também um projetor multimídia portátil para essa aula."
  * *Critério de Sucesso:* O participante preenche o formulário de reserva, seleciona o item adicional e recebe a confirmação visual de agendamento concluído.

* **Tarefa 3 (T3) - Alteração de Horário de Reserva Existente:**
  * *Cenário:* "A coordenação avisou que sua aula do dia 18/11 precisará começar uma hora mais tarde, passando a ser das 09h00 às 11h00. Atualize a reserva que você acabou de fazer para refletir esse novo horário."
  * *Critério de Sucesso:* O participante localiza sua reserva na área "Meus Agendamentos" e altera o intervalo de horário com sucesso.

* **Tarefa 4 (T4) - Cancelamento de Reserva:**
  * *Cenário:* "Devido a um evento acadêmico na instituição, sua aula prática foi adiada. Cancele a reserva do dia 18/11 para liberar o laboratório para outros professores."
  * *Critério de Sucesso:* O participante encontra a opção de cancelamento, confirma a ação e verifica que a reserva não consta mais como ativa.

## 4. Resultados Quantitativos

### 4.1. Taxa de Sucesso e Tempo de Execução

**Legenda:** **S** = Sucesso sem ajuda | **SA** = Sucesso com Ajuda | **F** = Falha

| Participante | T1 (Status / Tempo) | T2 (Status / Tempo) | T3 (Status / Tempo) | T4 (Status / Tempo) | Total de Erros / Cliques Errados |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **P1** | S / 01m10s | SA / 03m45s | F / 04m00s | S / 00m55s | 6 |
| **P2** | S / 00m42s | S / 01m50s | SA / 02m30s | S / 00m30s | 2 |
| **P3** | SA / 02m15s | F / 04m20s | F / 03m50s | SA / 01m40s | 9 |
| **P4** | S / 00m30s | S / 01m15s | S / 01m40s | S / 00m25s | 1 |
| **P5** | S / 00m58s | S / 02m20s | SA / 03m10s | S / 00m45s | 4 |
| **Média / Taxa de Sucesso** | **80% S (100% c/ ajuda) / 01m07s** | **60% S (80% c/ ajuda) / 02m42s** | **20% S (60% c/ ajuda) / 03m02s** | **80% S (100% c/ ajuda) / 00m47s** | **4,4 erros/usuário** |

### 4.2. Avaliação de Satisfação (Questionário SUS - *System Usability Scale*)

*(Referência: Abaixo de 50 = Inaceitável; 50–68 = Marginal; Acima de 68 = Aceitável; Acima de 80 = Excelente).*

| Participante | P1 | P2 | P3 | P4 | P5 | **Média Geral SUS** |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **Pontuação SUS** | 62,5 | 77,5 | 47,5 | 85,0 | 67,5 | **68,0 (Limite Aceitável)** |

## 5. Resultados Qualitativos e Observações

* **Pontos Positivos (O que funcionou bem):**
  * **Clareza na busca inicial (T1):** Quatro dos cinco participantes elogiaram o código de cores da grade de horários (verde para livre, vermelho para ocupado), afirmando que a leitura visual é imediata.
  * **Fluxo de cancelamento intuitivo (T4):** O botão vermelho com ícone de lixeira e a mensagem de confirmação (*"Tem certeza que deseja liberar este laboratório?"*) foram considerados muito claros e seguros por todos.

* **Dificuldades e Pontos de Atrito:**
  * **Invisibilidade da opção de editar reserva (T3):** Este foi o maior gargalo do sistema. Os usuários clicaram sobre o card da reserva em "Meus Agendamentos" esperando abrir uma tela de edição, mas o card não era clicável. O botão de editar estava escondido dentro de um menu de "três pontinhos" (`⋮`) com baixo contraste no canto superior direito. P1 e P3 desistiram da tarefa após tentarem clicar várias vezes no título da reserva.
  * **Termo técnico confuso na reserva (T2):** Para solicitar o projetor multimídia, o formulário exibia um campo chamado *"Alocar Periféricos de TI"*. P1, P3 e P5 não associaram o termo "periféricos" a um projetor e demoraram a encontrar a opção.
  * **Falta de validação de capacidade antes do envio (T2):** P3 tentou inicialmente reservar uma sala para 20 alunos; o sistema só informou o erro após ele preencher todo o formulário e clicar em "Confirmar", apagando os campos já preenchidos.

## 6. Diagnóstico de Problemas e Plano de Melhorias

**Escala de Severidade:** **1** - Cosmético | **2** - Menor | **3** - Maior | **4** - Catastrófico

| ID | Descrição do Problema | Tarefa(s) Afetada(s) | Usuários Afetados | Severidade (1 a 4) | Recomendação de Melhoria (Redesign) |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **PROB-01** | **Falta de affordance para edição de reservas:** O card da reserva não é clicável e o menu `⋮` passa despercebido, impedindo a alteração de horários. | T3 | P1, P2, P3, P5 | 4 (Catastrófico) | Tornar o card inteiro clicável para abrir os detalhes/edição e substituir o ícone `⋮` por um botão explícito com rótulo **"Editar Horário"** ao lado do botão cancelar. |
| **PROB-02** | **Perda de dados preenchidos após erro de validação:** Ao submeter um formulário com capacidade incompatível, a página recarrega e limpa os campos digitados. | T2 | P3 | 3 (Maior) | Implementar validação em tempo real (filtrando salas incompatíveis antes da seleção) e manter o estado dos campos preenchidos em caso de alerta. |
| **PROB-03** | **Terminologia técnica inadequada ao usuário:** O rótulo *"Alocar Periféricos de TI"* não comunica claramente que se trata de equipamentos audiovisuais (projetor, caixa de som). | T2 | P1, P3, P5 | 2 (Menor) | Renomear a seção para **"Equipamentos Adicionais (Projetor, Áudio, etc.)"** utilizando linguagem natural próxima ao vocabulário docente. |
| **PROB-04** | **Ausência de filtro por capacidade na tela inicial:** O usuário precisa passar o mouse sobre cada sala para descobrir quantos alunos ela comporta. | T1 | P1, P3 | 2 (Menor) | Adicionar um filtro rápido de "Número mínimo de lugares" no topo da grade de horários e exibir a lotação máxima ao lado do nome da sala (ex.: *Lab 03 - 35 lugares*). |

## 7. Conclusão da Equipe

O teste de usabilidade demonstrou que o sistema **LabReserve** possui uma base visual agradável e atende bem às tarefas básicas de consulta e cancelamento, alcançando uma média SUS de **68,0** (no limite entre marginal e aceitável). No entanto, a avaliação empírica foi fundamental para revelar falhas graves de interação que a equipe de desenvolvimento não havia percebido, especialmente na tarefa de edição de reservas (apenas 20% de sucesso sem ajuda) e no uso de jargões técnicos da área de TI em um sistema voltado para professores de diversas áreas.

**Prioridades para a próxima sprint (refatoração):**
1. Corrigir imediatamente o problema crítico **PROB-01**, tornando a edição de reservas visível e direta.
2. Ajustar a retenção de dados no formulário e aplicar validação preventiva (**PROB-02**).
3. Revisar os textos da interface para eliminar jargões técnicos (**PROB-03**) e incluir a capacidade visível nas salas (**PROB-04**).
