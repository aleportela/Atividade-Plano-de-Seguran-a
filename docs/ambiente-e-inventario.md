# Ambiente e inventário

Este documento organiza o que já foi informado sobre o ambiente e o que ainda precisa ser confirmado. Ele não substitui o inventário técnico real.

## 1. Caracterização conhecida

| Elemento | Informação conhecida | Ação de levantamento |
|---|---|---|
| Alunos | Aproximadamente 2.200 | Confirmar quantitativo e sistemas que armazenam seus dados |
| Professores e funcionários | Existem; quantitativos não informados | Identificar pessoas, funções, vínculos e perfis de acesso |
| Laboratórios | 3 laboratórios com 30 computadores cada | Confirmar patrimônio, localização, sistema, atualização e usuário |
| Parque adicional | Desktops e notebooks fora dos laboratórios | Levantar quantidade, localização, responsável, garantia e suporte |
| Data center | Local / on-premise | Inventariar servidores, serviços, contas, energia, climatização, logs e backup |
| Site | Hospedagem contratada | Identificar fornecedor, contrato, painel administrativo, dados e integrações |
| Aplicativo | Aplicativo institucional | Identificar fornecedor, dados tratados, permissões, integrações e atualizações |
| Sistema operacional | Windows | Identificar versões e situação de suporte |
| Sala de reunião | Espaço identificado no levantamento inicial | Verificar computador, tela, videoconferência, Wi-Fi e exposição de documentos |

## 2. Lacunas que precisam ser levantadas

Ainda não foram confirmados: quantidade e versões dos servidores; topologia e endereçamento da rede; firewall; Wi-Fi; provedor de internet; diretório e gestão de identidades; e-mail; sistemas acadêmicos e financeiros; fornecedor do aplicativo; controles atuais de backup; solução antimalware/EDR; VPN; monitoramento; e quantidade total de funcionários e professores.

## 3. Modelo de inventário de ativos

| Campo | Preenchimento |
|---|---|
| Identificador patrimonial / serial | |
| Tipo de ativo | |
| Fabricante e modelo | |
| Localização física | |
| Setor / responsável | |
| Sistema operacional e versão | |
| Aplicativos relevantes | |
| Endereço / identificação de rede (em registro restrito) | |
| Situação de atualização e suporte | |
| Proteção de endpoint | |
| Criptografia | |
| Criticidade | |
| Data da última verificação | |
| Observações / plano de ação | |

## 4. Inventário de sistemas e fornecedores

Para cada sistema, serviço ou fornecedor, registrar nome, finalidade, responsável interno, dados tratados, local de hospedagem, integrações, usuários com acesso, contrato, suporte, backup, recuperação, procedimento de saída e contato para incidentes.

## 5. Classificação das informações

| Classe | Exemplos | Regras mínimas |
|---|---|---|
| Pública | Calendário público, comunicados aprovados | Revisar antes de publicar; evitar dados pessoais desnecessários |
| Interna | Procedimentos e documentos operacionais | Acesso a colaboradores autorizados e uso de canais institucionais |
| Confidencial | Matrícula, notas, frequência, contratos, folha e contatos | Acesso por função; armazenamento institucional; criptografia quando disponível |
| Restrita / sensível | Saúde, deficiência, biometria, medidas disciplinares, credenciais e documentos de identificação | Acesso estritamente necessário; MFA em sistemas críticos; criptografia e registro |

## 6. Cuidados com o inventário

- Não registrar senhas, tokens, chaves, dados pessoais desnecessários ou segredos.
- Manter diagramas detalhados, endereços internos, configurações e inventários completos em local de acesso restrito.
- Registrar responsável e data da verificação.
- Marcar como pendente qualquer informação ainda não confirmada.
- Não afirmar que um controle está ativo sem evidência verificável.
