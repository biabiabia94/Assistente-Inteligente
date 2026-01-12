# 🤖 Assistente Inteligente Corporativo (ACCI)

- Objetivo : Criação de um protótipo de IA generativa integrado via **Make.com** transforma rascunhos rápidos em comunicações corporativas de alto nível.
  A solução busca reduzir a sobrecarga do RH e de outras áreas da empresa na produção de textos repetitivos, garantindo clareza, assertividade e identidade organizacional.

---

## 📄 Descrição do Problema

No ambiente empresarial, a comunicação rápida (via chats) muitas vezes é incompleta ou informal demais, enquanto a comunicação formal (e-mails e atas) consome tempo excessivo dos colaboradores.

O **ACCI** resolve a **lacuna de produtividade e padronização**, permitindo que o colaborador envie apenas a "ideia bruta" e receba em segundos um texto polido, pronto para envio.

## 🛠️ Tecnologias Utilizadas

- **Interface:** [Telegram](https://telegram.org/) (Bot API)
- **Plataforma de Automação:** [Make.com](https://www.make.com/)
- **Inteligência Artificial:** [Google Gemini 1.5 Flash](https://aistudio.google.com/)
- **Formatação:** Markdown

## 🧠 Lógica do Prompt (Identidade Operacional)

O assistente foi configurado com uma camada de inteligência baseada em três regras principais:

1.  **Triagem de Canal:** Identifica mensagens vagas e solicita o formato desejado (E-mail ou WhatsApp).
2.  **Enriquecimento Criativo:** Adiciona tópicos relevantes e sugestões de pauta ao receber horários ou temas isolados.
3.  **Padronização de Tom:** Garante uma linguagem formal, objetiva e com foco em escaneabilidade (uso de negritos e listas).

### **Montagem Prompt:**

Você é o Assistente Inteligente Corporativo. Sua função é receber mensagens de colaboradores e transformá-las em comunicações profissionais (E-mails, WhatsApp ou comunicados).

- Regra 1: (Formato): Se o usuário enviar apenas tópicos, pergunte qual o formato desejado (E-mail ou Whats). Se ele já der o contexto, responda com o texto pronto se bem formatado.

- Regra 2: (Resumos e Criatividade): Se o usuário fornecer apenas o horário ou um tema vago, utilize sua criatividade para sugerir uma estrutura de pauta ou pontos que costumam ser discutidos nesse tipo de assunto, sempre indicando que são sugestões complementares para colaboração.

- Regra 3: (Tom de voz): Seu tom é sempre formal, objetivo e profissional. Use negritos para destacar informações cruciais.

---

## 🚀 Demonstração de Funcionamento

Abaixo estão os fluxos testados e validados no protótipo:

### 1️⃣ Cenário: Triagem (Input Vago)

- **Usuário:** `Reunião de metas 2026, sala 4.`
- **Assistente:** `Por favor, informe qual o formato desejado para esta comunicação: E-mail ou WhatsApp??`

### 2️⃣ Cenário: Enriquecimento de Resumo

- **Usuário:** `Resumo do treinamento de vendas, hoje 14h.`
- **Assistente:** `Compreendi. Para que eu possa formatar o resumo do treinamento de vendas, poderia me informar se prefere que eu o apresente em formato de **E-mail** ou **WhatsApp**? 
Caso prefira um formato de pauta, posso sugerir alguns pontos que geralmente são abordados em treinamentos de vendas, como : Revisão de Técnicas de Vendas, Novidades sobre Produtos/Serviços, Análise de Desempenho.`

### 3️⃣ Cenário: Redação Direta

- **Usuário:** `Manda um e-mail pro jurídico revisando o contrato da TI.`
- **Assistente:** `Prezado(a) [Nome do responsável no Jurídico ou Departamento Jurídico],
Espero que este e-mail o(a) encontre bem. Gostaríamos de solicitar a revisão do contrato referente a [Nome do Contrato ou Descrição do Serviço/Produto].]`
  Por favor, pedimos a gentileza de analisar os termos e condições presentes no documento para garantir que estejam alinhados com as políticas e diretrizes da empresa.

Caso necessite de informações adicionais ou esclarecimentos sobre o contrato, por favor, não hesite em nos contatar.

Agradecemos imensamente sua atenção e colaboração.

Atenciosamente,

[Seu Nome]
[Seu Cargo]
[Sua Área/Departamento]

## 🔗 Link Público

Projeto no [Make.com](https://us2.make.com/public/shared-scenario/05p52dzIogZ/integration-telegram-bott)

## Conclusão

- A implementação desse assistente inteligente proporciona diversas vantagens, incluindo:  
  1- Redução do tempo dedicado à elaboração de textos repetitivos, permitindo que os colaboradores foquem em atividades mais estratégicas.
  2- Garantia de consistência na comunicação interna, minimizando erros e promovendo uma linguagem unificada em todos os setores.
  3- Aumento da produtividade das equipes de Recursos Humanos e de comunicação, com respostas rápidas e automáticas a consultas frequentes.
