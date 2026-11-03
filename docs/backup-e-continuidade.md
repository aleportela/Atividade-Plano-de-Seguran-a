# Backup, continuidade e recuperação

## 1. Objetivo

Garantir que a escola consiga recuperar dados e serviços após falha, erro humano, ataque, roubo ou desastre físico. A estratégia deve contemplar data center, sistemas administrativos, arquivos institucionais, configurações de rede e serviços hospedados por terceiros.

## 2. Padrão mínimo recomendado

- Adotar a regra **3-2-1**: pelo menos três cópias dos dados, em dois tipos de mídia/ambientes, com uma cópia isolada ou imutável.
- Criptografar backups com dados pessoais ou confidenciais.
- Guardar chaves separadamente e restringir quem pode excluir ou alterar cópias.
- Executar cópias frequentes conforme criticidade, verificar resultados e gerar alertas em caso de falha.
- Manter cópia offline ou imutável, com credenciais diferentes das usadas no ambiente de produção.
- Testar restauração de arquivos e sistemas pelo menos trimestralmente, registrando duração, integridade e problemas.
- Incluir bancos de dados, máquinas virtuais, arquivos compartilhados, configurações de rede, identidade e documentação técnica.
- Definir com fornecedores como solicitar restauração, exportar dados e recuperar o serviço.

## 3. Metas iniciais de recuperação — sujeitas à aprovação

**RTO** é o tempo-alvo para retomar o serviço. **RPO** é a perda máxima de dados medida em tempo. Os valores são metas sugeridas e devem ser ajustados após análise de impacto, capacidade, custo e contratos.

| Serviço / informação | RTO sugerido | RPO sugerido | Observação |
|---|---:|---:|---|
| Sistema acadêmico e base de alunos | Até 8 horas | Até 4 horas | Validar com fornecedor e calendário escolar |
| Sistema administrativo/financeiro | Até 8 horas | Até 4 horas | Considerar períodos de fechamento e folha |
| Arquivos institucionais | Até 24 horas | Até 24 horas | Separar pastas críticas |
| Site institucional | Até 8 horas | Até 24 horas | Dependente da hospedagem |
| Aplicativo institucional | Até 8 horas | Até 4 horas | Depende da arquitetura e contrato |
| Imagem padrão dos laboratórios | Até 48 horas | Conforme ciclo | Reinstalação padronizada pode ser preferível |

## 4. Continuidade das atividades escolares

- Preparar procedimentos manuais temporários para frequência, comunicação com responsáveis, matrícula e registros urgentes.
- Definir canais alternativos oficiais para comunicação com famílias e equipes.
- Manter contatos atualizados de fornecedores, internet, energia, suporte, Direção, TI e privacidade.
- Realizar ao menos um exercício anual de indisponibilidade de sistema ou perda de acesso ao data center.
- Após a recuperação, reconciliar lançamentos manuais e registrar correções.

## 5. Evidências e acompanhamento

Manter registro dos trabalhos de backup, falhas e correções, cópias protegidas, testes de restauração, tempo de recuperação e problemas identificados. O indicador inicial sugerido é concluir 95% ou mais dos trabalhos previstos, com falhas tratadas, e executar ao menos um teste por trimestre e um teste anual ampliado.
