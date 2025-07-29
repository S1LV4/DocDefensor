# DocDefensor

## Descrição do Projeto

Gerador automatizado de procurações voltado para uso institucional da Defensoria Pública. Este script foi criado para ajudar um amigo do grupo da Defensoria, utilizando o  Google Colab para processar documentos modelo `.docx` com base em informações provenientes de arquivos `.csv`, permitindo gerar múltiplas procurações personalizadas de forma prática e eficiente.

## Funcionalidades

- ✅ Geração automatizada de procurações personalizadas
- ✅ Processamento de arquivos `.docx` com base em dados de arquivos `.csv`
- ✅ Execução prática e eficiente via Google Colab
- ✅ Interface simples e intuitiva
- ✅ Geração em lote para múltiplos casos

## Requisitos

- Conta no Google para acessar o Google Colab
- Arquivo modelo `.docx` para a procuração
- Arquivo `.csv` contendo os dados necessários
- Conhecimento básico de estrutura de dados CSV

## Como Usar

### 1. Execução

1. Acesse o [DocDefensor - Google Colab]([https://colab.research.google.com](https://colab.research.google.com/drive/18BBfvNwIIadPc68WZ9BfNteE0ecbOTCd?usp=sharing));
2. Clique em "Ficheiro" > Guardar uma cópia no Drive;
3. Faça upload dos seus arquivos:
   - Substitua `FORM_PROCURACAO_AGE.docx` pelo seu modelo
   - Substitua `procuracao_age.csv` pelos seus dados
4. Execute todas as células do notebook
5. Os arquivos gerados aparecerão na pasta `/procuracoes`

### 3. Download dos Resultados

- Os documentos processados ficarão disponíveis na pasta `/procuracoes`
- Faça o download individual ou compacte todos os arquivos
- Cada procuração será nomeada automaticamente com base nos dados fornecidos

## Estrutura do Projeto

```
DocDefensor/
│
├── 📄 FORM_PROCURACAO_AGE.docx     # Modelo da procuração
├── 📊 procuracao_age.csv           # Base de dados com as informações
├── 📓 main.ipynb                   # Notebook principal para execução
├── 📁 procuracoes/                 # Pasta de saída dos arquivos gerados
│   ├── procuracao_001.docx
│   ├── procuracao_002.docx
│   └── ...
└── 📖 README.md                    # Esta documentação
```

## Configurações Avançadas

### Personalização de Campos

O sistema suporta os seguintes tipos de placeholders:

- **Dados Pessoais**: `{{nome}}`, `{{cpf}}`, `{{rg}}`, `{{endereco}}`
- **Contato**: `{{telefone}}`, `{{email}}`
- **Localização**: `{{cidade}}`, `{{estado}}`, `{{cep}}`
- **Datas**: `{{data_nascimento}}`, `{{data_documento}}`
- **Campos Customizados**: Adicione conforme necessário

### Formatação de Dados

- **CPF**: Aceita com ou sem formatação (123.456.789-00 ou 12345678900)
- **Telefone**: Formatos (11) 99999-9999 ou 11999999999
- **Datas**: DD/MM/AAAA ou DD-MM-AAAA

## Solução de Problemas

### Erros Comuns

1. **"Placeholder não encontrado"**
   - Verifique se os nomes das colunas no CSV correspondem aos placeholders no modelo

2. **"Arquivo não encontrado"**
   - Certifique-se de que fez upload dos arquivos corretamente no Colab

3. **"Erro de formatação"**
   - Verifique a codificação do arquivo CSV (recomendado: UTF-8)

### Dicas de Performance

- Para lotes grandes (>100 documentos), execute em partes menores
- Use conexão estável de internet durante o processamento
- Mantenha os arquivos modelo simples para melhor performance

## Links Úteis

- 🔗 **[Google Colab para execução]([https://colab.research.google.com](https://colab.research.google.com](https://colab.research.google.com/drive/18BBfvNwIIadPc68WZ9BfNteE0ecbOTCd?usp=sharing))** 
- 👨‍💻 **[Desenvolvedor Original - S1LV4](https://github.com/S1LV4)**
- 🌐 **[Minhas redes - joao.ai](https://linktr.ee/joao.ai)**
- 📧 **Suporte**: Entre em contato através dos links acima

## Licença

Este projeto está sob a licença MIT. Veja o arquivo `LICENSE` para mais detalhes.

---

## 🌟 Gostou do projeto?

Se este projeto foi útil para você, considere:
- ⭐ Dar uma estrela no repositório
- 🔄 Compartilhar com colegas da Defensoria Pública
- 💬 Deixar feedback para melhorias futuras

**Desenvolvido com ❤️ para a Defensoria Pública**
