# Scripts Medicina — AmorSaúde SJDR

---

## 📑 Índice

- [Scripts de Atendimento](#scripts-de-atendimento)
  - [1. Check-in](#1-check-in)
  - [2. Oferta de Exames (Gatilhos de Venda)](#2-oferta-de-exames-gatilhos-de-venda)
  - [3. Contato para Orçamentos Não Efetivados](#3-contato-para-orçamentos-não-efetivados)
  - [4. Objeções e Dúvidas](#4-objeções-e-dúvidas)
  - [5. Encaminhamento](#5-encaminhamento)
  - [6. Follow-up Pós-Exame](#6-follow-up-pós-exame)
- [Rotina — Medicina](#rotina--medicina)
- [Glossário](#glossário)

---

## Scripts de Atendimento

### 1. Check-in

| | |
|---|---|
| **Objetivo:** | Recepcionar o paciente, validar dados e orientar sobre a consulta |
| **Quando usar:** | Chegada do paciente à clínica |
| **Quem executa:** | Recepção Medicina |
| **Canal:** | 🏥 Presencial |

> "Bom dia, [nome]. Seja bem-vindo à AmorSaúde! Vou só confirmar seus dados para atualizar no sistema, tudo bem? … Sua consulta é com o Dr(a). [nome], às [hora]. O tempo médio de espera hoje é de [x] minutos. Enquanto isso, fique à vontade, qualquer dúvida é só me chamar."

**1.1 Check-in (com cashback)**

> "Bom dia, [nome]. Seja bem-vindo à AmorSaúde! Vou só confirmar seus dados para atualizar no sistema, tudo bem? … Sua consulta é com o Dr(a). [nome], às [hora]. O tempo médio de espera hoje é de [x] minutos."

> "Ah, posso olhar se você possui cashback pra utilizar no seu pagamento? Verifiquei aqui e você tem [R$ valor] de cashback disponível para usar no seu pagamento. Vamos realizar o seu check-in?"

🔗 Site para consulta do cashback: [busca-cashback.onrender.com](https://busca-cashback.onrender.com/)

---

### 2. Oferta de Exames (Gatilhos de Venda)

| | |
|---|---|
| **Objetivo:** | Converter orçamento de exames em venda imediata após a consulta |
| **Quando usar:** | Pós-consulta, quando o médico solicitar exames |
| **Quem executa:** | Recepção Medicina |
| **Canal:** | 🏥 Presencial |

> [!NOTE]
> Cada gatilho abaixo é uma abordagem diferente para o mesmo objetivo. Escolha o mais adequado ao perfil do paciente, ou combine-os conforme o item 2.7.

**2.1 Gatilho de Autoridade**

**Sangue:**

> "A coleta é feita aqui na clínica mesmo e a amostra é enviada no mesmo dia pro DB Diagnósticos, o laboratório de referência que atende praticamente todos os laboratórios da cidade. O valor é R$ [valor], orçamento válido por 3 dias, pois a tabela pode ser atualizada. Qual forma de pagamento é melhor pra você — Pix ou cartão?"

**Clínica Parceira:**

> "Você consegue agendar ainda essa semana com nossa clínica parceira, que é referência na cidade e tem excelente estrutura. O valor é R$ [valor], orçamento válido por 3 dias, pois pode ter atualização. O pagamento vai ser no Pix ou cartão?"

**2.2 Gatilho de Urgência**

**Sangue:**

> "Esse orçamento é válido por 3 dias porque, como a gente depende do laboratório, o valor pode sofrer alteração. Você consegue coletar amanhã de manhã mesmo, e o valor é R$ [valor]. O pagamento vai ser no Pix ou cartão?"

**Clínica Parceira:**

> "Esse orçamento é válido por 3 dias porque, como a gente depende da clínica parceira, o valor pode sofrer alteração. Você consegue agendar essa semana mesmo, e o valor é R$ [valor]. O pagamento vai ser no Pix ou cartão?"

**2.3 Gatilho de Escassez**

**Sangue:**

> "As coletas aqui na clínica são limitadas por manhã, e o DB Diagnósticos é o que faz a coleta da maioria dos laboratórios aqui de São João. Amanhã, por exemplo, já estamos quase no limite de coletas. O valor é R$ [valor] — se você já deixar pago hoje, garantimos sua coleta. O pagamento vai ser no Pix ou cartão?"

**Clínica Parceira:**

> "Os horários com a clínica parceira são bem disputados e costumam preencher rápido. O valor é R$ [valor] — se você já deixar pago hoje, garantimos seu agendamento. O pagamento vai ser no Pix ou cartão?"

**2.4 Gatilho de Prova Social**

**Sangue:**

> "Muitos pacientes têm feito esses exames e descoberto causas simples pra sintomas como cansaço e indisposição. O valor é R$ [valor], e conseguimos fazer amanhã cedo. O pagamento vai ser no Pix ou cartão?"

*Variação com testemunho pessoal (usar apenas se for autêntico para o colaborador):*

> "Eu mesma estava com a imunidade muito baixa, ficando doente direto, fiz aqui e descobri que estava com falta de vitaminas e melhorei muito depois da reposição."

*Variação com prova social de terceiros (alternativa):*

> "Uma paciente nossa descobriu uma deficiência de vitamina D que explicava o cansaço que ela sentia há meses. Depois do tratamento, a melhora foi muito rápida."

**Clínica Parceira:**

> "Vários pacientes do Dr(a). [nome] têm feito esse exame na clínica parceira e relatado ótimos resultados no acompanhamento. O valor é R$ [valor], válido até [data]. O pagamento vai ser no Pix ou cartão?"

**2.5 Gatilho de Ancoragem/Oportunidade**

**Sangue:**

> "Esse exame costuma ter um valor mais alto em outros laboratórios, mas conseguimos esse preço especial de R$ [valor] com o DB Diagnósticos, que é o laboratório de referência da cidade. O orçamento vale por 3 dias, porque a tabela pode mudar a qualquer momento. Qual forma de pagamento é melhor pra você?"

**Clínica Parceira:**

> "Por causa da parceria, conseguimos um valor mais acessível de R$ [valor] pra esse exame. O orçamento vale até [data], porque os preços podem ser atualizados. O pagamento vai ser no Pix ou cartão?"

**2.6 Gatilho de Conveniência**

**Sangue:**

> "Podemos deixar tudo pago agora, e amanhã é só vir pra coleta. A amostra é enviada pro DB Diagnósticos, o laboratório que atende os principais laboratórios da cidade. O valor é R$ [valor], orçamento válido por 3 dias. Qual forma de pagamento é melhor pra você?"

**Clínica Parceira:**

> "Podemos deixar essa parte paga por aqui e você agenda direto com a clínica parceira no melhor horário pra você. O valor é R$ [valor], sendo uma parte paga aqui e outra lá no dia do exame. O orçamento vale por 3 dias. O pagamento vai ser no Pix ou cartão?"

**2.7 Combo: Autoridade + Escassez + Urgência + Oportunidade + Conveniência + Prova Social**

**Sangue:**

> "A coleta é feita aqui mesmo na clínica e vai direto pro DB Diagnósticos, que é o laboratório de referência da cidade — é o mesmo que atende praticamente todos os laboratórios de São João."

> "As coletas são limitadas por manhã, e amanhã já estamos quase no limite."

> "O valor é R$ [valor], e o orçamento vale até [data], porque a tabela pode mudar a qualquer momento."

> "Podemos deixar tudo pago agora, assim amanhã é só vir pra coleta. Qual forma de pagamento é melhor pra você?"

*Variação com prova social leve (opcional):*

> "Eu mesma/Uma paciente nossa descobriu um problema simples que explicava os sintomas, e depois do tratamento a melhora foi rápida."

**Clínica Parceira:**

> "Temos parceria com uma clínica referência na cidade, com ótimos profissionais e estrutura."

> "Os horários deles são bem disputados, mas acredito que você ainda consegue encaixe essa semana."

> "O valor é R$ [valor], orçamento válido por poucos dias, porque os preços podem atualizar."

> "Se quiser, já podemos deixar a parte do pagamento garantido aqui, você só agenda o horário direto com eles. Qual forma de pagamento é melhor pra você?"

*Variação com toque de urgência mais direta:*

> "É bom aproveitar que ainda tem vaga essa semana, porque o pessoal costuma agendar logo depois da consulta."

---

### 3. Contato para Orçamentos Não Efetivados

| | |
|---|---|
| **Objetivo:** | Reativar pacientes que receberam orçamento mas não realizaram os exames |
| **Quando usar:** | 3 a 7 dias após o orçamento |
| **Quem executa:** | Recepção Medicina |
| **Canal:** | 📞 Telefone / 💬 WhatsApp |
| **Cadência:** | 1ª tentativa: 3 dias / 2ª tentativa: 7 dias / Máximo: 3 tentativas |

> "Oi, [nome]! Tudo bem? Aqui é [seu nome] da AmorSaúde. Tô retornando sobre os exames que o Dr(a). [nome] pediu na sua última consulta, que são importantes pra dar sequência no acompanhamento."

> "As coletas são por ordem de chegada, e amanhã cedo ainda temos algumas vagas livres. O valor é R$ [valor], e o orçamento é válido por tempo limitado, porque a tabela pode mudar."

> "Quer já deixar pago agora pra garantir o valor e só vir fazer amanhã? Vai preferir no Pix ou cartão?"

**Se o paciente hesitar:**

> "Tranquilo! Só lembrando que o valor pode mudar na semana que vem, porque depende do laboratório/clínica parceira. Se quiser, já deixo o pagamento registrado pra garantir o valor atual, tá?"

---

### 4. Objeções e Dúvidas

| | |
|---|---|
| **Objetivo:** | Contornar objeções com foco em solução |
| **Quando usar:** | Sempre que o paciente apresentar resistência ao pagamento/agendamento |
| **Quem executa:** | Recepção Medicina |
| **Canal:** | 🏥 Presencial / 📞 Telefone |

**Frase padrão:**

> "Entendo, [nome]. Temos opções de parcelamento no cartão, além de Pix e Crédito PF da clínica. Assim você já sai com tudo resolvido hoje e evita ter que voltar."

**Tabela de objeções específicas:**

| Situação do paciente | Frase estratégica |
|:---|:---|
| "Depois eu vejo" | "Claro! Só lembrando que o valor pode mudar, tá? Se quiser, já deixo pago e você faz no seu melhor dia." |
| "Vou esperar o retorno" | "Perfeito! Só que o médico pediu justamente pra trazer esses resultados no retorno, vale a pena já deixar resolvido." |
| "Tô sem tempo" | "Nem precisa agendar, é só vir de manhã, coleta rápida e pronto. Deixando pago, é só chegar e fazer." |
| "Achei caro" | "Esse valor é o que conseguimos com o laboratório parceiro, normalmente é bem mais alto fora. Por isso vale garantir enquanto tá nesse preço." |

> [!TIP]
> **DICA:** No momento da negociação, apresente sempre **o valor da parcela** ao paciente, pois esse já inclui as taxas de forma diluída. Se o paciente manifestar interesse em pagar à vista, utiliza-se o valor informado pelo sistema. Dessa forma, evitamos questionamentos sobre cobranças adicionais e não há necessidade de oferecer desconto para o pagamento à vista.

---

### 5. Encaminhamento

| | |
|---|---|
| **Objetivo:** | Orientar o paciente sobre próximos passos após aceitar o exame |
| **Quando usar:** | Após fechamento do pagamento/agendamento |
| **Quem executa:** | Recepção Medicina |
| **Canal:** | 🏥 Presencial |

> "Perfeito, [nome]. Aqui está sua guia com todas as informações de local, preparo e prazo. Qualquer dúvida, pode falar com a gente."

---

### 6. Follow-up Pós-Exame

| | |
|---|---|
| **Objetivo:** | Reengajar paciente após resultado dos exames para agendar retorno |
| **Quando usar:** | Quando os resultados ficarem prontos (geralmente 3-7 dias após coleta) |
| **Quem executa:** | Recepção Medicina |
| **Canal:** | 📞 Telefone / 💬 WhatsApp |

> "Oi, [nome]! Aqui é [seu nome] da AmorSaúde. Tudo bem? Estou entrando em contato porque os resultados dos seus exames já ficaram prontos."

> "O Dr(a). [nome] pediu esses exames justamente para avaliar no retorno. Posso já agendar sua consulta de retorno para [data/horário]? Assim o(a) doutor(a) já analisa tudo certinho."

**Se o paciente quiser receber os resultados primeiro:**

> "Claro! Vou encaminhar os resultados pelo WhatsApp. E quando quiser agendar o retorno, é só nos chamar, tá?"

---

## Rotina — Medicina

### 1. Check-in

- [ ] Cumprimentar com cordialidade.
- [ ] Solicitar documento/cartão (Cartão de TODOS, quando aplicável).
- [ ] Conferir dados no Amei e atualizar se necessário.
- [ ] Verificar se o paciente possui cashback disponível e informar → 🔗 [busca-cashback.onrender.com](https://busca-cashback.onrender.com/)
- [ ] Registrar check-in.
- [ ] Confirmar com o paciente: especialidade, nome do médico e horário.
- [ ] Informar tempo médio de espera.
- [ ] Conveniados: utilizar a [planilha de Conveniados](https://docs.google.com/spreadsheets/d/10P_QUoCBZg2l2QDD3TeiwwqURKNpbgnawSr52qFQE1c/edit?gid=1618174664#gid=1618174664) conforme orientações.
- [ ] Realizar as simulações dos pacientes e inserir na planilha: [Simulações - diária](https://docs.google.com/spreadsheets/d/1ZqIwlB1scTLtOWBfS14Atv80m_r5V2UBH7XHJF9sQcs/edit?gid=0#gid=0)

### 2. Durante a Consulta

- [ ] Chamar o paciente quando liberado.
- [ ] Conferir se prontuário está disponível no sistema para o médico.
- [ ] Manter atenção ao painel/agenda para evitar atrasos.

### 3. Pós-Consulta

- [ ] Receber paciente cordialmente após consulta.
- [ ] Verificar exames solicitados pelo médico no Amei.
- [ ] Explicar valores com clareza e padronização, oferecendo as formas de pagamento (dinheiro, Pix, cartão, Crédito PF).

**Caso o paciente aceite:**

- [ ] Emitir guia ou encaminhamento.
- [ ] Direcionar ao laboratório parceiro ou setor responsável.
- [ ] Registrar no sistema a decisão do paciente.
- [ ] Reforçar as orientações médicas e agradecer.

### 4. Orçamentos Não Efetivados

- [ ] Acessar relatórios dos orçados não efetivados no Slack e inserir os nomes na planilha.
- [ ] Fazer contato ativo (ligação/WhatsApp) com script padrão (item 3).
- [ ] Atualizar planilha após cada contato (status: agendado, reagendado, não fechou).

### 5. Lista de Espera

> [!IMPORTANT]
> Quando **não houver vaga** ou a especialidade não estiver disponível, **não utilize** a expressão "lista de espera". Explique que as agendas são abertas semanalmente e que, na próxima semana, entraremos em contato para agendar. Se não tiver a especialidade confirmada ainda, informe que ainda dentro do mês entraremos em contato assim que tivermos disponível.

### 📌 Checklist de Encerramento do Dia

- [ ] Todos os pacientes do dia tiveram exames oferecidos/encaminhados?
- [ ] Orçamentos não efetivados foram registrados?
- [ ] Planilha de simulações atualizada?
- [ ] Painel/agenda do dia seguinte verificado?
- [ ] Recepção organizada para o próximo dia?

### 📌 Protocolo de Escalação

| Situação | Ação |
|----------|------|
| Paciente reclama ou está insatisfeito | Ouvir com empatia, registrar a queixa e encaminhar para a coordenação |
| Paciente pede desconto além do permitido | Informar que os valores já são diferenciados e encaminhar para coordenação, se insistir |
| Urgência médica real | Encaminhar imediatamente para atendimento ou orientar UPA/SAMU |

---

## Glossário

| Termo | Definição |
|-------|-----------|
| **Cartão de TODOS** | Cartão de benefícios que dá acesso a consultas com valores acessíveis na AmorSaúde |
| **Crédito PF** | Linha de crédito pessoal oferecida pela clínica para parcelamento de procedimentos |
| **DB Diagnósticos** | Laboratório de referência parceiro da AmorSaúde para coleta e análise de exames |
| **Cashback** | Valor acumulado pelo paciente que pode ser usado como desconto no pagamento |
| **Amei** | Sistema de gestão utilizado pela AmorSaúde para cadastro e prontuários |
| **Clínica Parceira** | Clínica conveniada para realização de exames de imagem e procedimentos especializados |
