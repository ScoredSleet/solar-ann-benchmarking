# Sobre as execuções sem normalização
1. Os resultados sem normalização tendem a ser inferiores aos normalizados
2. O otimizador SGD gera `nan` em seu forward com dados desnormalizados o que impede completamente o aprendizado
3. O que mostramos aqui é um exemplo de alguams execuções com datasets TMY e WB-ESMAP apenas, sem SARAH
