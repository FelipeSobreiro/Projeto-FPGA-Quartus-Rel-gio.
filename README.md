🕒 Relógio Digital em FPGA (Altera DE2-115)

Sistema embarcado de relógio digital desenvolvido em **Verilog** (ou VHDL) utilizando a plataforma **Intel Quartus Prime** para a placa FPGA Altera DE2-115.

## 🚀 Sobre o Projeto
Este projeto implementa um relógio digital completo na placa FPGA DE2-115. O sistema faz uso de contadores síncronos, divisores de clock (para gerar a base de tempo de 1 segundo) e decodificadores para exibição dos valores em displays de 7 segmentos.

## 🛠️ Tecnologias e Ferramentas
* **Hardware:** Placa FPGA Altera DE2-115
* **Software:** Intel Quartus Prime
* **Linguagem:** Verilog / VHDL
* **Periféricos:** Displays de 7 segmentos, chaves (switches) e LEDs da placa.

## ⚙️ Arquitetura do Sistema
O projeto é dividido nos seguintes módulos principais:
1. **Divisor de Clock:** Converte o clock de alta frequência da placa (ex: 50 MHz) em um pulso de 1 Hz.
2. **Contadores:** Blocos responsáveis por contar segundos, minutos e horas (com tratamento de estouro, ex: 59 para 00).
3. **Decodificador BCD para 7 Segmentos:** Converte os valores binários dos contadores para o padrão aceso/apagado dos displays físicos da placa.
