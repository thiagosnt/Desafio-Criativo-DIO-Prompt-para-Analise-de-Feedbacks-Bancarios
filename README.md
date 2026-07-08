# Desafio Criativo DIO - Prompt para Análise de Feedbacks Bancários
Este repositório documenta a construção de um prompt estruturado para orientar uma Inteligência Artificial na análise de dados de clientes, desenvolvido como parte do Desafio Criativo da DIO.

## 🎯 Objetivo ##
O objetivo principal deste projeto é criar um comando claro para que a IA atue como Analista de Dados e Experiência do Cliente. O foco é analisar feedbacks em texto livre e notas de satisfação sobre recusas de aumento de limite no cartão de crédito , identificando os principais motivos de frustração, o tom emocional das mensagens e o risco de cancelamento de conta (churn).  

## 🏗️ Construção do Prompt ##
O desenvolvimento seguiu três etapas estratégicas:

**Passo 1: Definição da Intenção**
- Foco da Análise: Avaliar comentários sobre recusas de aumento de limite para mapear frustrações e o tom emocional.  
- Público-alvo: Equipes de Risco e Crédito em conjunto com o time de Comunicação.
- Entrega Esperada: Uma lista de pontos de atrito e uma tabela categorizando as reclamações, com sugestões de abordagem.
- Critério de Sucesso: O resultado deve ser direto ao ponto, classificar claramente os níveis de insatisfação e trazer recomendações práticas aplicáveis ao dia a dia.

**Prompt_1**: Quero que a IA analise os comentários de clientes sobre as recusas de aumento de limite no cartão de crédito para identificar os principais motivos de frustração e o tom emocional das mensagens.
O resultado será usado por equipe de Risco e Crédito em conjunto com o time de Comunicação para apoiar a criação de respostas mais empáticas e a possível revisão dos critérios de análise de crédito.
A entrega deve conter uma lista dos principais pontos de atrito e uma tabela categorizando as reclamações (ex: falta de transparência, demora na análise), incluindo sugestões de como o atendimento pode abordar cada caso.
O resultado será considerado bom se for direto ao ponto, classificar claramente os níveis de insatisfação e trouxer recomendações práticas que a equipe possa aplicar no dia a dia.

**Passo 2: Contexto e Restrições**
- Contexto de Negócio: Análise de pedidos negados de limite e do suporte prestado via chat do aplicativo.
- Dados Disponíveis para a IA: Data do comentário, canal de atendimento, texto livre, nota de satisfação (1 a 5) e tempo de espera.
- Critérios de Classificação: Motivo principal da queixa, tom emocional do cliente e risco de churn.
- Regras de Segurança: A IA deve usar apenas os dados fornecidos e não pode inventar números, causas ou conclusões. É expressamente proibido expor dados pessoais ou sensíveis (como CPF, nome, número da conta ou valor exato da renda). Qualquer informação desse tipo deve ser ocultada caso apareça nos comentários. A linguagem deve ser executiva, objetiva e orientada a soluções.

**Prompt_2**: 
- Contexto: Estou trabalhando com feedbacks de clientes bancários relacionados a pedidos negados de aumento de limite do cartão de crédito e ao suporte prestado via chat do aplicativo.
- Dados disponíveis: A base contém data do comentário, canal de atendimento, texto livre do feedback deixado pelo cliente, nota de satisfação (de 1 a 5) e tempo de espera até a resposta.
- Critérios de análise: A IA deve classificar os feedbacks por motivo principal da queixa (ex: falta de clareza nos critérios, demora na análise, limite incompatível com o mercado), tom emocional do cliente (frustração, - raiva, dúvida) e risco de cancelamento do cartão (churn).
- Cuidados e restrições:
   - Use apenas os dados fornecidos.
   - Não invente números, causas ou conclusões.
   - Não exponha dados pessoais ou sensíveis (como CPF, nome, número da conta ou valor exato da renda). Oculte qualquer informação desse tipo caso apareça nos comentários.
   - Se houver informação insuficiente, indique a limitação.
   - Use linguagem executiva, objetiva e orientada a soluções práticas, adequada para equipes de Risco e Comunicação.

## 🚀 O Prompt Final (Passo 3) ##: 
Abaixo está o comando consolidado que deve ser enviado para a Inteligência Artificial:
Atue como Analista de Dados e Experiência do Cliente numa instituição financeira.

Sua tarefa é analisar feedbacks em texto livre e notas de satisfação sobre recusas de aumento de limite no cartão de crédito e o suporte prestado via chat. O objetivo principal é identificar os principais motivos de frustração, o tom emocional das mensagens e o risco de cancelamento de conta (churn).

Contexto: O resultado da análise será usado pelas equipas de Risco, Crédito e Comunicação. A intenção é apoiar a criação de respostas mais empáticas, rever possíveis falhas no atendimento e fornecer dados para a revisão dos critérios de análise de crédito. O foco é transformar comentários soltos em insights claros e acionáveis.

Dados disponíveis: Serão fornecidos registos contendo data do comentário, canal de atendimento (chat), texto livre do feedback deixado pelo cliente, nota de satisfação (NPS de 1 a 5) e tempo de espera até à resposta.

Instruções de análise:
1. Classifique os feedbacks por motivo principal da queixa (ex: falta de transparência, demora na análise, limite incompatível), tom emocional (frustração, raiva, dúvida) e risco de cancelamento (alto, médio, baixo).
2. Identifique os principais padrões, problemas recorrentes, elogios (se houver) e oportunidades de melhoria.
3. Aponte evidências nos dados fornecidos, usando exemplos curtos extraídos dos comentários para ilustrar cada problema.
4. Sugira ações práticas para a equipa de Comunicação (ex: novos guiões de atendimento) e para a equipa de Risco.

Formato da resposta: Entregue um resumo executivo inicial com até 5 linhas. Em seguida, apresente uma tabela contendo as colunas: Tema da Queixa, Sentimento Predominante, Exemplo (Evidência) e Ação Sugerida. Finalize com uma lista clara contendo as 3 prioridades mais urgentes para a liderança.

Restrições:
* Use apenas os dados fornecidos.
* Não invente números, causas, nomes ou conclusões.
* Não exponha dados pessoais ou sensíveis. Oculte e substitua por [DADO SENSÍVEL] qualquer menção a NIF/CPF, nome, número da conta, morada ou valor exato do rendimento.
* Informe claramente as limitações quando os dados não forem suficientes para tirar uma conclusão.
* Use linguagem executiva, simples, direta e voltada para a tomada de decisão.


