# Checklist Cruzado | Matriz de Aderência

## Contexto

Este documento apresenta uma matriz de aderência entre os requisitos da **ISO/IEC 27001:2022**, da **Resolução BCB nº 4.893/2021** e do **PCI DSS v4.0**, considerando um ambiente fictício de uma Instituição de Pagamento regulada pelo Banco Central do Brasil.

A análise tem como objetivo identificar pontos em comum entre as normas, bem como avaliar o nível de aderência do ambiente analisado. Esse diagnóstico serve como base para a definição de ações de melhoria, priorização de riscos e fortalecimento do Sistema de Gestão de Segurança da Informação (SGSI).

---

## Matriz de Aderência

| Domínio / Controle | ISO/IEC 27001 | BCB 4.893 | PCI DSS 4.0 | Status | Observações (Gap Analysis) |
| :--- | :--- | :--- | :--- | :---: | :--- |
| **Gestão de Riscos (GRC)** | Cláusula 6.1 | Art. 6º | Req. 12.2 | 🟡 | Existe metodologia, mas falta alinhamento com a nova *Política de Gestão Integrada de Riscos* e revisão trimestral. |
| **Política de Segurança** | Cláusula 5.2 | Art. 4º | Req. 12.1 | 🟢 | Política aprovada pela diretoria e comunicada aos colaboradores. |
| **Gestão de Acessos & MFA** | A.9.2 / A.9.4 | Art. 8º / 16 | Req. 8.4.2 | 🟡 | Falta implementar **MFA** para todos os acessos administrativos ao CDE (Requisito crítico PCI v4.0). |
| **Gestão de Vulnerabilidades** | A.8.8 | Art. 15 | Req. 11.3 | 🔴 | Scans de vulnerabilidade não são realizados trimestralmente. Risco alto de exploração de falhas. |
| **Resposta a Incidentes** | A.5.24 | Art. 9º / 21 | Req. 12.10 | 🔴 | Processo reativo. Ausência de plano de resposta formalizado e testado para cenários de Ransomware. |
| **Continuidade (PCN)** | A.5.30 | Art. 10º | Req. 12.10.1 | 🟡 | Plano existente, mas sem testes periódicos documentados (falha de evidência para auditoria). |
| **Gestão de Terceiros** | A.5.19 | Art. 7º | Req. 12.8 | 🟡 | Avaliação ocorre apenas na contratação. Falta monitoramento contínuo do risco da cadeia de suprimentos. |
| **Conscientização** | A.6.3 | Art. 5º | Req. 12.6 | 🟡 | Treinamentos genéricos. Ausência de campanhas específicas de Phishing simulado e métricas. |
| **Monitoramento (Logs)** | A.8.15 | Art. 11º | Req. 10 | 🟢 | Centralização de logs e trilha de auditoria implementados conforme requisitos de retenção. |
| **Auditoria Interna** | Cláusula 9.2 | Art. 12º | Req. 12.11 | 🟡 | Auditorias sem cronograma fixo. Necessário formalizar para atender ao ciclo anual regulatório. |

<br>

<div align="center">
  <b>Legenda de Status:</b> &nbsp;&nbsp;
  🟢 Aderente &nbsp;|&nbsp;
  🟡 Parcial &nbsp;|&nbsp;
  🔴 Não Aderente (Risco Crítico)
</div>

---
**Nota:**  
O ambiente descrito é fictício e utilizado exclusivamente para fins avaliativos.
