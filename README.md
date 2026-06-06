# Space Connect - Global Solution (Dynamic Programming)

O **Space Connect** é um sistema interativo desenvolvido em Python para otimizar a conexão de dados entre estações terrestres 
e uma constelação de satélites em órbita. Este projeto faz parte da entrega da **Global Solution**, com foco na aplicação 
prática de lógica de programação e algoritmos de otimização.

---

##Integrantes
* **Caio Berardo de Araújo**      — RM: 560357
* **Giovanni Romano Provazi**     — RM: 560434
* **Guilherme Augusto Caseiro**   — RM: 559765
* **Leonardo Fernandes Mesquita** — RM: 559623
* **Vitor de Lima Domingues**     — RM: 561008

---

## Objetivo

Em operações aeroespaciais, a comunicação eficiente e resiliente entre bases na Terra e redes de satélites é crítica. O envio de
dados pode falhar se o satélite escolhido estiver muito distante ou sem energia suficiente para sustentar a transmissão.

O **Space Connect** resolve esse desafio simulando uma malha logística espacial. O sistema calcula a **Distância Euclidiana**
entre a estação terrestre e os satélites disponíveis em um plano cartesiano bidimensional e aplica regras de negócio 
automatizadas para escolher o melhor ponto de conexão.

### Regras de Negócio Implementadas:
1. **Filtro de Confiabilidade de Energia:** Satélites com nível de bateria inferior a 20% são automaticamente descartados
   da busca por segurança operacional.
2. **Critério de Proximidade Espacial:** Dentre os satélites com bateria suficiente, o algoritmo seleciona aquele com a
   menor distância geométrica em relação à estação.

---

## Funcionabilidade

O software opera em modo de linha de comando (CLI) totalmente interativo, oferecendo o seguinte menu:

* `[1] Cadastrar Novo Satélite`: Adiciona novos dispositivos à rede, coletando nome, coordenadas espaciais $(X, Y)$ e nível de
  bateria atual.
* `[2] Listar Constelação Atual`: Exibe o relatório de todos os satélites integrados na rede com suas respectivas posições e
   cargas de bateria.
* `[3] Otimizar Conexão com Estação Terrestre`: O usuário insere as coordenadas de uma base terrestre e o sistema calcula e
  aponta em tempo real qual é o satélite ideal para estabelecer a transmissão.
* `[0] Sair do Sistema`: Encerra a execução do programa com segurança.
  entre cada seleção se preciona a tecla enter para "resetar"

---

## Execução
O projeto foi feito pelo google collab, segue link abaixo:
https://colab.research.google.com/drive/1iZOii2y1HoxVLXkEyDZkBaAlul-Lhyrd?usp=sharing
