# Plano de Ação Priorizado

## Analista de Segurança da Informação (Conformidade e Governança)

---

## Contexto

Este plano de ação foi elaborado a partir dos **pontos de atenção** identificados na Matriz de Aderência. O cenário considera um ambiente simulado de uma Instituição de Pagamento, com foco no alinhamento à **Resolução BCB nº 4.893/2021** e no aprimoramento dos controles de Segurança da Informação já existentes, baseados na **ISO/IEC 27001**.

As ações propostas buscam tratar os **gaps** de conformidade identificados e fortalecer a capacidade da instituição de prevenir, detectar e responder a incidentes de segurança, considerando tanto requisitos regulatórios quanto impactos no negócio.

---

## Plano de Ação

| Ação | Requisito Associado | Prioridade | Prazo | Responsável | Risco Mitigado (Impacto no Negócio) |
| :--- | :--- | :--- | :--- | :--- | :--- |
| Aprimorar o processo de resposta a incidentes, com apoio de automação | ISO 27001 A.5.24 / BCB 4.893 Art. 21 / PCI DSS 12.10 | **Alta** | 30 dias | Segurança da Informação / GRC | Atrasos na resposta a incidentes podem causar indisponibilidade de serviços financeiros (ex.: Pix) e gerar sanções regulatórias. |
| Realizar varreduras periódicas de vulnerabilidades | PCI DSS 11.3.1 / BCB 4.893 Art. 15 | **Alta** | 30 dias | Segurança da Informação | Falhas não identificadas aumentam o risco de ataques como ransomware e exploração de sistemas. |
| Implementar autenticação multifator (MFA) e revisar acessos administrativos | ISO 27001 A.9.2 / PCI DSS 8.4.2 | **Alta** | 45 dias | Infraestrutura / Gestão de Acessos | Redução do risco de uso indevido de credenciais e acessos não autorizados a sistemas críticos. |
| Revisar a metodologia de gestão de riscos conforme a política corporativa vigente | ISO 27001 6.1 / BCB 4.893 Art. 6º / PCI DSS 12.2 | **Alta** | 60 dias | Compliance / Riscos | Riscos mal avaliados podem impactar decisões estratégicas e a continuidade do negócio. |
| Formalizar a avaliação de segurança de fornecedores | ISO 27001 A.5.19 / BCB 4.893 Art. 30 | **Média** | 90 dias | Compras / GRC | Riscos introduzidos por terceiros podem comprometer dados, sistemas e a operação da instituição. |
| Estruturar ações de conscientização sobre phishing e engenharia social | ISO 27001 A.6.3 / PCI DSS 12.6 | **Média** | 90 dias | RH / GRC | Usuários despreparados aumentam a probabilidade de incidentes causados por ataques de engenharia social. |
| Validar e testar o Plano de Continuidade de Negócios (PCN) | ISO 27001 A.5.30 / BCB 4.893 Art. 10º | **Média** | 90 dias | Continuidade / TI | Falta de testes pode comprometer a recuperação da operação em situações de indisponibilidade ou desastre. |

---

**Nota:**  
Os prazos foram definidos considerando a complexidade na sua implementação em um ambiente crítico, priorizando ações de maior impacto e de rápida execução, como a implementação de MFA e a revisão de acessos.
