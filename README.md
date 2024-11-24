# README  

## 📊 Análises e Simulações de Portfólios com Dados de Empresas Listadas  

Este repositório contém códigos e materiais relacionados às análises e simulações numéricas realizadas com base nos dados de empresas listadas na bolsa de valores brasileira (B3) usando a metodologia Fórmula Mágica de Greenblatt, considerando aprimoramentos de Gray-Carlisle. O pipeline aqui apresentado abrange desde a filtragem inicial (*screening*) até análises detalhadas e simulações de portfólios.  

---

## 📂 Estrutura do Repositório  

1. **Google Drive - Dados Base**  
   Contém os Demonstrativos de Resultados de Exercícios (DRE) das empresas listadas na bolsa, além de outros dados essenciais para as análises.  

   **Acesse os dados aqui:** [Link para Google Drive](https://drive.google.com/drive/folders/195aD9QhEaHMTrFlThoRwkojUcPlEGGXZ?usp=sharing)  

2. **Arquivo de Screening**  
   - `economatica-screening.xlsx`:  
     Um arquivo Excel que contém informações históricas de todas as empresas que já foram listadas na B3, com as seguintes colunas:  
     - **Nome**  
     - **Classe**  
     - **Tipo de Ativo**  
     - **Ativo/Cancelado**  
     - **Bolsa/Fonte**  
     - **Volume (ajustado por inflação)**  
     - **Setor NAICS**  
     - **Data do Início da Série**  
     - **Data da Última Cotação**  
     - **Código**  

     Este arquivo é utilizado no notebook de *screening* para filtrar as empresas com base na liquidez e nos setores NAICS mencionados.  

3. **Notebooks**  
   - `screening.ipynb`:  
     Este notebook realiza a filtragem inicial das empresas com base no arquivo `economatica-screening.xlsx`.  

     **Principais funcionalidades:**  
     - Carregamento do arquivo Excel;  
     - Filtragem por liquidez (volume negociado ajustado);  
     - Seleção por setores NAICS, como **energia elétrica**, **indústria química**, entre outros.  

   - `TCC_MAIN_NOTEBOOK.ipynb`:  
     Notebook principal que realiza análises financeiras e simulações numéricas com os dados das empresas filtradas.  

     **Principais funcionalidades:**  
     - Implementação de funções para análise de portfólios;  
     - Simulações com diferentes estratégias e pesos;  
     - Visualização gráfica e geração de tabelas para interpretação dos resultados.  

---

## 🛠️ Requisitos  

Certifique-se de ter as seguintes dependências instaladas:  

- Python 3.8+  
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn  
- Scikit-learn  
- Jupyter Notebook ou JupyterLab  

Instale as dependências com o comando:  

```bash
pip install -r requirements.txt
```  

---

## 🚀 Como Utilizar  

1. **Prepare os Dados:**  
   Faça o download dos arquivos disponíveis na pasta do Google Drive (link acima). Certifique-se de incluir o arquivo `economatica-screening.xlsx` no mesmo diretório do notebook `screening.ipynb`.  

2. **Execute o Screening:**  
   - Abra e execute o `screening.ipynb` para gerar uma lista filtrada de empresas com base em critérios como liquidez e setores NAICS.  

3. **Analise e Simule:**  
   - Utilize o `TCC_MAIN_NOTEBOOK.ipynb` para realizar as análises detalhadas e simulações numéricas dos portfólios.  

---

## 📈 Exemplos de Análises  

- *Filtragem por Liquidez e Setor*: Seleção de empresas com volume negociado ajustado acima de um limite específico e pertencentes aos setores de interesse, como **energia elétrica** e **indústria química**.  
- *Simulação de Portfólios*: Testes com diferentes estratégias, como alocação por pesos fixos ou com rebalanceamento periódico.  

---

## 📜 Licença  

Este repositório é disponibilizado sob a licença [MIT](LICENSE).  

---

## 🤝 Contribuições  

Contribuições são bem-vindas! Caso tenha sugestões ou melhorias, abra uma *issue* ou envie um *pull request*.  

---

## 📬 Contato  

Se tiver dúvidas ou comentários, entre em contato:  
📧 **Gmail: felipegabriel.mecanica@gmail.com**  
🌐 **LinkedIn: https://www.linkedin.com/in/felipe-gabriel0/**  

--- 

Aproveite os códigos e análises! 🚀
