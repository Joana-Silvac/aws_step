O QUE É AWS STEP FUNCTIONS?
Definição Simples:
Serviço de ORQUESTRAÇÃO de workflows

Coordena múltiplos serviços AWS em uma sequência

Gerencia o estado da aplicação durante todo o processo

Analogia:
Como um chef de cozinha coordenando vários cozinheiros

Cada um faz sua parte, mas o chef garante que tudo aconteça na ordem certa

---ARQUITETURA E COMPONENTES
1. State Machine (Máquina de Estado)
É o WORKFLOW principal

Define todos os passos do processo

Exemplo: ins.json



 TIPOS PRINCIPAIS:
-Task State (Estado de Tarefa)
Faz alguma coisa (executa código)

Chama Lambda, ECS, etc.

--Choice State (Estado de Escolha)
-Toma decisões baseado em dados

Como um "if/else" do workflow

---Wait State (Estado de Espera)
Espera um tempo determinado

Útil para aprovações humanas

--Parallel State (Estado Paralelo)
Executa várias tarefas ao mesmo tempo

--Pass State (Estado de Passagem)
Só passa dados sem processar

Modifica o JSON que trafega