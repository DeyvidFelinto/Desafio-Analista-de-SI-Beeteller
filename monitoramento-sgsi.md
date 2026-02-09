# Mecanismos de Monitoramento Contínuo (KPIs & KRIs)

## Contexto Estratégico

A efetividade do SGSI não se mede pela quantidade de documentos, mas pela capacidade de resposta a incidentes e pela aderência contínua aos controles.

Esta proposta define o **Painel de Indicadores** que será apresentado mensalmente ao Comitê de Risco e à Diretoria, visando dar visibilidade sobre a maturidade do ambiente frente à **ISO 27001**, **PCI DSS 4.0** e ao novo prazo regulatório do **Bacen (Março/2026)**.

---

## 1. Indicadores de Desempenho (KPIs) - Operacional

| Indicador (KPI) | Meta Definida (SLA) | Frequência | Fonte de Dados |
| :--- | :--- | :--- | :--- |
| **Cobertura de Patching** | > 95% dos ativos críticos atualizados em até 7 dias | Mensal | Ferramenta de Scan |
| **Efetividade do MFA** | 100% dos acessos remotos e admin com duplo fator ativo | Contínua | IdP / Active Directory |
| **Tempo de Resposta** | Incidentes de Alta Criticidade contidos em < 4 horas | Mensal | Ferramenta de Service Desk |
| **Conscientização (Phishing)** | < 5% de taxa de cliques em testes simulados | Trimestral | Plataforma de Treinamento |

---

## 2. Indicadores de Risco (KRIs) - Tático/Estratégico

| Indicador de Risco (KRI) | Limite de Tolerância (Threshold) | Ação em caso de Desvio |
| :--- | :--- | :--- |
| **Exposição na Dark Web** | **Zero** credenciais de VIPs/Admins expostas | Redefinição forçada de senha imediata e análise forense. |
| **Shadow IT** | < 3 Aplicações não homologadas detectadas na rede | Bloqueio via Proxy/Firewall e notificação ao gestor. |
| **Risco de Terceiros** | 100% com avaliação vigente | Bloqueio de pagamentos ou acesso até regularização. |
| **Débito Regulatório (Bacen)** | 100% dos controles da Res. 4.893 implementados até Fev/2026 | Convocação de Comitê Extraordinário de Crise. |

---

## 3. Estrutura do Reporte

Garantir a transparência exigida pela **Resolução BCB 4.893 (Art. 12)**, realizar um reporte mensal:

### 🚦 Painel de Conformidade Regulatória (Data limite: 01/03/2026).

* **Status Geral:** 🟡 EM ATENÇÃO
* **Aderência ISO 27001:** 85% (🟢 Estável)
* **Aderência PCI DSS 4.0:** 70% (🟡 Atenção: Foco no Req 8.4.2 - MFA)
* **Novas Resoluções (CMN 5.274):** 40% (🔴 Crítico: Necessário investimento em Threat Intel (Monitorar a Dark Web)

### 🚨 Top 3 Focos de Atenção
1.  **Vulnerabilidades:** Falta de scans automatizados (Plano de ação em andamento).
2.  **Identidade:** Acessos administrativos sem MFA (Mitigação prevista para 30 dias).
3.  **Monitoramento:** Monitorar vazamentos na Deep Web (Risco de Fraude).

---

## 4. Rituais de Governança

* **Mensal:** Reunião do Comitê de Segurança para apresentação dos KPIs.
* **Trimestral:** Revisão de Acessos.
* **Semestral:** Teste de Mesa do Plano de Continuidade de Negócios (PCN).
* **Anual:** Auditoria Externa e Pentest (Blackbox/Greybox).

---

**Nota:**  

O ambiente descrito é fictício e utilizado exclusivamente para fins avaliativos.
