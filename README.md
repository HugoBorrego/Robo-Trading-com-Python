# Projeto de Simulação de Robô de Negociação

## Visão Geral
 Este repositório contém uma simulação de um robô de negociação desenvolvido em Python, que utiliza o algoritmo de aprendizado por reforço Q-Learning. O objetivo deste projeto é servir como um experimento de aprendizado e demonstrar meus conhecimentos em conceitos de aprendizado de máquina, estratégias de negociação financeira e programação em Python.

 O robô de negociação é treinado para tomar decisões sobre comprar, vender ou manter ações com base em dados históricos de preços. Ao interagir com o ambiente (representado pelos preços das ações) e receber recompensas por ações lucrativas, o robô aprimora sua tomada de decisões ao longo do tempo.

### Como Funciona
### Conceitos-Chave:
- Gráfico de Candlestick: Com a biblioteca plotly, é gerado um gráfico de candlestick para visualizar as tendências dos preços das ações ao longo do tempo.
- Algoritmo Q-Learning: Um algoritmo de aprendizado por reforço usado para atualizar uma tabela Q, que serve como memória das melhores ações a serem tomadas em diferentes estados.
- Ambiente: O cenário de negociação inclui ações (comprar, vender, manter), um saldo inicial e os preços das ações como estados.
- Treinamento do Agente: O robô é treinado ao longo de vários episódios, aprendendo por tentativa e erro a maximizar os lucros.
- Execução: Após o treinamento, o robô utiliza a tabela Q para executar negociações no ambiente de teste.

### Componentes Principais:
#### Configuração de Hiperparâmetros:
- Número de episódios (num_episodios)
- Taxa de aprendizado (alfa)
- Fator de desconto (gama)
- Taxa de exploração (epsilon)

#### Processo de Q-Learning:
- Inicializar a tabela Q.
- Realizar ações com base em exploração ou exploração do conhecimento.
- Atualizar os valores da tabela Q com base na recompensa e próximo estado.

#### Execução das Ações:
- Comprar: Comprar ações se houver saldo suficiente.
- Vender: Vender ações se houver ações disponíveis.
- Manter: Manter o estado atual sem realizar negociações.

#### Cálculo do Lucro:

- Avaliar o desempenho do agente calculando o lucro final com base no saldo final e nas ações restantes.

#### Aviso:
Este projeto é destinado apenas para fins educacionais, para testar e aprimorar meus conhecimentos em aprendizado por reforço e negociação algorítmica. Não é destinado para conselhos financeiros reais ou implementação prática.
