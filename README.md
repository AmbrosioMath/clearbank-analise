# 🏦 Análise Financeira - ClearBank

## 📖 Descrição do Projeto
Este projeto consiste num *notebook* em Python desenvolvido para automatizar a análise de dados de transações financeiras da fintech **ClearBank**. 

Atuando como analista de dados, o objetivo deste *script* é processar um ficheiro CSV de transações com potenciais erros (campos vazios, formatos inválidos, etc.), realizar a limpeza e validação de cada registo de forma segura e calcular métricas financeiras detalhadas. Todo o código foi estruturado em funções com responsabilidades únicas e com tratamento de erros (`try/except`) para garantir que o programa não encerra de forma abrupta.

## 🚀 Como Executar
Para testar e correr este projeto, siga os passos abaixo:

1. **Ambiente:** Abra o ficheiro `.ipynb` (Notebook) através do [Google Colab](https://colab.research.google.com/) ou de um Jupyter Notebook local.
2. **Ficheiro de Dados:** Certifique-se de ter o ficheiro `transacoes.csv` criado e posicionado na mesma diretoria do *notebook*. Se estiver a utilizar o Google Colab, faça o *upload* do ficheiro de texto na aba de ficheiros (menu lateral esquerdo).
3. **Execução:** Execute todas as células do *notebook* de forma sequencial (de cima para baixo). 
4. A última célula do ficheiro é a **Célula de Execução Principal**. Ela orquestra todas as funções anteriores, processa os dados e gera os resultados finais.

## 📊 O que o Notebook Gera como Saída
Após a execução completa, o programa gera automaticamente duas saídas:

1. **Relatório Visual no Terminal:**
   - Um cabeçalho indicando o período analisado e um resumo da limpeza de dados (total de linhas lidas, transações válidas e inválidas).
   - Um **Relatório Mensal** formatado que exibe, para cada mês: Quantidade de transações, Total de Créditos, Total de Débitos, Saldo do mês, Valor Médio, Maior e Menor valor.
   - Uma secção de **Transações Suspeitas**, listando qualquer movimentação que ultrapasse o limite de R$ 10.000,00.

2. **Ficheiro de Exportação (`relatorio.json`):**
   - Um ficheiro gerado dinamicamente na mesma pasta contendo toda a análise estruturada em formato JSON (métricas mensais consolidadas e o detalhe das transações suspeitas). Este ficheiro fica pronto a ser consumido por outras aplicações ou bases de dados.
