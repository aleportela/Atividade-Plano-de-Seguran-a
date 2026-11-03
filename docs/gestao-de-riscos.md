# Gestão de riscos

## 1. Método de avaliação

A avaliação inicial considera probabilidade e impacto, ambos pontuados de 1 a 5. O nível de risco é o produto dos dois valores:

**Risco = Probabilidade × Impacto**

A classificação é uma referência inicial e deve ser calibrada após o inventário e o diagnóstico técnico.

| Pontuação | Nível | Tratamento recomendado |
|---:|---|---|
| 1 a 4 | Baixo | Manter controles e revisar periodicamente |
| 5 a 9 | Moderado | Definir responsável e ação de melhoria |
| 10 a 16 | Alto | Plano de tratamento com prioridade e prazo curto |
| 17 a 25 | Crítico | Ação imediata, escalonamento à Direção e avaliação de interrupção segura do serviço |

## 2. Riscos prioritários iniciais — a validar

| Risco | Impacto potencial | Prioridade inicial | Ação-chave |
|---|---|---|---|
| Ransomware ou malware | Perda de dados, paralisação e possível vazamento | Crítica | EDR/antimalware, atualização, segmentação, privilégio mínimo e backup isolado testado |
| Acesso indevido a dados de alunos | Exposição de notas, dados cadastrais, documentos ou saúde | Crítica | MFA, revisão de acessos, logs, classificação e controle de compartilhamento |
| Conta de professor/funcionário comprometida | Fraude, exposição de dados ou alteração de registros | Alta | MFA, proteção de e-mail, treinamento e redefinição segura de credenciais |
| Indisponibilidade do data center ou internet | Interrupção de sistemas acadêmicos, administrativos e comunicação | Alta | UPS, contratos, backups e plano manual de contingência |
| Ataque a site/aplicativo/fornecedor | Exposição de dados, interrupção e dependência de terceiro | Alta | Avaliação contratual, controle de acesso, testes e plano de saída |
| Perda ou roubo de notebook | Acesso a arquivos locais, e-mail e sistemas | Alta | Criptografia de disco, bloqueio, inventário, gestão remota e reporte imediato |
| Pendrive ou Wi-Fi não autorizado | Infecção ou entrada indevida na rede interna | Moderada/Alta | Política de mídia removível, segmentação e controle de rede sem fio |

## 3. Tratamento de cada risco

Para cada risco identificado, manter registro com:
- Ativo, processo ou serviço afetado.
- Evento de risco e causas prováveis.
- Probabilidade e impacto, com justificativa.
- Prioridade e responsável.
- Medidas de tratamento e prazo.
- Evidência de conclusão.
- Risco residual e decisão formal da Direção, quando aplicável.

## 4. Revisão

A TI deve revisar riscos e controles em conjunto com as áreas responsáveis. O Comitê de Segurança e Privacidade deve revisar o registro trimestralmente e após incidentes graves, mudanças de fornecedor ou alterações relevantes na infraestrutura.
