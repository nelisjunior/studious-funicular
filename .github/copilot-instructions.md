```markdown name=README.md
# Meta App Metadata

Repositório contendo metadados do aplicativo para Meta App Dashboard.

## App Info
- **ID:** 25434790692795135
- **Nome:** Nome de exibição
- **Agente:** Agente Tupiniquin
- **Categoria:** Bots do Messenger para empresas
- **Email:** facebook@nelis.me

## URLs
- Política de Privacidade: `https://example.com/politica-privacidade`
- Termos de Serviço: `https://example.com/termos`
- Exclusão de Dados: `https://example.com/instrucoes-exclusao-dados`
```

```json name=app-metadata.json
{
  "appId": "25434790692795135",
  "displayName": "Nome de exibição",
  "agentName": "Agente Tupiniquin",
  "contactEmail": "facebook@nelis.me",
  "privacyPolicyUrl": "https://example.com/politica-privacidade",
  "privacyPolicyDialog": "Política de Privacidade da caixa de diálogo Login e Detalhes do aplicativo",
  "termsOfServiceUrl": "https://example.com/termos",
  "termsOfServiceDialog": "Termos de Serviço da caixa de diálogo de Login e Detalhes do aplicativo",
  "userDataDeletionUrl": "https://example.com/instrucoes-exclusao-dados",
  "category": "Bots do Messenger para empresas",
  "createdAt": "2024-01-15T00:00:00Z",
  "updatedAt": "2024-01-15T00:00:00Z"
}
```

```yaml name=app-metadata.yaml
appId: "25434790692795135"
displayName: Nome de exibição
agentName: Agente Tupiniquin
contactEmail: facebook@nelis.me
privacyPolicyUrl: https://example.com/politica-privacidade
privacyPolicyDialog: Política de Privacidade da caixa de diálogo Login e Detalhes do aplicativo
termsOfServiceUrl: https://example.com/termos
termsOfServiceDialog: Termos de Serviço da caixa de diálogo de Login e Detalhes do aplicativo
userDataDeletionUrl: https://example.com/instrucoes-exclusao-dados
category: Bots do Messenger para empresas
createdAt: 2024-01-15T00:00:00Z
updatedAt: 2024-01-15T00:00:00Z
```

```plain name=.gitignore
node_modules/
.DS_Store
*.log
.env
config.json
```

```plain name=LICENSE
MIT License
Copyright (c) 2024
Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files, to deal in the Software
without restriction, including without limitation the rights to use, copy,
modify, merge, publish, distribute, sublicense, and/or sell copies of the
Software, and to permit persons to whom the Software is furnished to do so.
THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED.
