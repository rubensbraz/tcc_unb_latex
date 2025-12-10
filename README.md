# Modelo de TCC UnB - Engenharia Elétrica (LaTeX)

Este repositório contém um modelo completo em LaTeX para a elaboração de Trabalhos de Conclusão de Curso (TCC) e Monografias, formatado especificamente para o **Departamento de Engenharia Elétrica (ENE)** da Faculdade de Tecnologia (FT) da **Universidade de Brasília (UnB)**.

O modelo já inclui a estrutura pré-textual obrigatória (Capas, Ficha Catalográfica, Folha de Aprovação) configurada conforme as normas da instituição.

### 📄 Exemplo de Resultado

Você pode visualizar o documento final compilado no link abaixo:

🔗 **[Visualizar TCC Compilado (Resultado.pdf)](https://github.com/rubensbraz/tcc_unb_latex/blob/main/Resultado.pdf)**

---

## 🚀 Funcionalidades do Modelo

* **Identidade Visual UnB:** Pacote `ft_unb.sty` customizado para gerar capas, folhas de rosto e assinaturas com as fontes e brasões oficiais.
* **Metadados Automáticos:** Configuração centralizada de título, autores, banca e datas no arquivo `configuracoes_iniciais.tex`.
* **Suporte a Códigos-Fonte:**
    * Configuração avançada do pacote `listings` para **Python**, **HTML5**, **CSS** e **JavaScript** com realce de sintaxe colorido.
    * Pacote `mcode.sty` incluído para inserção profissional de scripts **MATLAB**.
* **Normas ABNT:** Referências bibliográficas e citações configuradas via `abntex2`.
* **Elementos Gráficos:** Suporte para subfiguras (`subfigure`), marca d'água/fundo na capa (`eso-pic`) e tabelas avançadas.

## 📂 Estrutura de Arquivos

A organização do projeto foi pensada para facilitar a manutenção de textos longos e a compilação de capítulos independentes:

* **`main.tex`**: Arquivo principal que une todos os componentes. Não é necessário editar o texto aqui, apenas a ordem dos arquivos incluídos.
* **`TCC/config/`**:
    * `configuracoes_iniciais.tex`: **Comece por aqui.** Define Título, Autores, Banca, Palavras-chave e Data.
    * `pacotes.tex`: Lista de bibliotecas LaTeX importadas.
    * `ft_unb.sty`: Definições de estilo da UnB.
* **`TCC/capitulos/`**: Conteúdo textual do trabalho.
    * `introducao.tex`, `fundamentos.tex`, `metodologia.tex`, `resultados.tex`, `conclusao.tex`: Capítulos principais.
    * `resumos.tex`: Resumo em português e Abstract em inglês.
    * `dedicatoria.tex`, `agradecimentos.tex`: Elementos pré-textuais opcionais.
* **`referencias.bib`**: Arquivo de bibliografia no formato BibTeX.

## 🛠️ Como Utilizar

### No Overleaf (Recomendado)
1.  Faça um cópia do projeto e começe a editar: https://www.overleaf.com/read/gdgggwtzcksv

### Edição Local
Certifique-se de ter uma distribuição TeX instalada (TeX Live ou MiKTeX).
1.  Clone o repositório.
2.  Abra o arquivo `main.tex`.
3.  Compile a bibliografia (BibTeX) e o documento.

## 📝 Personalização Rápida

Para alterar os dados do aluno e orientador, edite `TCC/config/configuracoes_iniciais.tex`:

```latex
% Definição de Autores
\autori{Seu Nome Completo}
\autorii{Nome do Segundo Autor (se houver)}

% Título (quebrado em linhas manuais para melhor ajuste)
\titulolinhai{Seu Título Principal}
\titulolinhaii{Subtítulo do Trabalho}

% Banca
\membrodabancai{Prof. Dr. Nome do Orientador, ENE/UnB}
\membrodabancaifuncao{Orientador}
```

## 💻 Inserção de Código

O modelo permite inserir códigos de forma elegante. Exemplo:

```latex
\begin{lstlisting}[language=Python]
# Exemplo de código Python
def analisar_conversa(caminho):
    df = carregar_dados(caminho)
    return df.describe()
\end{lstlisting}
```

## 📄 Licença e Créditos

Este modelo é de uso livre.

Autores do Modelo:

* Matheus Noschang de Oliveira
* Rubens Saito Mira Braz
