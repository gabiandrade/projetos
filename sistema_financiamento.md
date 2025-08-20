# 📌 Projeto Final – Sistema de Financiamento

## 🎯 Objetivo

Desenvolver um sistema de simulação de financiamento utilizando os conceitos de Programação Orientada a Objetos (POO) em Java. 
O sistema será usado por funcionários da instituição financeira para cadastrar e consultar financiamentos de clientes, permitindo aplicar regras de negócio diferentes para imóveis e veículos.

---

## 🧑‍💻 Conceitos de POO a serem aplicados
- **Classes e Objetos**: Cliente, Financiamento (abstrata), FinanciamentoImovel, FinanciamentoVeiculo.  
- **Herança e Polimorfismo**: cálculo de parcelas e juros de acordo com o tipo de financiamento.  
- **Encapsulamento**: uso de atributos privados e métodos getters/setters.  
- **Composição**: um Cliente está associado a um Financiamento.  
- **Menu interativo**: implementação com `Scanner` para capturar opções e dados do usuário.  

---

## 📋 Fluxo do Sistema
1. Exibir **Menu Principal**:
   ```text
   === MENU PRINCIPAL ===
   1 - Financiamento de Imóvel
   2 - Financiamento de Veículo
   3 - Listar Financiamentos de Imóveis (DESAFIO-EXTRA)
   4 - Listar Financiamentos de Veículos (DESAFIO-EXTRA)
   0 - Sair
   Escolha uma opção:
     
2. Após a escolha, solicitar os dados do cliente:

- Nome
- Idade
- Renda mensal
- Valor do bem

3. Aplicar as **regras de negócio** específicas.  
4. Exibir o resultado:  
- ✅ Se aprovado: mostrar entrada, parcelas, juros e valor final.  
- ❌ Se reprovado: mostrar motivo da reprovação.  

---

## 📋 Regras de Negócio

### 🔹 Financiamento de Imóvel
- Idade mínima: **21 anos**  
- Entrada: **20% do valor do imóvel**  
- Máximo de parcelas: **360 (30 anos)**  
- Juros: **8% ao ano**  
- Parcela não pode ultrapassar **30% da renda mensal**  

### 🔹 Financiamento de Veículo
- Idade mínima: **18 anos**  
- Entrada: **10% do valor do veículo**  
- Máximo de parcelas: **60 (5 anos)**  
- Juros: **1,5% ao mês**  
- Parcela não pode ultrapassar **20% da renda mensal**

### 🔹 Listagem de Financiamentos

Ao escolher listar financiamentos (opções 3 ou 4), o sistema exibirá para cada cliente:

-Nome do cliente
-Valor do bem
-Status: Aprovado ✅ ou Reprovado ❌
-Motivo da reprovação (se aplicável)
---

## 📌 Exemplo de Execução

1. ✅ Exemplo de Aprovado:
   ```text
    === MENU PRINCIPAL ===
    1 - Financiamento de Imóvel
    2 - Financiamento de Veículo
    0 - Sair
    Escolha uma opção: 2
    
    Digite seu nome: João Silva
    Digite sua idade: 20
    Digite sua renda mensal: 2500
    Digite o valor do veículo: 50000
    
    Financiamento Aprovado!
    Entrada mínima: R$ 5.000,00
    Valor financiado: R$ 45.000,00
    Número de parcelas: 48
    Valor da parcela: R$ 468,75
     
2. ❌ Exemplo de Reprovado:
   ```text
    === MENU PRINCIPAL ===
    1 - Financiamento de Imóvel
    2 - Financiamento de Veículo
    0 - Sair
    Escolha uma opção: 1
    
    Digite seu nome: Maria Oliveira
    Digite sua idade: 19
    Digite sua renda mensal: 3500
    Digite o valor do imóvel: 200000
    
    Financiamento Reprovado!
    Motivo: Idade mínima para financiamento de imóvel é 21 anos.

Bom projeto!!
