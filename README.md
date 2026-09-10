<div align="center">
  <h1>📈 Calculadora do Lugar das Raízes (LGR)</h1>
  <p><strong>Ferramenta didática interativa para cálculo e visualização do algoritmo Root Locus em 12 passos.</strong></p>
  
  [![Acessar Aplicação](https://img.shields.io/badge/Acessar-Streamlit_App-FF4B4B?style=for-the-badge&logo=streamlit)](controlcalc.streamlit.app)
  [![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)](#)
  [![SymPy](https://img.shields.io/badge/SymPy-336699?style=for-the-badge&logo=python&logoColor=white)](#)
</div>

---

## Sobre o Projeto

Este projeto é uma aplicação web desenvolvida em **Streamlit** com o objetivo de destrinchar o algoritmo clássico de Controle para o desenho do **Lugar Geométrico das Raízes (LGR)** ou *Root Locus*. A ferramenta foi construída com propósito pedagógico, visando ajudar estudantes e engenheiros a visualizarem, passo a passo, como a resposta de um sistema de controle de malha fechada evolui no plano complexo $s$.

**Acesse a aplicação online:** [controlcalc.streamlit.app](https://controlcalc.streamlit.app)

---

## Demonstração da interface
  <!-- Imagem 1 -->
  <img src="imgs/demo-01.png" alt="Imagem da tela inicial">

  <!-- Imagem 2 -->
  <img src="imgs/demo-02.png" alt="Imagem da tela depois de clicar no botão de calcular, aparece a equação de malha fechada e o início do gráfico" >
</p>

  <!-- Imagem 4 -->
  <img src="imgs/demo-04.png" alt="Imagem da tela mostrando o gráfico do LGR">

  <!-- Imagem 5 -->
  <img src="imgs/demo-05.png" alt="Foto dos 12 passos recolhidos (é possível clicar em cada ítem da lista para mostrar detalhes)">

---

## Funcionamento: O Algoritmo dos 12 Passos

A aplicação divide a resolução do LGR de forma extremamente didática, seguindo os 12 passos fundamentais:

1. **Forma Padrão:** Obtenção da equação de malha fechada.
2. **Polos e Zeros:** Identificação e plotagem inicial.
3. **Número de Ramos:** Determinação da quantidade de ramos do LGR.
4. **Simetria:** Confirmação da simetria em relação ao eixo real.
5. **LGR no Eixo Real:** Regiões de existência no eixo real.
6. **Assíntotas (Ângulos):** Direção dos ramos em direção ao infinito.
7. **Ponto de Partida das Assíntotas (Centroide):** Ponto de cruzamento das assíntotas.
8. **Pontos de Quebra ou Chegada:** *Break-away* e *break-in points*.
9. **Ângulos de Partida e Chegada:** Ângulos em malha aberta para polos e zeros complexos.
10. **Cruzamento com Eixo Imaginário:** Pontos de interseção com o eixo jω (Routh-Hurwitz).
11. **Ramos de Polos para Zeros:** Mapeamento visual das conexões.
12. **Esboço Final (Gráfico):** Renderização final do lugar das raízes com o LGR completo traçado.

---

## Tecnologias Utilizadas

- **[Streamlit](https://streamlit.io/):** Responsável por toda a interface web, widgets interativos e exibição dos passos.
- **[Python](https://www.python.org/):** Linguagem base de estruturação e manipulação de fluxo.
- **[SymPy](https://www.sympy.org/):** Utilizada para a resolução simbólica e manipulação de equações algébricas e diferenciais.
- **[NumPy](https://numpy.org/) e [Matplotlib](https://matplotlib.org/):** Cálculos matriciais numéricos e plotagem vetorial dos gráficos detalhados do lugar das raízes.

---

## Execução local

Caso deseje rodar o ambiente didático em sua própria máquina, siga os passos:

1. **Clone este repositório:**
   ```bash
   git clone https://github.com/gabriel26077/gabriel_LGR.git
   cd gabriel_LGR
   ```

2. **(Recomendado) Crie um ambiente virtual:**
   ```bash
   python -m venv venv
   source venv/bin/activate  # No Windows use: venv\Scripts\activate
   ```

3. **Instale as dependências:**
   ```bash
   pip install -r requirements.txt
   ```

4. **Inicie a aplicação:**
   ```bash
   streamlit run lgr_app.py
   ```

Acesse `http://localhost:8501` em seu navegador para utilizar a ferramenta localmente.
> [!CAUTION]
> **Aviso:** É possível que existam alguns bugs. O gráfico não fica 100% fiel nos pontos de quebra e chegada, e em alguns casos pode não plotar os ramos corretamente.
