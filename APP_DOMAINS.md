# Domínios do Aplicativo

**Última atualização:** 22 de outubro de 2025

## Introdução

Este documento lista todos os domínios autorizados e utilizados pelo nosso aplicativo, conforme requerido pelas políticas da plataforma META.

## Domínios Principais

### Domínio de Produção
- **URL Principal:** `https://example.com`
- **Descrição:** Domínio principal do aplicativo em produção
- **Uso:** Aplicativo web principal, APIs e serviços

### Domínio de API
- **URL:** `https://api.example.com`
- **Descrição:** Endpoint principal para APIs
- **Uso:** Requisições de API, integração com serviços

## Domínios de Política e Documentação

### Política de Privacidade
- **URL:** `https://example.com/privacy-policy`
- **URL Alternativa:** `https://example.com/PRIVACY_POLICY.md`
- **Descrição:** Página da Política de Privacidade
- **Acessível publicamente:** Sim

### Termos de Serviço
- **URL:** `https://example.com/terms-of-service`
- **URL Alternativa:** `https://example.com/TERMS_OF_SERVICE.md`
- **Descrição:** Página dos Termos de Serviço
- **Acessível publicamente:** Sim

### Exclusão de Dados do Usuário
- **URL:** `https://example.com/data-deletion`
- **URL Alternativa:** `https://example.com/DATA_DELETION.md`
- **Descrição:** Instruções e formulário para exclusão de dados
- **Acessível publicamente:** Sim

## Domínios de Ambiente

### Ambiente de Staging
- **URL:** `https://staging.example.com`
- **Descrição:** Ambiente de testes e homologação
- **Uso:** Testes antes da produção

### Ambiente de Desenvolvimento
- **URL:** `https://dev.example.com`
- **Descrição:** Ambiente de desenvolvimento
- **Uso:** Desenvolvimento e testes internos

## Domínios de Callback e Redirecionamento

### OAuth Redirect URIs
- `https://example.com/auth/callback`
- `https://example.com/auth/facebook/callback`
- `https://example.com/auth/meta/callback`

### Logout Redirect URIs
- `https://example.com/logout`
- `https://example.com/`

## Domínios de Canvas (META/Facebook)

### Canvas URL
- **URL:** `https://example.com/canvas`
- **Descrição:** URL para aplicativo Canvas do Facebook
- **Secure Canvas URL:** `https://example.com/canvas`

### Mobile Site URL
- **URL:** `https://example.com/mobile`
- **Descrição:** URL otimizada para dispositivos móveis

## Domínios de Suporte

### Central de Ajuda
- **URL:** `https://help.example.com`
- **Descrição:** Centro de suporte e documentação

### Portal de Contato
- **URL:** `https://example.com/contact`
- **Descrição:** Formulário de contato e suporte

## Subdomínios Autorizados

### Subdomínios de Serviço
- `cdn.example.com` - Rede de distribuição de conteúdo
- `static.example.com` - Recursos estáticos
- `media.example.com` - Upload e armazenamento de mídia
- `images.example.com` - Servidor de imagens

### Subdomínios de Infraestrutura
- `status.example.com` - Página de status do serviço
- `blog.example.com` - Blog oficial
- `docs.example.com` - Documentação técnica

## Domínios Externos Integrados

### Serviços de Terceiros Autorizados
- **Analytics:** Google Analytics (google-analytics.com)
- **CDN:** CloudFlare (cloudflare.com)
- **Storage:** AWS S3 (amazonaws.com)
- **Email:** SendGrid (sendgrid.net)

## Domínios para META Platform

### App Domains (Configuração META)
```
example.com
api.example.com
staging.example.com
```

### Site URL
- **Production:** `https://example.com`

### Privacy Policy URL
- **URL:** `https://example.com/privacy-policy`

### Terms of Service URL
- **URL:** `https://example.com/terms-of-service`

### User Data Deletion
- **Callback URL:** `https://api.example.com/meta/data-deletion`
- **Info URL:** `https://example.com/data-deletion`

## Configuração de CORS

### Origens Permitidas
```
https://example.com
https://api.example.com
https://staging.example.com
https://dev.example.com
```

### Headers Permitidos
- Authorization
- Content-Type
- X-Requested-With
- Accept

## Configuração de Segurança

### HTTPS
- **Obrigatório:** Sim
- **Certificado SSL:** Válido e atualizado
- **TLS Version:** 1.2 ou superior

### Content Security Policy (CSP)
```
default-src 'self';
script-src 'self' https://connect.facebook.net;
style-src 'self' 'unsafe-inline';
img-src 'self' data: https:;
connect-src 'self' https://api.example.com;
frame-src 'self' https://www.facebook.com;
```

## Webhooks e Callbacks

### Webhook URLs
- **Primary:** `https://api.example.com/webhooks/meta`
- **Backup:** `https://api.example.com/webhooks/facebook`

### Verification
- **Verify Token:** (Configurado no painel META)
- **Challenge:** Suportado conforme API META

## Verificação de Domínio

### Status de Verificação
- ✅ `example.com` - Verificado
- ✅ `api.example.com` - Verificado
- ⏳ `staging.example.com` - Pendente
- ⏳ `dev.example.com` - Pendente

### Método de Verificação
- DNS TXT Record
- HTML Meta Tag
- HTML File Upload

## Observações Importantes

### Política de Domínios META
1. Todos os domínios devem usar HTTPS
2. Política de Privacidade deve estar publicamente acessível
3. URLs de callback devem ser explicitamente autorizadas
4. Domínios devem ser verificados antes do uso em produção

### Manutenção
- Revisar lista de domínios trimestralmente
- Remover domínios não utilizados
- Manter certificados SSL atualizados
- Atualizar URLs nas configurações META quando necessário

## Contato

Para questões sobre domínios e configuração:
- **E-mail Técnico:** devops@example.com
- **E-mail de Suporte:** support@example.com
- **Documentação:** https://docs.example.com

---

**Nota:** Substitua `example.com` pelos domínios reais do seu aplicativo antes de configurar na plataforma META.

**Checklist de Configuração META:**
- [ ] Adicionar domínios em App Domains
- [ ] Configurar Site URL
- [ ] Adicionar Privacy Policy URL
- [ ] Adicionar Terms of Service URL
- [ ] Configurar Data Deletion Callback
- [ ] Verificar todos os domínios
- [ ] Testar OAuth redirect URIs
- [ ] Validar HTTPS em todos os domínios
