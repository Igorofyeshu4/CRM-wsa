# CRM-WSA: Automação de Busca de Contratos
> Desenvolvido por Igor Soares

## 🔍 Sobre o Projeto
Workflow de automação para busca e extração de informações de contratos em sistema CRM usando a extensão Automa.

## 🚀 Tutorial Completo
Acesse o tutorial completo em: [Automa.site - CRM-WSA Tutorial](https://automa.site)

## ⚡ Recursos Principais
- Busca automática de múltiplos contratos
- Validação de números de contrato (4-6 dígitos)
- Extração de palavras-chave (COD:, CÓD:, BANCO)
- Exportação para CSV e Google Sheets
- Interface amigável para entrada de dados

## 🛠️ Como Usar

### 1. Pré-requisitos
- Instale a extensão [Automa](https://chrome.google.com/webstore/detail/automa/infppggnoaenmfagbfknfkancpbljcca) no Chrome
- Acesse sua conta no sistema CRM

### 2. Configuração
1. Baixe o arquivo `crm-workflow.json`
2. Importe o workflow no Automa
3. Configure suas credenciais (se necessário)

### 3. Uso
1. Execute o workflow no Automa
2. Insira os números dos contratos
3. Aguarde o processamento
4. Verifique os resultados no arquivo CSV ou Google Sheets

## 📝 Exemplo de Entrada
```
1234
5678
91011
```

## 📊 Exemplo de Saída
```csv
Contrato,Palavras-Chave,Status
1234,"COD:;BANCO",Encontrado
5678,"CÓD:",Encontrado
91011,"",Não Encontrado
```

## 📌 Observações Importantes
- Respeite os limites de requisições do sistema
- Mantenha suas credenciais seguras
- Verifique os resultados antes de usar

## 📫 Contato
- GitHub: [@Igorofyeshu4](https://github.com/Igorofyeshu4)

## 📄 Licença
Este projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.

---
⭐ Se este projeto te ajudou, considere dar uma estrela no GitHub!
