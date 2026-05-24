# Modelo base LaTeX UFC

<p align="center">
  <img src="figures/logo-ufc-horizontal.png" alt="Logo da Universidade Federal do Ceará" width="420">
</p>

Este repositório é o meu modelo base para trabalhos acadêmicos em LaTeX da Universidade Federal do Ceará (UFC). A estrutura foi organizada para facilitar a escrita, a manutenção e a reutilização em listas, relatórios, resoluções comentadas, artigos curtos e outros documentos da universidade.

## 🎯 Objetivo

- Servir como ponto de partida para novos trabalhos em LaTeX.
- Separar conteúdo, estilo, imagens e comandos em arquivos próprios.
- Manter um padrão visual com capa, sumário, cabeçalho, rodapé e organização por capítulos/seções.
- Facilitar a adaptação do projeto para diferentes disciplinas, professores e tipos de entrega.

## 📁 Estrutura do projeto

```text
.
├── main.tex
├── chapters/
│   ├── capa.tex
│   ├── questao-01.tex
│   ├── questao-02.tex
│   └── questao-03.tex
├── figures/
│   ├── logo-ufc-horizontal.png
│   └── logo-ufc.PNG
├── style/
│   ├── comandos.tex
│   └── pacotes.tex
└── README.md
```

## ✍️ Sobre este modelo

Eu montei este projeto para não precisar começar meus trabalhos em LaTeX do zero toda vez. A ideia é deixar uma base simples, organizada e fácil de adaptar para disciplinas da UFC, especialmente quando o trabalho envolve capa, questões, explicações, figuras e um PDF final bem formatado.

Sinta-se à vontade para usar como ponto de partida, modificar a estrutura, trocar os dados da capa e adaptar o estilo para o seu professor, disciplina ou tipo de entrega.

## O que tem em cada parte

### `main.tex`

É o arquivo principal. Ele junta tudo: pacotes, comandos, capa e arquivos de conteúdo. Na prática, é nele que o LaTeX começa a montar o documento final.

### `chapters/`

É onde fica o texto do trabalho. Eu prefiro separar cada questão, capítulo ou seção em um arquivo próprio, porque isso deixa o projeto bem mais fácil de editar depois.

- `capa.tex`: dados da capa, como universidade, curso, disciplina, título, autor, professor e data.
- `questao-01.tex`, `questao-02.tex`, `questao-03.tex`: arquivos de exemplo para organizar questões, resoluções ou seções do documento.

### `figures/`

Pasta para guardar imagens, gráficos, diagramas e logos. Sempre que eu preciso colocar uma figura no trabalho, deixo o arquivo aqui para evitar bagunça na raiz do projeto.

- `logo-ufc-horizontal.png`: logo horizontal da UFC, usada também neste README.
- `logo-ufc.PNG`: outra versão da logo da UFC, que pode ser usada na capa ou em outras partes do documento.

Exemplo de uso no LaTeX:

```latex
\includegraphics[width=0.5\textwidth]{figures/logo-ufc-horizontal.png}
```

### `style/`

Pasta onde ficam as configurações gerais do modelo. A intenção é separar estilo de conteúdo: o texto fica em `chapters/`, e os ajustes visuais ficam aqui.

- `pacotes.tex`: pacotes LaTeX usados no projeto.
- `comandos.tex`: comandos personalizados, cabeçalho, rodapé, espaçamentos e outros ajustes de aparência.

## 🛠️ Como eu costumo usar

1. Copio este modelo para uma nova pasta.
2. Altero os dados da capa em `chapters/capa.tex`.
3. Escrevo cada questão ou seção em um arquivo dentro de `chapters/`.
4. Se precisar de mais partes, crio novos arquivos e adiciono no `main.tex` com `\input{chapters/nome-do-arquivo}`.
5. Coloco imagens e gráficos em `figures/`.
6. Só mexo em `style/` quando quero mudar alguma coisa no visual do documento.

## ⚠️ Observação

Este modelo não tenta ser uma classe oficial da UFC. É apenas uma base prática que eu uso para deixar meus trabalhos mais organizados e com uma apresentação consistente.