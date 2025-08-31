# 🏦 Sistema Bancário em Python

Um sistema bancário simples implementado em Python 3, desenvolvido para simular operações básicas de depósito, saque e extrato.

Este projeto foi criado com fins de aprendizado e boas práticas de programação.

### 📌Funcionalidades

✔️ Depósito – Adiciona valores ao saldo da conta.

✔️ Saque – Permite retirar valores, respeitando limite diário e quantidade máxima de saques.

✔️ Extrato – Mostra todas as movimentações (depósitos/saques) e o saldo final.

✔️ Menu Interativo – Interface via linha de comando.


### ⚙️ Regras de Negócio

- Depósito:

    - O valor informado deve ser positivo.

    - O depósito é registrado no extrato.

- Saque:
    
    - O valor não pode ser superior ao saldo disponível.
    - O valor não pode ultrapassar o limite de R$ 500,00 por saque.

    - O usuário pode realizar no máximo 3 saques por sessão.

    - O valor deve ser positivo.

    - Cada saque é registrado no extrato.

- Extrato:

    - Exibe todas as movimentações realizadas.

    - Caso não existam movimentações, informa que nenhuma operação foi registrada.

    - Sempre mostra o saldo atualizado.

### 📂 Estrutura do Código

- saldo → armazena o valor atual disponível na conta.
- limite → define o valor máximo permitido por saque (R$ 500).
- extrato → armazena o histórico de depósitos e saques.
- numero_saques → contador de saques realizados.
- LIMITE_SAQUES → número máximo de saques permitidos (3 por sessão).
- menu → string que apresenta as opções disponíveis para o usuário.

### ▶️ Como Executar

1. Certifique-se de ter o Python 3.x instalado.
2. Execute no terminal:
```shell
 python3 desafio_bancario.py
```