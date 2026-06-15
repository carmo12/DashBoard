# 🚀 Space Operations Dashboard

Sistema interativo de monitoramento e alerta desenvolvido com **Arduino Uno**, lógica booleana e interface web moderna para simulação de cenários operacionais críticos.

## 📋 Sobre o Projeto

O projeto simula um sistema de monitoramento de operações espaciais capaz de identificar condições críticas a partir de múltiplas entradas digitais.

A solução combina:

* Interface web interativa
* Lógica booleana aplicada
* Circuito eletrônico com Arduino Uno
* Simulação no Tinkercad
* Tabela verdade automática
* Visualização em tempo real dos estados do sistema

---

## 🎯 Objetivo

Detectar situações de risco operacional através da análise de seis condições monitoradas:

| Variável | Descrição                     |
| -------- | ----------------------------- |
| A        | Falha de comunicação          |
| B        | Temperatura crítica           |
| C        | Baixo nível de energia        |
| D        | Falha em módulo operacional   |
| E        | Instabilidade da nave         |
| F        | Alerta do sistema inteligente |

O sistema ativa um alerta quando qualquer uma das seguintes condições é satisfeita.

## 🧮 Expressão Booleana

```text
X = (A AND B)
 OR (C AND D)
 OR (E AND F)
 OR (A AND NOT C)
```

Onde:

* X = 1 → Estado de alerta
* X = 0 → Operação normal

---

## 🔌 Hardware Utilizado

### Arduino Uno

### Entradas

| Pino | Função  |
| ---- | ------- |
| D2   | Botão A |
| D3   | Botão B |
| D4   | Botão C |
| D5   | Botão D |
| D6   | Botão E |
| D7   | Botão F |

### Saídas

| Pino | Dispositivo           |
| ---- | --------------------- |
| D12  | LED Verde (Normal)    |
| D13  | LED Vermelho (Alerta) |

### Componentes

* Arduino Uno
* 6 Push Buttons
* 2 LEDs
* 2 Resistores 220Ω
* Protoboard
* Jumpers

---

## 🖥️ Funcionalidades

### Dashboard Interativo

* Simulação das entradas em tempo real
* Atualização instantânea dos LEDs virtuais
* Exibição do estado do sistema
* Interface responsiva

### Tabela Verdade

* Geração automática das 64 combinações possíveis (2⁶)
* Identificação visual dos estados de alerta

### Circuito

* Diagrama completo do Arduino
* Pinagem documentada
* Representação dos componentes eletrônicos

### Código Arduino

* Código fonte integrado ao dashboard
* Função de cópia rápida
* Monitor Serial para depuração

---

## ⚙️ Funcionamento

### Estado Normal

Quando:

```text
X = 0
```

O sistema:

✅ Acende o LED Verde
❌ Mantém o LED Vermelho desligado

---

### Estado de Alerta

Quando:

```text
X = 1
```

O sistema:

🔴 Acende o LED Vermelho
⚫ Desliga o LED Verde

---

## 📂 Estrutura do Projeto

```text
📦 Space-Operations-Dashboard
 ┣ 📜 DashBoard_CS.html
 ┣ 📜 README.md
 ┗ 📜 space_ops_alert.ino
```

---

## 🔧 Tecnologias Utilizadas

* HTML5
* CSS3
* JavaScript
* Arduino C++
* Lógica Booleana
* SVG
* Tinkercad

---

## 🎓 Projeto Acadêmico

Desenvolvido para a disciplina de Arquitetura de Computadores e Sistemas Embarcados.

**Curso:** Ciência da Computação

---

## 📸 Demonstração

O dashboard permite:

* Acionar variáveis manualmente
* Simular cenários de falha
* Visualizar LEDs em tempo real
* Consultar a tabela verdade
* Analisar o circuito eletrônico
* Executar a simulação no Tinkercad

---

## 🚀 Como Executar

1. Clone o repositório:

```bash
git clone https://github.com/seu-usuario/space-operations-dashboard.git
```

2. Abra o arquivo:

```text
DashBoard_CS.html
```

3. Execute em qualquer navegador moderno.

---

## 📄 Licença

Projeto desenvolvido para fins educacionais e acadêmicos.
