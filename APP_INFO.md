# Informações do Aplicativo - Política META

**Última atualização:** 22 de outubro de 2025

## Resumo Executivo

Este documento consolida todas as informações necessárias para conformidade com as políticas da plataforma META (Facebook Platform). Ele serve como guia de referência rápida para configuração e manutenção do aplicativo na plataforma META.

## Índice

1. [Informações Básicas do Aplicativo](#informações-básicas-do-aplicativo)
2. [URLs Obrigatórias](#urls-obrigatórias)
3. [Domínios do Aplicativo](#domínios-do-aplicativo)
4. [Política de Privacidade](#política-de-privacidade)
5. [Termos de Serviço](#termos-de-serviço)
6. [Exclusão de Dados do Usuário](#exclusão-de-dados-do-usuário)
7. [Configurações da Plataforma META](#configurações-da-plataforma-meta)
8. [Conformidade e Segurança](#conformidade-e-segurança)
9. [Contato e Suporte](#contato-e-suporte)

---

## Informações Básicas do Aplicativo

### Identificação
- **Nome do Aplicativo:** [Nome do seu aplicativo]
- **App ID:** [Será fornecido pela META após cadastro]
- **App Secret:** [Será fornecido pela META - manter em segredo]
- **Categoria:** [Social, Jogos, Negócios, etc.]
- **Plataforma:** Web, iOS, Android

### Descrição
Breve descrição do aplicativo e seus principais recursos:
- [Descreva o propósito do aplicativo]
- [Liste os principais recursos]
- [Explique o valor para os usuários]

### Público-Alvo
- **Faixa Etária:** 13+ anos
- **Região Geográfica:** Brasil / Global
- **Idiomas Suportados:** Português (BR), Inglês

---

## URLs Obrigatórias

### URL Principal do Aplicativo
```
https://example.com
```

### URL de Política de Privacidade
```
https://example.com/privacy-policy
```
**Arquivo de Referência:** [PRIVACY_POLICY.md](PRIVACY_POLICY.md)

**Requisitos:**
- ✅ Acessível publicamente sem necessidade de login
- ✅ Descreve quais dados são coletados
- ✅ Explica como os dados são usados
- ✅ Descreve com quem os dados são compartilhados
- ✅ Inclui informações sobre integração META

### URL de Termos de Serviço
```
https://example.com/terms-of-service
```
**Arquivo de Referência:** [TERMS_OF_SERVICE.md](TERMS_OF_SERVICE.md)

**Requisitos:**
- ✅ Acessível publicamente
- ✅ Define direitos e responsabilidades dos usuários
- ✅ Descreve uso aceitável do aplicativo
- ✅ Inclui termos relacionados à integração META

### URL de Exclusão de Dados
```
https://example.com/data-deletion
```
**Arquivo de Referência:** [DATA_DELETION.md](DATA_DELETION.md)

**Requisitos:**
- ✅ Instruções claras sobre como solicitar exclusão
- ✅ Métodos alternativos de contato
- ✅ Prazo de processamento (máximo 30 dias)
- ✅ Descrição dos dados que serão excluídos

---

## Domínios do Aplicativo

**Arquivo de Referência Completo:** [APP_DOMAINS.md](APP_DOMAINS.md)

### App Domains (Configuração META)
```
example.com
api.example.com
```

### Domínios Adicionais
- **Staging:** `staging.example.com`
- **Development:** `dev.example.com`
- **API:** `api.example.com`
- **CDN:** `cdn.example.com`

### URLs de Redirecionamento OAuth
```
https://example.com/auth/callback
https://example.com/auth/facebook/callback
https://example.com/auth/meta/callback
```

### URLs de Canvas (se aplicável)
- **Canvas URL:** `https://example.com/canvas`
- **Secure Canvas URL:** `https://example.com/canvas`

---

## Política de Privacidade

### Resumo dos Dados Coletados

#### Informações do Usuário
- Nome e informações de perfil público
- Endereço de e-mail
- ID de usuário META (quando usa login social)
- Foto de perfil (se autorizado)

#### Informações de Uso
- Dados de interação com o aplicativo
- Preferências e configurações
- Histórico de atividades

#### Informações Técnicas
- Endereço IP
- Tipo de dispositivo e navegador
- Sistema operacional
- Identificadores de dispositivo

### Uso de Dados META
Quando o usuário faz login através da plataforma META:
- Solicitamos apenas permissões essenciais
- Respeitamos as preferências de privacidade do usuário
- Seguimos as Políticas de Plataforma META
- Não vendemos dados do usuário

### Compartilhamento de Dados
- Não compartilhamos dados com terceiros sem consentimento
- Podemos compartilhar com provedores de serviços necessários
- Cumprimos com requisitos legais quando aplicável

**Documento Completo:** [PRIVACY_POLICY.md](PRIVACY_POLICY.md)

---

## Termos de Serviço

### Pontos Principais

#### Elegibilidade
- Idade mínima: 13 anos
- Deve aceitar os termos para usar o aplicativo
- Deve fornecer informações precisas

#### Uso Aceitável
Proibido:
- Conteúdo ilegal ou ofensivo
- Violação de direitos de terceiros
- Tentativas de hacking ou abuso
- Spam ou uso comercial não autorizado

#### Propriedade Intelectual
- O aplicativo e seu conteúdo são protegidos por direitos autorais
- Usuários mantêm propriedade de seu conteúdo
- Licença concedida para operação do serviço

#### Integração META
- Conformidade com Políticas da Plataforma META
- Uso apropriado de dados obtidos via META
- Respeito aos termos de serviço da META

**Documento Completo:** [TERMS_OF_SERVICE.md](TERMS_OF_SERVICE.md)

---

## Exclusão de Dados do Usuário

### Métodos de Solicitação

#### 1. Através do Aplicativo
```
Configurações → Conta → Excluir Conta e Dados
```

#### 2. Via E-mail
```
Enviar para: data-deletion@example.com
Assunto: Solicitação de Exclusão de Dados
```

#### 3. Formulário Online
```
https://example.com/data-deletion
```

#### 4. Através do Facebook
```
Configurações do Facebook → Aplicativos e Sites → Remover
```

### Callback URL para META
```
POST https://api.example.com/meta/data-deletion
```

**Payload esperado:**
```json
{
  "user_id": "USER_ID",
  "confirmation_code": "CONFIRMATION_CODE"
}
```

**Resposta:**
```json
{
  "url": "https://example.com/data-deletion/status?code=CONFIRMATION_CODE",
  "confirmation_code": "CONFIRMATION_CODE"
}
```

### Prazo de Processamento
- **Confirmação:** Até 24 horas
- **Exclusão Completa:** Até 30 dias
- **Notificação:** E-mail de confirmação ao concluir

### Dados Excluídos
- Informações de perfil
- Conteúdo gerado pelo usuário
- Dados de atividade
- Tokens de autenticação
- Logs e dados técnicos (após período de retenção)

**Documento Completo:** [DATA_DELETION.md](DATA_DELETION.md)

---

## Configurações da Plataforma META

### Dashboard do Facebook Developers

#### 1. Basic Settings
```
App ID: [Seu App ID]
App Secret: [Mantenha seguro]
Display Name: [Nome do Aplicativo]
Contact Email: support@example.com
Privacy Policy URL: https://example.com/privacy-policy
Terms of Service URL: https://example.com/terms-of-service
Category: [Selecione categoria apropriada]
```

#### 2. App Domains
```
example.com
api.example.com
```

#### 3. Website Settings
```
Site URL: https://example.com
```

#### 4. Data Deletion Request Callback
```
Callback URL: https://api.example.com/meta/data-deletion
```

### Permissões e Recursos

#### Permissões Básicas (Não requerem aprovação)
- `public_profile` - Informações básicas do perfil
- `email` - Endereço de e-mail

#### Permissões Avançadas (Requerem revisão da META)
- `user_friends` - Lista de amigos que também usam o app
- `user_photos` - Acesso a fotos (se necessário)
- `user_posts` - Acesso a posts (se necessário)

**Nota:** Solicite apenas permissões essenciais para a funcionalidade do app.

### Webhook Configuration (Opcional)
```
Callback URL: https://api.example.com/webhooks/meta
Verify Token: [Seu token de verificação seguro]
```

**Eventos Subscritos:**
- `user_data_deletion` - Notificação de exclusão de dados

---

## Conformidade e Segurança

### Conformidade Regulatória

#### LGPD (Lei Geral de Proteção de Dados - Brasil)
- ✅ Consentimento explícito do usuário
- ✅ Transparência no tratamento de dados
- ✅ Direito de acesso e exclusão
- ✅ Segurança e proteção de dados
- ✅ Notificação de incidentes

#### GDPR (General Data Protection Regulation - Europa)
- ✅ Base legal para processamento
- ✅ Direitos do titular dos dados
- ✅ Portabilidade de dados
- ✅ Privacy by design
- ✅ Data Protection Officer (se aplicável)

#### Políticas da Plataforma META
- ✅ Uso aprovado de dados da plataforma
- ✅ Respeito às preferências de privacidade
- ✅ Não armazenamento indevido de dados
- ✅ Conformidade com guidelines de interface

### Medidas de Segurança

#### Segurança de Dados
- Criptografia em trânsito (HTTPS/TLS 1.2+)
- Criptografia em repouso
- Controles de acesso baseados em função
- Autenticação multifator para administradores

#### Segurança de Aplicação
- Proteção contra CSRF
- Validação de entrada
- Sanitização de saída
- Proteção contra injeção SQL
- Limitação de taxa (rate limiting)

#### Monitoramento
- Logs de auditoria
- Detecção de anomalias
- Alertas de segurança
- Backup regular de dados

### Certificações e Auditorias
- [ ] Auditoria de segurança anual
- [ ] Penetration testing
- [ ] Revisão de código de segurança
- [ ] Certificação ISO 27001 (se aplicável)

---

## Contato e Suporte

### Equipe de Suporte
- **E-mail Geral:** support@example.com
- **E-mail de Privacidade:** privacy@example.com
- **E-mail de Exclusão de Dados:** data-deletion@example.com
- **E-mail Técnico:** devops@example.com

### Horário de Atendimento
- Segunda a Sexta: 9h às 18h (Horário de Brasília)
- Sábado: 9h às 13h
- Domingo e Feriados: Fechado
- Suporte de Emergência: 24/7 para questões críticas

### Canais Adicionais
- **Website:** https://example.com/contact
- **Central de Ajuda:** https://help.example.com
- **Status do Serviço:** https://status.example.com
- **Telefone:** +55 (XX) XXXX-XXXX

### Encarregado de Proteção de Dados (DPO)
- **Nome:** [Nome do DPO]
- **E-mail:** dpo@example.com
- **Responsabilidade:** Questões relacionadas à LGPD/GDPR

### Autoridades de Proteção de Dados
- **ANPD (Brasil):** https://www.gov.br/anpd
- **Telefone ANPD:** 0800-XXX-XXXX

---

## Checklist de Implementação

### Pré-Lançamento
- [ ] Criar conta no Facebook Developers
- [ ] Registrar aplicativo na plataforma META
- [ ] Configurar App ID e App Secret
- [ ] Adicionar domínios do aplicativo
- [ ] Configurar URLs obrigatórias
- [ ] Implementar sistema de autenticação META
- [ ] Implementar callback de exclusão de dados
- [ ] Testar fluxo de OAuth
- [ ] Testar processo de exclusão de dados
- [ ] Revisar e publicar política de privacidade
- [ ] Revisar e publicar termos de serviço

### Segurança
- [ ] Configurar HTTPS em todos os domínios
- [ ] Implementar certificados SSL válidos
- [ ] Configurar CORS apropriadamente
- [ ] Implementar proteção CSRF
- [ ] Configurar rate limiting
- [ ] Implementar logging de segurança
- [ ] Configurar backup de dados

### Conformidade
- [ ] Revisar conformidade com LGPD
- [ ] Revisar conformidade com GDPR (se aplicável)
- [ ] Revisar Políticas da Plataforma META
- [ ] Configurar processo de consentimento
- [ ] Implementar exportação de dados
- [ ] Documentar fluxo de dados

### Testes
- [ ] Testar login via META
- [ ] Testar solicitação de permissões
- [ ] Testar callback de exclusão de dados
- [ ] Testar acessibilidade de URLs públicas
- [ ] Testar em diferentes dispositivos
- [ ] Realizar testes de segurança
- [ ] Testar recuperação de desastres

### Pós-Lançamento
- [ ] Monitorar logs de erro
- [ ] Revisar métricas de uso
- [ ] Coletar feedback de usuários
- [ ] Atualizar documentação conforme necessário
- [ ] Revisar políticas trimestralmente
- [ ] Manter certificados atualizados

---

## Recursos Adicionais

### Documentação da META
- [Facebook Platform Policies](https://developers.facebook.com/policy/)
- [Facebook Login Documentation](https://developers.facebook.com/docs/facebook-login/)
- [Data Deletion Guide](https://developers.facebook.com/docs/development/create-an-app/app-dashboard/data-deletion-callback)
- [App Review Process](https://developers.facebook.com/docs/app-review/)

### Documentação Legal
- [LGPD - Lei 13.709/2018](http://www.planalto.gov.br/ccivil_03/_ato2015-2018/2018/lei/l13709.htm)
- [GDPR Official Text](https://gdpr-info.eu/)
- [ANPD - Autoridade Nacional](https://www.gov.br/anpd)

### Ferramentas Úteis
- [Facebook Access Token Debugger](https://developers.facebook.com/tools/debug/accesstoken/)
- [Sharing Debugger](https://developers.facebook.com/tools/debug/)
- [Graph API Explorer](https://developers.facebook.com/tools/explorer/)

---

## Histórico de Alterações

| Data | Versão | Alterações | Autor |
|------|--------|------------|-------|
| 2025-10-22 | 1.0 | Criação inicial do documento | Equipe de Desenvolvimento |

---

## Notas Importantes

### ⚠️ Antes de ir para Produção

1. **Substitua todas as URLs de exemplo** (`example.com`) pelos domínios reais
2. **Configure credenciais reais** da META (App ID, App Secret)
3. **Atualize informações de contato** com e-mails e telefones reais
4. **Implemente o callback de exclusão de dados** conforme especificado
5. **Teste completamente** todos os fluxos antes de publicar
6. **Submeta para revisão** da META se usar permissões avançadas

### 🔒 Segurança

- **NUNCA** exponha o App Secret publicamente
- **NUNCA** commite credenciais no controle de versão
- **SEMPRE** use HTTPS em produção
- **SEMPRE** valide e sanitize entradas do usuário

### 📝 Manutenção

- Revisar políticas a cada 3 meses
- Atualizar URLs quando houver mudanças
- Monitorar notificações da plataforma META
- Manter backups regulares

---

**Para mais informações, consulte os documentos individuais:**
- [Política de Privacidade](PRIVACY_POLICY.md)
- [Termos de Serviço](TERMS_OF_SERVICE.md)
- [Exclusão de Dados do Usuário](DATA_DELETION.md)
- [Domínios do Aplicativo](APP_DOMAINS.md)
