# CRM-WSA: Automação de Busca de Contratos

[![Deploy to GitHub Pages](https://github.com/Igorofyeshu4/CRM-wsa/actions/workflows/deploy.yml/badge.svg)](https://github.com/Igorofyeshu4/CRM-wsa/actions/workflows/deploy.yml)
[![GitHub license](https://img.shields.io/github/license/Igorofyeshu4/CRM-wsa)](https://github.com/Igorofyeshu4/CRM-wsa/blob/main/LICENSE)
[![GitHub stars](https://img.shields.io/github/stars/Igorofyeshu4/CRM-wsa)](https://github.com/Igorofyeshu4/CRM-wsa/stargazers)

> 🤖 Workflow de automação desenvolvido por Igor Soares para busca e extração de informações de contratos em sistema CRM.

[Ver Demo](https://igorofyeshu4.github.io/CRM-wsa/) | [Tutorial](https://automa.site) | [Reportar Bug](https://github.com/Igorofyeshu4/CRM-wsa/issues)

## 📋 Sobre o Projeto

Este projeto automatiza o processo de busca e verificação de contratos em sistemas CRM usando a extensão Automa. O workflow é capaz de processar múltiplos contratos simultaneamente, extrair informações relevantes e exportar os resultados em diferentes formatos.

### 🌟 Destaques
- ⚡ Processamento rápido de múltiplos contratos
- 🔍 Busca inteligente por palavras-chave
- 📊 Exportação para CSV e Google Sheets
- 🔒 Validação de dados integrada
- 🚀 Interface amigável

## 🛠️ Tecnologias Utilizadas

- [Automa](https://www.automa.site/) - Framework de automação
- [GitHub Actions](https://github.com/features/actions) - CI/CD e deploy automático
- [GitHub Pages](https://pages.github.com/) - Hospedagem da documentação

## 🚀 Começando

### Pré-requisitos
- Google Chrome ou Microsoft Edge
- Extensão Automa instalada
- Acesso ao sistema CRM

### Instalação

1. Instale a extensão Automa:
   ```bash
   # Chrome Web Store
   https://chrome.google.com/webstore/detail/automa/infppggnoaenmfagbfknfkancpbljcca
   ```

2. Clone o repositório:
   ```bash
   git clone https://github.com/Igorofyeshu4/CRM-wsa.git
   cd CRM-wsa
   ```

3. Importe o workflow:
   - Abra o Automa Dashboard
   - Clique em "Importar"
   - Selecione o arquivo `crm-workflow.json`

## 💻 Uso

1. Execute o workflow no Automa
2. Insira os números dos contratos (4-6 dígitos cada)
3. Aguarde o processamento
4. Verifique os resultados no arquivo CSV ou Google Sheets

### Exemplo de Entrada
```
1234
5678
91011
```

### Exemplo de Saída
```csv
Contrato,Palavras-Chave,Status
1234,"COD:;BANCO",Encontrado
5678,"CÓD:",Encontrado
91011,"",Não Encontrado
```

## 🔄 Pipeline CI/CD

O projeto utiliza GitHub Actions para automação do processo de deploy:

```yaml
name: Deploy to GitHub Pages
on:
  push:
    branches: [main]
  workflow_dispatch:

jobs:
  deploy:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v3
      - uses: actions/configure-pages@v3
      - uses: actions/upload-pages-artifact@v2
      - uses: actions/deploy-pages@v2
```

### Fluxo do Pipeline
1. 📥 Checkout do código
2. ⚙️ Configuração do GitHub Pages
3. 📤 Upload dos arquivos
4. 🚀 Deploy automático

## 📈 Status do Projeto

- ✅ Busca de contratos
- ✅ Extração de dados
- ✅ Exportação CSV
- ✅ Integração com Google Sheets
- 🔄 Pipeline CI/CD
- 📚 Documentação

## 🤝 Contribuindo

1. Fork o projeto
2. Crie sua Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit suas mudanças (`git commit -m 'Add some AmazingFeature'`)
4. Push para a Branch (`git push origin feature/AmazingFeature`)
5. Abra um Pull Request

## 📫 Contato

Igor Soares - [@Igorofyeshu4](https://github.com/Igorofyeshu4)

## 📄 Licença

Este projeto está sob a licença MIT - veja o arquivo [LICENSE](LICENSE) para detalhes.

---

<div align="center">

### ⭐ Gostou do projeto? Deixe uma estrela!

[![GitHub stars](https://img.shields.io/github/stars/Igorofyeshu4/CRM-wsa?style=social)](https://github.com/Igorofyeshu4/CRM-wsa/stargazers)

</div>
