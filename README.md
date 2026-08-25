# Calculadora Saúde e Bem-Estar
Programa simples desenvolvido em Python que permite calcular o **IMC**, a **recomendação diária de água** e a **frequência cardíaca máxima estimada**.
## Relatório de Bugs Encontrados
Durante a análise do código original, foram encontrados os seguintes bugs:
| **Bug** | **Local do Bug** | **Comportamento incorreto** | **Solução aplicada** |
|---|---|---|---|
| 1 | `calcular_imc()` — linha 5 | Fórmula do IMC incorreta. | Alterado para `altura ** 2`.
| 2 | `classificar_imc()` — linhas 12–16 | Faixas de classificação incorretas. | Faixas corrigidas.
| 3 | `calcular_agua_diaria()` — linha 21 | Fórmula da água incorreta. | Alterado para `(peso * 35) / 1000`.
| 4 | `calcular_frequencia_cardiaca_maxima()` — linha 26 | Idade somada em vez de subtraída. | Alterado para `220 - idade`.
| 5 |  linha 39 | Opção recebida como `string`.|Convertida para `int`.
| 6 | linha 47 | Comparação entre tipos diferentes. | Opção convertida para `int`.
| 7 | linha 66 | Falta do `break` ao sair. | Adicionado `break`.

## Como executar
É necessário ter o **Python 3** instalado.
Para verificar, execute no terminal:
```python
python3 --version
```
Depois, no terminal, entre na pasta do projeto e execute:
```python
python3 calculadora_saude.py
```
## Funcionamento
O programa apresenta um menu com quatro opções:
1.Calcular IMC
2.Calcular recomendação de água
3.Calcular frequência cardíaca máxima
4.Sair

As três primeiras opções solicitam os dados necessários e realizam os cálculos. A opção 4 encerra o programa.
## Exemplo de execução
```text
==============================
  SISTEMA DE SAÚDE E BEM-ESTAR
==============================
1. Calcular IMC
2. Calcular Recomendação de Água
3. Calcular Frequência Cardíaca Máxima
4. Sair

Escolha uma opção (1-4): 1
Digite seu peso (kg): 66
Digite sua altura (m): 1.70

Seu IMC é: 22.84
Classificação: Peso normal
```
## Sobre os Autores

- Alice Fernandes Barbosa - @alicefbarbosa - 326128348

- Ana Carolina de Sousa Freitas - @AnaFreitas1 - 325132932

**Atividade 2 da disciplina de Gestão e Qualidade de Software.**


