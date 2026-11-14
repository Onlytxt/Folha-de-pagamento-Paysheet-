# Folha-de-pagamento-Paysheet-
Sistema de folha de pagamento desenvolvido em Java, com cadastro de colaboradores, cálculo de salários por categoria e geração de relatórios utilizando Programação Orientada a Objetos.

# 💰 Sistema de Folha de Pagamento

Sistema de gerenciamento de folha de pagamento desenvolvido em **Java**, utilizando conceitos de **Programação Orientada a Objetos (POO)**.

O projeto permite cadastrar diferentes tipos de colaboradores, calcular suas respectivas remunerações e gerar relatórios com informações individuais e financeiras.

## 📌 Funcionalidades

- Cadastro de colaboradores.
- Cadastro por categoria de remuneração.
- Cálculo automático dos salários.
- Geração da folha de pagamento.
- Exibição de resumo financeiro.
- Validação básica das entradas fornecidas pelo usuário.

## 👥 Tipos de Colaboradores

O sistema trabalha com três categorias:

**1. Colaborador Padrão**
- Recebe um salário fixo de R$ 2.000,00.

**2. Colaborador Comissionado**
- Recebe o salário-base acrescido de uma comissão calculada sobre o valor total de suas vendas.
- O percentual de comissão é informado no cadastro.

**3. Colaborador de Produção**
- Recebe o salário-base acrescido de um valor calculado pela quantidade de peças produzidas multiplicada pelo valor pago por peça.

## 🧮 Cálculos de Remuneração

O sistema utiliza as seguintes fórmulas:

**Colaborador Padrão**

`Salário Final = Salário Base`

**Colaborador Comissionado**

`Comissão = (Valor das Vendas × Percentual) / 100`

`Salário Final = Salário Base + Comissão`

**Colaborador de Produção**

`Produtividade = Quantidade de Peças × Valor por Peça`

`Salário Final = Salário Base + Produtividade`

## 📊 Relatórios

O sistema disponibiliza duas formas de consulta:

- **Folha de Pagamento:** apresenta os dados de cada colaborador, sua categoria, salário-base, adicionais e remuneração final.
- **Resumo Financeiro:** apresenta a quantidade de colaboradores cadastrados, o valor total da folha e a média salarial.

## 🏗️ Estrutura do Projeto

```text
payroll/
│
└── src/
    │
    ├── Modelo/
    │   ├── Colaborador.java
    │   ├── ColaboradorPadrao.java
    │   ├── ColaboradorComissionado.java
    │   └── ColaboradorProducao.java
    │
    ├── Servico/
    │   └── GerarRelatorio.java
    │
    └── Principal.java
```

### Organização das Classes

- `Colaborador`: classe base que representa um colaborador.
- `ColaboradorPadrao`: implementa a remuneração fixa.
- `ColaboradorComissionado`: implementa o cálculo de comissões.
- `ColaboradorProducao`: implementa o cálculo de produtividade.
- `GerarRelatorio`: responsável pela geração da folha e dos resumos financeiros.
- `Principal`: contém o método principal, o menu interativo e o gerenciamento dos cadastros.

## 🛠️ Tecnologias e Conceitos

- **Java:** linguagem utilizada no desenvolvimento.
- **Programação Orientada a Objetos:** organização e estruturação do sistema.
- **Herança:** reutilização de características da classe base.
- **Polimorfismo:** implementação de comportamentos específicos para cada categoria de colaborador.
- **Encapsulamento:** controle de acesso aos atributos das classes.
- **ArrayList:** armazenamento dos colaboradores durante a execução.
- **Scanner:** leitura de informações fornecidas pelo usuário.

## ▶️ Como Executar

1. Faça o clone do repositório:

```bash
git clone URL_DO_SEU_REPOSITORIO
```

2. Abra o projeto em uma IDE compatível com Java, como IntelliJ IDEA ou NetBeans.

3. Execute o arquivo `Principal.java`.

4. Utilize o menu interativo no terminal para cadastrar colaboradores e consultar os relatórios.

## 🎯 Objetivo do Projeto

Este projeto foi desenvolvido com o objetivo de praticar e consolidar conhecimentos em Java, especialmente os conceitos de Programação Orientada a Objetos, por meio da construção de um sistema de gerenciamento de colaboradores e cálculo de remuneração.

---

**Desenvolvido como projeto de estudo em Java.**
