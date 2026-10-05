# Regressão Linear Múltipla para Estimativa de Esforço de Software

Trabalho acadêmico do curso de Engenharia de Software (SENAI).

## Sobre a atividade

Uma empresa de engenharia de software quer abandonar estimativas
puramente subjetivas (baseadas em "chute" ou planning poker sem calibração)
e adotar uma abordagem quantitativa para prever o Esforço de Desenvolvimento
(em horas-homem). Como equipe de engenharia, vocês devem construir, auditar
e validar um modelo de Regressão Linear Múltipla para estimar Y (Horas de
Desenvolvimento) a partir de métricas do sistema.
Utilizando a base de dados informada (NASA93), considere as seguintes
variáveis:
• Y (Horas_Dev): Variável dependente (target).
• X1
(Linhas_Codigo_KLOC): Milhares de linhas de código estimadas.
• X2
(Complexidade_Ciclomatica_Media): Complexidade ciclomática
média das funções/módulos.
• X3
(Pontos_Funcao): Pontos de função não ajustados.
• X4
(Experiencia_Equipe_Anos): Média de anos de experiência dos
desenvolvedores envolvidos.
• X5
(Num_Integracoes_Externas): Quantidade de APIs/sistemas legados
integrados.

Etapa 1: Análise Exploratória e Matriz de Correlação
1. Carregar a base de dados e exibir estatísticas descritivas (média, desvio
padrão, percentis).
2. Gerar uma matriz de correlação com heatmap para identificar como cada
métrica se relaciona com as horas de desenvolvimento e se existem
variáveis explicativas altamente correlacionadas entre si.

Etapa2: Treinamento e Interpretação Estatística
1. Dividir os dados em Treino (80%) e Teste (20%) com semente
pseudoaleatória fixada (random_state=42).
2. Ajustar o modelo utilizando para inspeção estatística detalhada:
o Analisar o R²
3. Treinar o mesmo modelo com o scikit-learn (LinearRegression) e calcular
métricas de teste:
o MAE (Mean Absolute Error)
o RMSEP (Root Mean Squared Error)
