# Plano de Segurança da Informação

**Ambiente escolar | Versão 1.0 — Minuta técnica | 03 de novembro de 2026**  
**Classificação prevista no documento institucional:** uso interno — documento sujeito à validação da Direção e da equipe de TI.

> Este plano é uma proposta de diretrizes. A instituição deve confirmar o inventário, nomear os responsáveis, validar os riscos e aprovar as medidas antes de tratá-las como implantadas.

## Controle do documento

| Campo | Definição |
|---|---|
| Responsável institucional | Direção / mantenedora da escola — a confirmar formalmente |
| Responsável operacional | Coordenação de TI — nomear responsável e substituto |
| Encarregado / privacidade | Indicar o encarregado, quando aplicável, e publicar canal para titulares e responsáveis |
| Aprovação | Direção: __________________________ Data: ____/____/______ |
| Próxima revisão | Até 12 meses após a aprovação, ou antes em caso de incidente ou mudança relevante |
| Abrangência | Alunos, responsáveis, professores, funcionários, prestadores e terceiros com acesso a sistemas ou dados |

## 1. Resumo executivo

A escola mantém informações acadêmicas, administrativas e operacionais de uma comunidade de aproximadamente **2.200 alunos**, além de professores, funcionários e responsáveis. O ambiente considerado inclui data center local, site com hospedagem contratada, aplicativo institucional, três laboratórios com 30 computadores cada (90 máquinas) e um parque adicional de desktops e notebooks, cujo quantitativo ainda precisa ser levantado. O levantamento inicial também indica ambiente Windows e sala de reunião.

O plano busca reduzir a probabilidade e o impacto de incidentes como ransomware, vazamento de dados de alunos, fraude por e-mail, indisponibilidade de sistemas acadêmicos, perda de arquivos, acesso indevido por contas compartilhadas e comprometimento de fornecedores. A proteção precisa envolver tecnologia, processos e pessoas.

A proposta está organizada em seis frentes contínuas, alinhadas ao NIST Cybersecurity Framework 2.0: **governar, identificar, proteger, detectar, responder e recuperar**. A adequação à LGPD deve considerar especialmente o tratamento de dados de crianças e adolescentes.

### Prioridades executivas

1. **Conhecer o ambiente:** inventariar computadores, servidores, softwares, contas, dados, redes, contratos e responsáveis.
2. **Controlar identidades:** adotar contas individuais, privilégio mínimo, revisão de acessos e MFA em acessos críticos.
3. **Proteger o que é essencial:** atualizar Windows e servidores, proteger endpoints, segmentar redes e restringir o acesso ao data center.
4. **Garantir recuperação:** manter backups criptografados e isolados, testar restaurações e documentar prioridades de retomada.
5. **Preparar a resposta:** criar canal de reporte, equipe de crise, registro de incidentes e fluxo de avaliação de comunicação à ANPD e aos titulares.

**Decisão solicitada à Direção:** aprovar este plano como diretriz institucional, nomear responsáveis, autorizar o inventário e o diagnóstico técnico inicial e priorizar as ações dos primeiros 90 dias.

## 2. Objetivo, princípios e resultados esperados

O plano busca preservar a confidencialidade, a integridade e a disponibilidade das informações e dos serviços utilizados pela escola, sem prejudicar as atividades pedagógicas. A segurança deve ser proporcional ao risco, simples de operar e compatível com a rotina escolar.

- **Confidencialidade:** somente pessoas autorizadas acessam as informações necessárias à sua função.
- **Integridade:** registros acadêmicos, financeiros e administrativos devem permanecer corretos, completos e protegidos contra alteração indevida.
- **Disponibilidade:** sistemas e dados devem poder ser utilizados quando necessários, com procedimentos de contingência.
- **Necessidade e minimização:** coletar e compartilhar apenas os dados necessários para cada finalidade.
- **Responsabilização:** decisões, acessos, alterações e incidentes devem ser rastreáveis e documentados.
- **Melhoria contínua:** medir resultados, corrigir falhas e revisar controles periodicamente.

## 3. Contexto e escopo

O escopo abrange ativos e processos físicos e digitais que armazenam, processam, transmitem ou dão suporte às informações da escola, estejam nas dependências da instituição ou sob responsabilidade de fornecedor.

| Elemento | Informação conhecida | Tratamento previsto |
|---|---|---|
| Alunos | 2.200 alunos | Prioridade elevada para privacidade, disponibilidade acadêmica e dados de menores |
| Professores e funcionários | Existem; quantitativos não informados | Levantar número de pessoas, funções, vínculos e perfis de acesso |
| Laboratórios | 3 laboratórios, 30 máquinas cada | Considerar os 90 computadores e separar a rede dos laboratórios da rede administrativa e dos servidores |
| Parque de computadores | Desktops e notebooks além dos laboratórios | Inventariar quantidade, localização, usuário, sistema, garantia e suporte |
| Data center | Local / on-premise | Avaliar acesso físico, energia, climatização, incêndio, backups, rede, logs e atualizações |
| Site | Hospedagem contratada | Revisar contrato, responsabilidades, autenticação administrativa, backups, logs e incidentes |
| Aplicativo | Aplicativo institucional mencionado | Mapear dados, integrações, fornecedor, permissões, notificações e atualizações |
| Sistema operacional | Windows | Identificar versões e garantir que estejam em suporte e recebam atualizações |
| Sala de reunião | Ambiente físico identificado no levantamento inicial | Avaliar tela, computador, videoconferência, rede sem fio e exposição de documentos |

### Limites conhecidos

Ainda não há confirmação sobre quantidade e versão dos servidores, topologia de rede, firewall, Wi-Fi, provedor de internet, diretório de usuários, e-mail, sistemas acadêmicos e financeiros, fornecedor do aplicativo, controles atuais de backup, antivírus/EDR, VPN e monitoramento. Esses itens devem ser levantados no diagnóstico.

### 3.1. Sistemas e processos prioritários

- **Gestão acadêmica:** matrícula, cadastro, frequência, notas, histórico, turmas, avaliações e comunicação com responsáveis.
- **Gestão administrativa e financeira:** contratos, cobrança, folha, dados bancários, compras e documentos institucionais.
- **Identidade e comunicação:** contas de e-mail, diretório, portal, aplicativo, site e ferramentas de colaboração.
- **Infraestrutura e ensino:** servidores, rede, internet, laboratórios, desktops, notebooks e sala de reunião.
- **Serviços contratados:** hospedagem do site, aplicativo, sistemas em nuvem, suporte técnico, armazenamento e conectividade.

### 3.2. Premissas de implantação

- A escola designará um responsável institucional e um responsável técnico, com substituto e segregação de aprovações críticas.
- A implantação será feita em etapas, avaliando o impacto nas aulas e nos períodos de matrícula, provas e fechamento de notas.
- Nenhum controle será considerado implantado sem evidência: configuração, registro, teste, contrato ou procedimento aprovado.

## 4. Governança e responsabilidades

A Direção deve patrocinar o programa e aprovar políticas, orçamento, prioridades e aceitação de riscos. A equipe de TI implementa e opera os controles. As áreas pedagógica e administrativa validam necessidades de acesso e ajudam a proteger os dados sob sua responsabilidade.

| Papel | Responsabilidades principais |
|---|---|
| Direção / mantenedora | Aprovar o plano e as políticas; definir orçamento; nomear responsáveis; decidir sobre riscos relevantes; apoiar resposta a incidentes e continuidade |
| Coordenação de TI | Manter inventário; administrar identidades e equipamentos; aplicar atualizações; monitorar alertas; gerir backups; documentar mudanças; coordenar resposta técnica |
| Encarregado / privacidade e jurídico | Orientar sobre LGPD; manter canal com titulares; apoiar análise de risco; avaliar comunicações regulatórias com o controlador |
| Coordenações pedagógica e administrativa | Solicitar e aprovar acessos; revisar permissões; comunicar mudanças de função; classificar informações e orientar equipes |
| Professores e funcionários | Usar contas individuais; proteger credenciais; tratar dados conforme orientação; reportar suspeitas imediatamente; participar de treinamentos |
| Alunos e responsáveis | Usar recursos digitais de forma responsável; não compartilhar credenciais; comunicar suspeitas pelos canais indicados |
| Fornecedores e prestadores | Cumprir requisitos contratuais; limitar acessos; manter registros; proteger dados; notificar incidentes rapidamente; devolver ou eliminar dados ao fim do contrato |

### 4.1. Regras de governança

- Criar um Comitê de Segurança e Privacidade com Direção, TI e representante administrativo ou pedagógico. Reunir-se trimestralmente e após incidentes graves.
- Manter registro de riscos, decisões, exceções, mudanças relevantes, incidentes, treinamentos e testes de recuperação.
- Toda conta administrativa, acesso remoto, contratação de sistema ou compartilhamento externo de dados deve ter responsável e justificativa.
- Exceções aos controles devem ter prazo de validade, justificativa, responsável aprovador e medida compensatória.

### 4.2. Documentos complementares a aprovar

- Política de Segurança da Informação e Uso Aceitável.
- Política de Controle de Acesso e Gestão de Senhas.
- Política de Backup, Retenção e Restauração.
- Procedimento de Resposta a Incidentes e Comunicação de Crise.
- Aviso de Privacidade, registro de operações de tratamento e regras para fornecedores.
- Termos de responsabilidade e confidencialidade para colaboradores e prestadores.

## 5. Classificação da informação e avaliação de riscos

A escola deve classificar informações conforme o impacto de sua exposição, alteração ou indisponibilidade. A classificação orienta armazenamento, compartilhamento, retenção e descarte.

| Classe | Exemplos | Regras mínimas |
|---|---|---|
| Pública | Informações institucionais aprovadas para divulgação, calendário público e comunicados | Revisar conteúdo antes de publicar; evitar expor dados pessoais desnecessários |
| Interna | Procedimentos, documentos operacionais e comunicados internos | Acesso a colaboradores autorizados; compartilhamento por canais institucionais |
| Confidencial | Dados de matrícula, notas, frequência, contratos, folha e contatos de responsáveis | Acesso por função; armazenamento institucional; criptografia quando disponível; registro de compartilhamento |
| Restrita / sensível | Dados de saúde, deficiência, biometria, medidas disciplinares, credenciais e documentos de identificação | Acesso estritamente necessário; MFA em sistemas críticos; criptografia; logs; compartilhamento excepcional e documentado |

### 5.1. Método de priorização

Atribuir probabilidade e impacto de 1 a 5. O nível de risco é o produto dos dois valores. A classificação é uma referência inicial e deve ser calibrada após o inventário e o diagnóstico.

| Pontuação | Nível | Tratamento recomendado |
|---:|---|---|
| 1 a 4 | Baixo | Manter controles e revisar periodicamente |
| 5 a 9 | Moderado | Definir responsável e ação de melhoria |
| 10 a 16 | Alto | Plano de tratamento com prioridade e prazo curto |
| 17 a 25 | Crítico | Ação imediata, escalonamento à Direção e avaliação de interrupção segura do serviço |

Os riscos iniciais e suas ações-chave estão detalhados em [Gestão de riscos](gestao-de-riscos.md).

## 6. Controles de segurança — identidades, acessos e estações

### 6.1. Contas e autenticação

- Cada pessoa deve utilizar conta individual. É proibido compartilhar senhas ou utilizar conta genérica para atividades administrativas.
- Conceder apenas permissões necessárias à função. Professores, alunos, secretaria, financeiro, TI e fornecedores devem ter perfis separados.
- Ativar MFA para administradores, acesso remoto, e-mail institucional, painel de hospedagem, nuvem e sistemas com dados pessoais, sempre que suportado.
- Criar procedimento de admissão, mudança de função e desligamento: solicitação aprovada, concessão, revisão e revogação de acessos no mesmo dia do desligamento ou conforme o risco.
- Contas privilegiadas devem ser separadas das contas comuns. Utilizar senha forte e gerenciador institucional; nunca enviar credenciais em grupos ou planilhas abertas.
- Revisar mensalmente contas administrativas e trimestralmente acessos aos sistemas críticos. Desabilitar contas sem uso e acessos de fornecedores ao fim do serviço.

### 6.2. Computadores Windows, desktops e notebooks

- Inventariar hostname, número patrimonial ou serial, localização, responsável, versão do Windows, data de atualização, software instalado e situação do suporte.
- Manter sistemas operacionais e aplicativos em versões suportadas, com atualizações automáticas e correções de segurança.
- Utilizar solução antimalware/EDR centralizada, com proteção em tempo real e alertas enviados à TI.
- Remover privilégios de administrador local de usuários comuns. A instalação de programas deve ser controlada pela TI.
- Ativar criptografia de disco nos notebooks e equipamentos que armazenem dados confidenciais, com chaves guardadas de forma segura.
- Configurar bloqueio automático de tela, senha/PIN, firewall local e inicialização segura quando compatíveis.
- Controlar instalação e execução de programas; restringir mídias USB conforme necessidade pedagógica.
- Nos laboratórios, utilizar contas de aluno com permissões limitadas, separar dados de usuários e restaurar computadores conforme rotina aprovada.

### 6.3. E-mail, navegação e colaboração

- Ativar filtragem antiphishing/antispam e proteção contra anexos e links maliciosos; configurar SPF, DKIM e DMARC no domínio.
- Não encaminhar dados pessoais de alunos para contas pessoais. Usar armazenamento institucional com permissões explícitas e prazo de validade.
- Confirmar por canal independente pedidos urgentes de pagamento, alteração bancária, envio de lista de alunos ou redefinição de senha.
- Restringir encaminhamento automático para e-mails externos e revisar regras suspeitas de caixa postal.

## 7. Controles de segurança — rede, data center e serviços externos

### 7.1. Segmentação da rede

A arquitetura deve evitar que um equipamento comprometido em um laboratório alcance livremente servidores, financeiro, secretaria ou equipamentos de gestão. A TI deve documentar topologia, endereços, VLANs, regras de firewall e dependências.

| Zona sugerida | Finalidade | Regra de comunicação |
|---|---|---|
| Administrativa | Secretaria, financeiro, direção e apoio | Acesso apenas a sistemas e impressoras necessários |
| Pedagógica / professores | Computadores e recursos docentes | Acesso aos sistemas pedagógicos autorizados |
| Laboratórios de alunos | 90 computadores dos três laboratórios | Internet e recursos pedagógicos aprovados; bloquear acesso a servidores e painéis administrativos |
| Servidores / data center | Servidores, armazenamento, virtualização e backup | Acesso somente de sistemas e administradores autorizados |
| Convidados / BYOD | Visitantes e dispositivos pessoais | Somente internet; isolamento da rede interna |
| Gerenciamento | Firewall, switches, Wi-Fi e monitoramento | Acesso exclusivo de TI, com MFA e logs |

Medidas recomendadas:

- Configurar firewall de borda com regras explícitas e revisão semestral.
- Utilizar Wi-Fi corporativo com autenticação adequada e rede de visitantes separada. Não conectar roteadores pessoais ou pontos de acesso não autorizados.
- Desativar serviços, portas e protocolos inseguros desnecessários. Monitorar alterações de configuração e manter cópias seguras.
- Acesso remoto administrativo somente por VPN ou solução segura equivalente, com MFA e registro. Não expor RDP ou painéis administrativos diretamente à internet.

### 7.2. Data center local (on-premise)

- Restringir acesso físico à sala de servidores por chave controlada ou controle eletrônico; registrar visitantes e acessos técnicos.
- Manter rack trancado, cabeamento identificado, detecção/prevenção de incêndio apropriada e proteção contra água, poeira e calor.
- Avaliar UPS/nobreak, aterramento, energia, climatização e procedimento de desligamento seguro. Testar autonomia e manutenção.
- Manter inventário de servidores, sistemas, serviços, contas administrativas, certificados, licenças e datas de suporte.
- Aplicar atualizações em janela controlada, com backup prévio e plano de retorno. Desabilitar contas padrão e serviços desnecessários.
- Enviar logs críticos para repositório central protegido, com horário sincronizado e acesso restrito.
- Não utilizar servidor de produção como única cópia de backup. Separar credenciais e permissões do ambiente de backup.

### 7.3. Site hospedado e aplicativo

- Identificar formalmente fornecedores, suboperadores, localização do armazenamento, integrações, dados coletados e responsáveis.
- Revisar contratos: finalidade, confidencialidade, segurança, controle de acesso, subcontratação, incidentes, retenção, devolução e eliminação.
- Propor obrigação contratual de notificação à escola em até 24 horas após suspeita ou confirmação de incidente relevante. **Esse é prazo interno proposto, não o prazo legal da ANPD.**
- Proteger painéis administrativos com MFA e contas individuais. Atualizar CMS, plugins, bibliotecas e componentes do aplicativo.
- Solicitar evidências de backup, restauração, testes de segurança, atualização e gestão de vulnerabilidades.
- Evitar publicar dados de alunos em páginas abertas, links públicos ou diretórios indexáveis.

## 8. Proteção de dados pessoais e LGPD

A escola deve mapear quais dados pessoais trata, para quais finalidades, com qual fundamento jurídico, por quanto tempo, com quem compartilha e quais controles protegem cada operação. O tratamento de dados de crianças e adolescentes deve observar seu melhor interesse, conforme o art. 14 da LGPD.

### 8.1. Inventário e ciclo de vida dos dados

- Mapear dados de alunos, responsáveis, professores, funcionários, candidatos, visitantes e fornecedores.
- Registrar finalidade, categoria de dados, sistema/local de armazenamento, pessoas com acesso, compartilhamentos, prazo de retenção e descarte.
- Avaliar especialmente dados de saúde, deficiência, biometria, imagens, documentos de identificação, informações financeiras, registros disciplinares e credenciais.
- Definir fundamento jurídico adequado para cada finalidade. Não presumir que consentimento seja a base legal obrigatória para todo tratamento escolar.
- Publicar aviso de privacidade claro para responsáveis, alunos e colaboradores, explicando dados coletados, finalidades, compartilhamentos, direitos e canal de contato.
- Manter processo para atender solicitações de titulares e responsáveis, com validação de identidade e registro.
- Definir prazos de guarda com apoio jurídico/administrativo e eliminar ou anonimizar dados quando não houver justificativa para mantê-los.

### 8.2. Cuidados específicos com crianças e adolescentes

- Tratar dados sempre considerando o melhor interesse do aluno e a necessidade concreta da atividade escolar.
- Disponibilizar informações em linguagem simples e acessível a responsáveis e alunos.
- Controlar listas de turma, notas, frequência, ocorrências, laudos, documentos e contatos de responsáveis.
- Não divulgar fotos, vídeos, voz, trabalhos ou identificação de alunos sem avaliar finalidade, base jurídica, autorizações aplicáveis e regras internas.
- Evitar grupos informais ou dispositivos pessoais para distribuir planilhas, documentos, notas ou dados de saúde.
- Restringir informações de saúde e necessidades específicas às pessoas que realmente precisam delas.

### 8.3. Contratos e compartilhamento

- Formalizar a relação controlador-operador conforme o papel real de cada parte.
- Antes de contratar sistema, avaliar dados coletados, necessidade, riscos, permissões, retenção, exportação e dependência do fornecedor.
- Não compartilhar credenciais ou bases completas quando uma extração reduzida ou acesso temporário resolver a necessidade.
- Avaliar transferências internacionais de dados antes de habilitar serviços com armazenamento ou suporte fora do Brasil.

> **Observação jurídica:** este documento é um plano operacional de segurança e não substitui análise jurídica do tratamento de dados, revisão de contratos, definição de bases legais ou avaliação formal de conformidade com a LGPD.

## 9. Backup, continuidade e recuperação

A escola deve conseguir recuperar dados e serviços após falha, erro humano, ataque, roubo ou desastre físico. A estratégia deve contemplar data center, sistemas administrativos, arquivos institucionais, configurações de rede e serviços hospedados por terceiros.

### 9.1. Padrão mínimo recomendado

- Adotar a regra 3-2-1: pelo menos três cópias dos dados, em dois tipos de mídia/ambientes, com uma cópia isolada ou imutável.
- Criptografar backups com dados pessoais ou confidenciais. Armazenar chaves separadamente e restringir quem pode excluir ou alterar cópias.
- Executar cópias frequentes conforme criticidade, verificar resultados e gerar alertas em caso de falha.
- Manter cópia offline ou imutável, com credenciais diferentes das usadas no ambiente de produção.
- Testar restauração de arquivos e sistemas pelo menos trimestralmente, registrando duração, integridade e problemas.
- Incluir bancos de dados, máquinas virtuais, arquivos compartilhados, configurações de rede, identidade e documentação técnica.
- Definir com fornecedores como solicitar restauração, exportar dados e recuperar o serviço.

### 9.2. Metas iniciais de recuperação — sujeitas à aprovação

RTO é o tempo-alvo para retomar o serviço; RPO é a perda máxima de dados medida em tempo. Os valores são metas sugeridas e devem ser ajustados após análise de impacto, capacidade, custo e contratos.

| Serviço / informação | RTO sugerido | RPO sugerido | Observação |
|---|---:|---:|---|
| Sistema acadêmico e base de alunos | Até 8 horas | Até 4 horas | Validar com fornecedor e calendário escolar |
| Sistema administrativo/financeiro | Até 8 horas | Até 4 horas | Considerar períodos de fechamento e folha |
| Arquivos institucionais | Até 24 horas | Até 24 horas | Separar pastas críticas |
| Site institucional | Até 8 horas | Até 24 horas | Dependente da hospedagem |
| Aplicativo institucional | Até 8 horas | Até 4 horas | Depende da arquitetura e contrato |
| Imagem padrão dos laboratórios | Até 48 horas | Conforme ciclo | Reinstalação padronizada pode ser preferível |

### 9.3. Continuidade das atividades escolares

- Preparar procedimentos manuais temporários para frequência, comunicação com responsáveis, matrícula e registros urgentes.
- Definir canais alternativos oficiais para comunicação com famílias e equipes.
- Manter contatos atualizados de fornecedores, internet, energia, suporte, Direção, TI e privacidade.
- Realizar ao menos um exercício anual de indisponibilidade de sistema ou perda de acesso ao data center.
- Após a recuperação, reconciliar lançamentos manuais e registrar correções.

## 10. Gestão e resposta a incidentes

Incidente é qualquer evento que comprometa ou possa comprometer confidencialidade, integridade ou disponibilidade de dados, sistemas ou serviços. Suspeitas devem ser reportadas rapidamente, mesmo sem confirmação.

Exemplos: ransomware ou vírus; phishing; conta invadida; perda ou roubo de notebook, celular ou mídia; envio de boletim ou lista de alunos ao destinatário errado; acesso não autorizado; site ou aplicativo alterado ou indisponível; falha de backup; exclusão indevida; perda de banco de dados ou indisponibilidade de fornecedor.

O fluxo, a severidade e a ficha de registro estão detalhados em [Resposta a incidentes](resposta-a-incidentes.md).

## 11. Comunicação de incidentes e obrigações regulatórias

A Resolução CD/ANPD nº 15/2024 disciplina a comunicação de incidentes de segurança com dados pessoais. Quando o incidente puder acarretar risco ou dano relevante aos titulares, o controlador deve avaliar a comunicação à ANPD e aos titulares, observando critérios e prazos aplicáveis.

A referência geral indicada no documento-base é de **três dias úteis**, contados do conhecimento pelo controlador de que o incidente afetou dados pessoais, para comunicação à ANPD e aos titulares, ressalvada regra específica. A resolução prevê etapas preliminar e complementar em situações justificadas nas quais ainda não estejam disponíveis todas as informações. Prazo diferenciado para agentes de pequeno porte depende de enquadramento efetivo; a escola não deve presumir que se enquadra nessa categoria sem análise.

A regulamentação também exige manter registro dos incidentes de segurança com dados pessoais por, no mínimo, cinco anos, inclusive daqueles que não forem comunicados à ANPD ou aos titulares, observadas as regras aplicáveis.

Qualquer incidente com possível exposição de dados de alunos, responsáveis ou funcionários deve ser escalonado imediatamente à Direção e ao responsável por privacidade. Não se deve aguardar confirmação completa para reportar internamente.

## 12. Segurança física, pessoas e fornecedores

### 12.1. Segurança física

- Controlar entrada em áreas administrativas, arquivo físico, sala de servidores e locais com documentos confidenciais.
- Não deixar boletins, fichas, listas de chamada, documentos médicos ou contratos expostos em mesas, impressoras ou salas.
- Bloquear computadores ao se afastar e encerrar sessões ao final do expediente.
- Destruir documentos físicos confidenciais por fragmentação ou serviço controlado, conforme tabela de retenção.
- Manter procedimentos para perda de chaves, crachás, equipamentos e mídias.

### 12.2. Conscientização e treinamento

- Realizar treinamento na admissão e reciclagem anual para professores, funcionários e prestadores com acesso a dados ou sistemas.
- Abordar phishing, senhas, MFA, privacidade de alunos, compartilhamento seguro, dispositivos pessoais, mídias removíveis e reporte.
- Fazer exercícios simulados de phishing e usar resultados para melhorar o treinamento, sem constrangimento.
- Fornecer orientações específicas à secretaria, financeiro, TI, coordenações e comunicação.

### 12.3. Gestão de fornecedores

- Manter cadastro de fornecedores que acessam dados ou sistemas, com contato de segurança/privacidade, serviço e criticidade.
- Antes da contratação, avaliar controles de acesso, criptografia, backups, continuidade, subcontratados e histórico de incidentes.
- Prever contrato com confidencialidade, finalidade, instruções, segurança, notificação de incidentes em até 24 horas como meta contratual interna, cooperação, auditoria, devolução e eliminação dos dados.
- Revisar anualmente fornecedores críticos e após mudança de escopo, troca de plataforma ou incidente relevante.

### 12.4. Sala de reunião e videoconferência

- Usar contas institucionais e senhas/salas de espera quando disponíveis; evitar links públicos para reuniões confidenciais.
- Não gravar reuniões por padrão. Quando necessário, definir finalidade, acesso, prazo de guarda e aviso aos participantes.
- Ao terminar, remover arquivos temporários e sair das contas. Evitar deixar apresentações ou listas de alunos abertas.

## 13. Plano de implantação

O cronograma é uma proposta de priorização. A Direção deve ajustar prazos e recursos após o diagnóstico inicial.

| Prazo | Ações | Evidência de conclusão |
|---|---|---|
| 0–30 dias | Nomear responsáveis; aprovar canal de incidentes; inventariar servidores, equipamentos, sistemas e fornecedores; identificar Windows sem suporte; verificar backups; revisar contas administrativas; mapear sistemas com dados de alunos | Responsáveis nomeados; inventário inicial; relatório de contas privilegiadas e backups; relação de sistemas e fornecedores |
| 31–60 dias | Validar MFA em contas críticas; eliminar contas compartilhadas; definir admissão/desligamento; corrigir vulnerabilidades críticas; testar restauração; formalizar fluxo de incidente | Evidência de MFA; revisão de acessos; teste de restauração; procedimento aprovado |
| 61–90 dias | Desenhar segmentação; separar laboratórios e convidados; avaliar proteção de endpoints; restringir acesso ao data center; revisar contratos do site e aplicativo; validar aviso de privacidade | Diagrama de rede; regras aprovadas; relatório de proteção; checklist físico; contratos revisados |
| 3–6 meses | Implantar segmentação; centralizar logs críticos; revisar retenção e descarte; treinar equipes; realizar simulado de phishing e exercício de indisponibilidade | Relatório de implantação; evidência de logs; matriz de retenção; lista de presença; relatório de exercício |
| 6–12 meses | Avaliação técnica de vulnerabilidades; revisar riscos e fornecedores; teste ampliado de recuperação; avaliar segurança do site/aplicativo; revisar plano e metas de RTO/RPO | Relatório técnico; plano de correção; teste de recuperação; avaliação de fornecedor; versão revisada |

### 13.1. Dependências e aprovações

- Orçamento para proteção de endpoints, backup, MFA, firewall, armazenamento e substituição de equipamentos.
- Disponibilidade da equipe técnica e das áreas para levantamento e validação.
- Acesso aos contratos e painéis de administração dos fornecedores.
- Aprovação de políticas e comunicação institucional pela Direção.
- Janelas de manutenção que não comprometam aulas, avaliações e matrículas.

## 14. Indicadores e revisão

A escola deve acompanhar indicadores objetivos, com responsáveis e periodicidade. O objetivo é verificar se os controles funcionam, não apenas se documentos foram produzidos.

| Indicador | Meta inicial sugerida | Periodicidade |
|---|---|---|
| Equipamentos inventariados | 100% dos equipamentos sob gestão escolar cadastrados | Mensal até concluir; depois trimestral |
| Equipamentos com sistema suportado e atualizado | 95% ou mais; exceções documentadas e com plano | Mensal |
| Cobertura de proteção de endpoint | 100% dos computadores gerenciados com proteção ativa | Mensal |
| Contas críticas com MFA | 100% quando o sistema suportar MFA | Mensal |
| Revisão de acessos críticos | 100% dos sistemas críticos revisados no trimestre | Trimestral |
| Backups concluídos | 95% ou mais dos trabalhos previstos, com falhas tratadas | Semanal/mensal |
| Testes de restauração | Ao menos um teste por trimestre e teste anual ampliado | Trimestral/anual |
| Treinamento de segurança | 100% dos colaboradores ativos treinados no ciclo anual | Anual |
| Incidentes registrados | 100% dos incidentes reportados registrados e classificados | Mensal |
| Fornecedores críticos avaliados | 100% dos fornecedores críticos com avaliação atualizada | Anual |

### 14.1. Rotina de revisão

- **Mensal:** TI apresenta falhas de backup, atualizações, alertas e contas privilegiadas.
- **Trimestral:** Comitê revisa riscos, acessos, incidentes, fornecedores e andamento do plano.
- **Anual:** Direção aprova revisão do plano, orçamento e metas de continuidade; ocorre exercício de recuperação.
- **Extraordinária:** após incidente grave, alteração de fornecedor crítico, novo sistema, mudança relevante da rede ou alteração normativa.

## 15. Referências legais e técnicas

As referências estão reunidas em [REFERENCIAS.md](../REFERENCIAS.md). A escola deve acompanhar versões e orientações vigentes e buscar validação jurídica quando necessário.

## Anexos operacionais

Os seguintes modelos estão organizados em [Modelos e registros](modelos-e-registros.md):

- Checklist de diagnóstico inicial.
- Ficha rápida de registro de incidente.
- Campos para formalização dos responsáveis e contatos institucionais.
