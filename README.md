# Plano de Segurança da Informação — Ambiente Escolar

> **Atividade acadêmica | Minuta técnica | Versão de referência: 1.0 — 03/11/2026**

Este repositório organiza o plano de segurança da informação proposto para uma instituição de ensino com aproximadamente **2.200 alunos**, professores, funcionários e responsáveis. A proposta considera a infraestrutura informada: data center local, site hospedado por fornecedor, aplicativo institucional, estações Windows e rede escolar.

<details>
<summary><strong>Visão geral do ambiente considerado</strong></summary>

| Elemento | Contexto informado |
|---|---|
| Comunidade escolar | Aproximadamente 2.200 alunos |
| Laboratórios | 3 laboratórios, com 30 máquinas cada |
| Computadores nos laboratórios | 90 |
| Parque adicional | Desktops e notebooks, quantidade ainda a levantar |
| Servidores | Data center local (on-premise) |
| Serviços externos | Site com hospedagem contratada e aplicativo institucional |
| Sistema operacional | Ambiente Windows |
| Outros espaços | Sala de reunião identificada no levantamento inicial |

</details>

## Sobre o projeto

O objetivo é estabelecer diretrizes para proteger as informações acadêmicas, administrativas e operacionais, reduzir a possibilidade de incidentes e orientar a continuidade dos serviços escolares.

O plano está organizado em seis frentes: **governar, identificar, proteger, detectar, responder e recuperar**, seguindo a estrutura do NIST Cybersecurity Framework 2.0 e considerando as obrigações aplicáveis da LGPD, especialmente no tratamento de dados de crianças e adolescentes.

## Navegação

| Documento | Conteúdo |
|---|---|
| [Plano de Segurança da Informação](docs/plano-de-seguranca.md) | Documento principal, objetivos, escopo, governança, riscos, controles e implantação |
| [Ambiente e inventário](docs/ambiente-e-inventario.md) | Ativos conhecidos, lacunas de informação e modelo de inventário |
| [Gestão de riscos](docs/gestao-de-riscos.md) | Método de avaliação, matriz inicial e tratamento dos riscos |
| [Política e responsabilidades](docs/politica-e-responsabilidades.md) | Papéis, regras de uso, acesso e governança |
| [Controles técnicos](docs/controles-tecnicos.md) | Identidades, estações, rede, data center, site, aplicativo e segurança física |
| [Backup e continuidade](docs/backup-e-continuidade.md) | Cópias de segurança, RTO, RPO e retomada dos serviços |
| [Resposta a incidentes](docs/resposta-a-incidentes.md) | Fluxo de resposta, severidade, comunicação e registro |
| [Cronograma e indicadores](docs/cronograma.md) | Etapas de implantação, evidências e acompanhamento |
| [Modelos e registros](docs/modelos-e-registros.md) | Checklists, ficha de incidente e campos para formalização |
| [Referências](REFERENCIAS.md) | Bases legais e técnicas utilizadas |

## Como ler este plano

Este material é uma **minuta para validação da Direção e da equipe de TI**. Os dados de contexto vieram das informações fornecidas para a atividade e do levantamento inicial. Recomendações como MFA, criptografia, segmentação de rede, backup imutável e monitoramento **não significam que esses controles já estejam implantados**.

Nenhuma medida deve ser marcada como concluída sem evidência, como configuração validada, registro, teste, contrato ou procedimento aprovado.

## Situação do projeto

- [x] Estrutura inicial do repositório
- [x] Documentação organizada por assunto
- [x] Plano principal alinhado ao documento de referência
- [ ] Validação dos dados reais do ambiente pela instituição
- [ ] Aprovação formal da Direção
- [ ] Definição dos responsáveis e canais institucionais
- [ ] Diagnóstico técnico e priorização final
- [ ] Inclusão do documento final em PDF — **reservada para a etapa posterior**

## Referência do documento principal

A versão de referência para a futura inclusão do documento final é o arquivo enviado em formato DOCX, denominado **Plano_de_Seguranca_da_Informacao_Escola(1).docx**. O arquivo não foi incluído neste repositório nesta etapa; a inclusão do documento em PDF ficará para depois, conforme combinado.
