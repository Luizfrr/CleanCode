- [1. Clean code](#1-clean-code)
  - [1.1. Nomes de variáveis ruins](#11-nomes-de-variáveis-ruins)
    - [1.1.1. Nomes misteriosos](#111-nomes-misteriosos)
    - [1.1.2. Nomes exagerados](#112-nomes-exagerados)
    - [1.1.3. Nomes com tipo da variável](#113-nomes-com-tipo-da-variável)
    - [1.1.4. Nome ambíguos](#114-nome-ambíguos)
    - [1.1.5. Nomes redundantes](#115-nomes-redundantes)
    - [1.1.6. Resumo](#116-resumo)
  - [1.2. Convenção](#12-convenção)
  - [1.3. Assinatura dos métodos](#13-assinatura-dos-métodos)
  - [1.4. Muitos parâmetros dentro do método](#14-muitos-parâmetros-dentro-do-método)
  - [1.5. Parâmetros no topo](#15-parâmetros-no-topo)
  - [1.6. Parâmetros de saida](#16-parâmetros-de-saida)
  - [1.7. Números mágicos](#17-números-mágicos)


# 1. Clean code

## 1.1. Nomes de variáveis ruins

### 1.1.1. Nomes misteriosos

- Não devemos usar nomes misteriosos
- Nomes ruins:
  - dr1: SqlDataReader
  - page1: Page
  - od: int

### 1.1.2. Nomes exagerados

### 1.1.3. Nomes com tipo da variável

- Evitar no código
  - intIdade
  - strNome
  - array_Produtos
- Mas faz sentido no front, para identificar o tipo do elemento visual.

### 1.1.4. Nome ambíguos

- Evitar nomes que dizem mais de uma coisa
  - nomeDoIncidenteID: int
  - multiSelect: bool

### 1.1.5. Nomes redundantes

  - oCliente: Cliente
  - listaDeClientesElegives: list[Cliente]

### 1.1.6. Resumo

- Nomes não tão curtos nem tão grandes
- Revelar a inteção da variável
- O nome da variável deve estar relacionado ao domínio

## 1.2. Convenção

- Toda linguagem tem sua própria convenção, ou seja a comunidade criou um **style code** para um bom entendimento entre os programadores da comunidade.
- Se atentar para a forma como escrevemos as variáveis, arquivos, classes:
- Snake case: snake_case
- Pascal case: PascalCase
- Camel case: camelCase

## 1.3. Assinatura dos métodos

- Evitar:
  - def buscar_cliente(id_incidente: str) -> Fruta:
- [Código de Exemplo](AssinaturaRuim/)

## 1.4. Muitos parâmetros dentro do método

- Evitar colocar muitos pâmetros, no máximo 4, passando disso criar uma classe para encapsular os parâmetros.

## 1.5. Parâmetros no topo

- Evitar que todas as variaveis fiquem no topo, sempre que possivel.

## 1.6. Parâmetros de saida

- Sempre que possível encapsular muitos retornos dentro de uma entidade (classe)

## 1.7. Números mágicos

- Evitar
  - Status == "A"
  - Status == 1
