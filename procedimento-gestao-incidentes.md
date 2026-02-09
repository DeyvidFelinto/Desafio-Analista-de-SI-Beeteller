# Procedimento de Resposta a Incidentes de Segurança (CSIRT)

## 1. Objetivo
Estabelecer o protocolo oficial para detecção, contenção, erradicação e recuperação de incidentes cibernéticos, garantindo a conformidade com a **Resolução BCB nº 4.893**, **LGPD** e **PCI DSS v4.0**, minimizando impactos financeiros e reputacionais.

## 2. Escopo
Este procedimento é padrão para todos os colaboradores, fornecedores e terceiros conectados à infraestrutura da Instituição.

## 3. Papéis e Responsabilidades (CSIRT)
* **Primeiro Respondente:** Service Desk/SOC - Responsável pela triagem inicial.
* **Analista de Resposta:** Segurança da Informação - Responsável pela contenção técnica.
* **Sala de Crise:** Diretoria + Jurídico + DPO - Irá decidir sobre a comunicação e a continuidade das operações.
* **DPO:** O encarregado da proteção de dados faz comunicação com a ANPD e Titulares.

## 4. Fluxo de Tratamento (Ciclo de Vida)

### 4.1. Detecção e Triagem
* **Canais de Denúncia:** SIEM, E-mail de Segurança, Service Desk.
* **SLA de Triagem:** Todo alerta crítico deve ser analisado no menor tempo possível.

### 4.2. Classificação de Severidade (Matriz de Risco)
Todo incidente deve ser classificado imediatamente para definir o SLA de Resposta:

| Nível | Descrição | Exemplo | SLA de Resposta |
| :--- | :--- | :--- | :--- |
| **P1 - Crítico** | Parada de Negócio, Vazamento de Dados Sensíveis ou Ransomware. | Servidor criptografado, Vazamento de base de CPF. | **Imediato** (Acionar Comitê) |
| **P2 - Alto** | Degradação de serviço ou infecção contida. | Malware em 1 estação, Phishing direcionado. | **Menor que 2 Horas** |
| **P3 - Médio** | Evento suspeito sem impacto confirmado. | Falha de login recorrente, varredura de porta. | **Menor que 24 Horas** |
| **P4 - Baixo** | Desvio de política ou falso positivo. | Instalação de software não autorizado. | **Menor que 48 Horas** |

### 4.3. Contenção e Erradicação
* **Ação Prioritária:** Isolar o ativo afetado da rede para impedir qualquer tipo de movimentação.
* **Preservação de Evidências:** É proibido desligar ou reiniciar equipamentos comprometidos antes da coleta de logs e memória volátil.

### 4.4. Comunicação Regulatória

1.  **Banco Central:** Notificar a ocorrência de incidentes que afetem a prestação de serviços ou sigilo de dados (Conforme Res. BCB 4.893).
2.  **ANPD (Via DPO):** Notificar em "prazo razoável" caso envolva dados pessoais com risco aos titulares.
3.  **Bandeiras (Visa/Master):** Notificar imediatamente em caso de comprometimento de dados de cartão (CDE).

### 4.5. Pós-Incidente
* Após o encerramento, o CSIRT deve produzir o **Relatório de Causa Raiz (RCA)** em até 5 dias úteis.
* O relatório deve conter: Linha do tempo, falha explorada, impacto financeiro e plano de ação para evitar reincidência.

## 5. Referências
* **NIST SP 800-61r2** (Computer Security Incident Handling Guide)
* **PCI DSS v4.0** – Requisito 12.10 (Plano de Resposta a Incidentes)
* **Resolução BCB 4.893/2021** – Art. 21 (Política de Resposta a Incidentes)
