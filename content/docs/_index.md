+++
title = 'Docs'
date = 2026-04-06T23:11:24-03:00
draft = false
+++

# Documentação do Sistema

## Índice

- [1. Configuração](#configuracao)
- [2. Vendas](#vendas)
- [3. Relatórios](#relatorios)
- [4. Compras](#compras)

---

## 1. Configuração {#configuracao}

### Empresa {#empresa}
Você deve preencher com dados corretos sobre sua empresa, especialmente se vai emitir nota.  
*As informações poderão ser usadas na emissão de notas fiscais e recibos não fiscais.*

---

### Financeiro {#financeiro}
Campos usados para facilitar a automação da aplicação de taxas padrões, preencha com valores em porcentagem.  
*Os valores serão usados como sugestão na hora do cadastro de produtos e vendas que utilizem crédito ou débito.*

---

### Fiscal {#fiscal}

Configuração de dados obrigatórios para emissão de **nota fiscal**.

- **Usar IBS**  
Marcar "Usar IBS" fará com que as notas sejam emitidas usando os novos campos IBS da reforma tributária.

- **Número da última NF**  
Preencha com os valores da última nota emitida ou `0` se nunca usou outro sistema.

- **Ambiente**
  - **Homologação**: testes (sem valor fiscal)
  - **Produção**: notas reais

- **CSC e ID CSC**  
Acesse: https://receita.pr.gov.br

- **Pasta Schemas**
  - Windows: `%appdata%\Roaming\QEstoqueLoja\recursos\NFeSchemas`
  - Linux: `/usr/local/share/QEstoqueLoja/recursos/NFeSchemas`

- **Certificado**
Arquivo `.pfx` modelo A1.

- **Código UF**
https://sistemasweb.agricultura.gov.br/manuais/Manual_PGA_WS/322CodigoIBGESigladaUnidadeFeder.html

- **Código do Município**
https://www.ibge.gov.br/explica/codigos-dos-municipios.php

- **Inscrição Estadual**
Número da empresa.

---

### Produto {#conf-produto}
Use esta aba para definir valores padrão de impostos.

---

### E-mail {#conf-email}

Configure o envio automático de notas.

#### Gmail (OAuth2)
Use senha de app:  
https://support.google.com/accounts/answer/185833?hl=pt-BR

SMTP:  
https://developers.google.com/workspace/gmail/imap/imap-smtp?hl=pt-br

---

### Contador {#conf-contador}
Preencha nome e email do contador.

---

## 2. Vendas {#vendas}

### Como vender {#pedido}

1. Abra a tela "Vendas" ou pressione `F5`
2. Pesquise produto e selecione com `Enter`
3. Edite preço/quantidade com duplo clique
4. Clique em **Próximo: Pagamento**
5. Finalize a venda (com ou sem nota)

---

### Vendas a prazo {#venda-prazo}

- Registre pagamentos na tela de entradas
- Gere recibo clicando com botão direito

---

### Recibos e DANFE {#recibos}

- Clique com botão direito na venda
- Escolha:
  - Imprimir Recibo
  - Imprimir DANFE

---

## 3. Relatórios {#relatorios}

### Gráficos {#grafico-venda}
Relatórios de:
- Valor de vendas
- Produtos mais vendidos

---

### Orçamento {#orcamento}

- Gere orçamento em PDF
- Pode incluir logo da empresa

---

## 4. Compras {#compras}

Consulte notas fiscais recebidas e importe produtos automaticamente.

---

### Importação de produtos {#importacao-cadastro-produtos}

1. Selecione a nota
2. Clique com botão direito
3. "Adicionar Produto"
4. Informe código de barras

---

### Devolução {#compras-devolucao}

1. Selecione nota
2. Escolha produtos
3. Clique em "Devolver Produtos"