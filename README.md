# 🛡️ Cyber Diagnostic IA: Detecção de Intrusão em Redes

Este projeto utiliza **Inteligência Artificial (Machine Learning)** para identificar automaticamente tentativas de ataques em tráfego de rede. O sistema foi treinado com dados 
reais de cibersegurança e é capaz de distinguir entre atividades normais e ameaças maliciosas com alta precisão.

---

## 🚀 Resultados do Projeto (Resumo Executivo)

O modelo foi submetido a um teste rigoroso com **23.900 novos registros de ataque** de tráfego que ele nunca havia visto antes.

* **Taxa de Acerto Geral (Acurácia):** 95.06%
* **Eficiência na Detecção de Ataques:** 97.6% (O modelo barrou 23.317 ataques reais).
* **Tempo de Resposta:** O sistema analisa milhares de pacotes em menos de 7 segundos.

> **Nota para Gestores:** Este diagnóstico permite que uma equipe de segurança (SOC) foque apenas nos 2.4% de alertas mais complexos, automatizando a triagem da grande massa de
>  dados e reduzindo drasticamente o tempo de exposição a riscos.

---

### 📊 Principais Pistas de Ataque

![Top 10 pistas](/img/Top10_Pistas.png)


---

### 🛡️ Eficiência por Tipo de Ameaça

![Relatorio_Eficiencia_da_IA](/img/Relatorio_Eficiencia_da_IA.png)

---

## 📊 O que a IA está analisando? (Pistas de Ataque)

Diferente de sistemas comuns, nossa IA aprendeu a identificar padrões suspeitos. O gráfico abaixo (gerado no projeto) mostra as características mais importantes para a decisão:

1.  **Tempo de Resposta do Servidor:** Atrasos anormais na resposta.
2.  **Taxa de Download/Upload:** Volumes de dados desproporcionais.
3.  **Tamanho Médio de Pacotes:** Padrões de dados que não condizem com uso humano normal.

---

## 🛠️ Tecnologias Utilizadas

* **Linguagem:** Python 3.12
* **Ambiente:** VS Code (Jupyter Notebooks)
* **Processamento de Dados:** Pandas & FastParquet (para lidar com grandes volumes)
* **Inteligência Artificial:** Scikit-Learn (Algoritmo *Random Forest*)
* **Visualização de Dados:** Matplotlib & Seaborn

---

## 📂 Processo de Desenvolvimento

1.  **Carga de Dados Reais:** Utilização do dataset **UNSW-NB15**, contendo mais de 170.000 registros de tráfego real.
2.  **Tratamento de Dados:** Conversão de linguagens técnicas de rede em formatos matemáticos que a IA entende (*One-Hot Encoding*).
3.  **Padronização:** Ajuste de escalas para que dados pequenos e grandes tenham a mesma importância na análise.
4.  **Treinamento:** Uso do algoritmo *Random Forest Classifier*, utilizando múltiplos núcleos de processamento para máxima velocidade.
5.  **Relatório de Incidentes:** Criação de visualizações amigáveis que traduzem termos técnicos (como *Fuzzers* ou *Backdoors*) para linguagem de negócios.

---

### Bibliotecas necessárias

pip install pandas scikit-learn matplotlib seaborn fastparquet

### Execute o arquivo .ipynb dentro do VS Code

Desenvolvido por: Rafael Silva Guimarães 'guimaraesdevweb@gmail.com'
Objetivo: Demonstrar o poder da IA aplicada à Defesa Cibernética.