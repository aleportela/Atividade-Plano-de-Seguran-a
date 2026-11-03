# Controles técnicos

Este documento reúne as medidas técnicas propostas no plano. Cada item precisa ser avaliado pela equipe responsável e só deve ser marcado como implantado após validação.

## 1. Identidades e autenticação

- Utilizar contas individuais; não compartilhar credenciais.
- Aplicar privilégio mínimo e separar perfis de alunos, professores, secretaria, financeiro, TI e fornecedores.
- Ativar MFA para administradores, acesso remoto, e-mail institucional, hospedagem, nuvem e sistemas com dados pessoais, sempre que suportado.
- Separar contas privilegiadas das contas comuns.
- Revisar mensalmente contas administrativas e trimestralmente os acessos aos sistemas críticos.
- Revogar acessos de usuários desligados e de fornecedores ao fim do serviço.

## 2. Estações Windows, desktops e notebooks

- Inventariar hostname, patrimônio/serial, localização, responsável, versão, atualização, software e situação de suporte.
- Manter sistemas e aplicativos em versões suportadas e corrigidas.
- Utilizar proteção antimalware/EDR centralizada, com alertas enviados à TI.
- Remover privilégios de administrador local de usuários comuns.
- Ativar criptografia de disco em notebooks e equipamentos com dados confidenciais, guardando chaves de forma segura.
- Configurar bloqueio automático, senha/PIN, firewall local e inicialização segura quando compatíveis.
- Controlar instalação e execução de programas e uso de USB conforme necessidade pedagógica.
- Nos laboratórios, utilizar contas de aluno limitadas, separar dados e restaurar computadores conforme rotina aprovada.

## 3. E-mail, navegação e colaboração

- Habilitar filtragem antiphishing/antispam e proteção de anexos e links.
- Configurar SPF, DKIM e DMARC no domínio.
- Não encaminhar dados pessoais de alunos para contas pessoais.
- Usar armazenamento institucional com permissões explícitas e prazo de validade.
- Confirmar por canal independente pedidos urgentes de pagamento, alteração bancária, envio de listas ou redefinição de senha.
- Restringir encaminhamento automático para e-mails externos e revisar regras suspeitas.

## 4. Rede escolar e segmentação

A arquitetura deve impedir que uma estação comprometida em laboratório alcance livremente servidores, financeiro, secretaria ou equipamentos de gestão.

| Zona sugerida | Finalidade | Regra de comunicação |
|---|---|---|
| Administrativa | Secretaria, financeiro, direção e apoio | Somente sistemas e impressoras necessários |
| Pedagógica / professores | Computadores e recursos docentes | Sistemas pedagógicos autorizados |
| Laboratórios de alunos | 90 computadores | Internet e recursos pedagógicos aprovados; bloquear servidores e painéis administrativos |
| Servidores / data center | Servidores, armazenamento, virtualização e backup | Acesso de sistemas e administradores autorizados |
| Convidados / BYOD | Visitantes e dispositivos pessoais | Somente internet; isolamento da rede interna |
| Gerenciamento | Firewall, switches, Wi-Fi e monitoramento | Acesso exclusivo de TI, com MFA e logs |

Recomendações: firewall com regras explícitas e revisão semestral; Wi-Fi corporativo com autenticação adequada; rede separada para visitantes; proibição de pontos de acesso não autorizados; desativação de serviços inseguros desnecessários; cópia segura das configurações; acesso remoto por VPN ou solução equivalente com MFA e registro; não expor RDP ou painéis administrativos diretamente à internet.

## 5. Data center local

- Restringir acesso físico, controlar chaves ou acesso eletrônico e registrar visitantes e técnicos.
- Manter rack trancado e cabeamento identificado.
- Avaliar proteção contra incêndio, água, poeira e calor.
- Avaliar UPS/nobreak, aterramento, energia, climatização e desligamento seguro.
- Inventariar servidores, sistemas, serviços, contas administrativas, certificados, licenças e datas de suporte.
- Atualizar em janela controlada, com backup prévio e plano de retorno.
- Desabilitar contas padrão e serviços desnecessários.
- Centralizar logs críticos em repositório protegido, com horário sincronizado e acesso restrito.
- Separar credenciais e permissões do ambiente de backup; não usar produção como única cópia.

## 6. Site e aplicativo institucional

- Identificar fornecedores, suboperadores, localização do armazenamento, integrações, dados coletados e responsáveis.
- Revisar contratos quanto a finalidade, confidencialidade, segurança, acesso, subcontratação, incidentes, retenção, devolução e eliminação.
- Propor meta contratual interna de notificação à escola em até 24 horas após suspeita ou confirmação de incidente relevante. Esse prazo é proposta interna, não prazo legal da ANPD.
- Proteger painéis administrativos com MFA e contas individuais.
- Atualizar CMS, plugins, bibliotecas e componentes do aplicativo.
- Solicitar evidências de backup, restauração, testes de segurança e gestão de vulnerabilidades.
- Evitar publicar dados de alunos em páginas abertas, links públicos ou diretórios indexáveis.

## 7. Segurança física, sala de reunião e videoconferência

- Controlar acesso às áreas administrativas, arquivo físico, sala de servidores e locais com documentos confidenciais.
- Não deixar documentos escolares expostos em mesas, impressoras ou salas.
- Bloquear computadores ao se afastar e encerrar sessões ao fim do expediente.
- Destruir documentos físicos confidenciais conforme tabela de retenção.
- Para reuniões, usar contas institucionais, senhas e sala de espera quando disponíveis.
- Evitar links públicos para reuniões confidenciais.
- Não gravar reuniões por padrão; quando necessário, definir finalidade, acesso, prazo de guarda e aviso aos participantes.
