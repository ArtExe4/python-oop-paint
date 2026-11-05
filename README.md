# 🎨 Python OOP Paint Application

Aplicação gráfica desktop para criação e manipulação de desenhos vetoriais e formas geométricas, desenvolvida em **Python** com foco estrito em **Programação Orientada a Objetos (POO)**, princípios **SOLID** e aplicação prática de **Design Patterns (GoF)**.

---

## 🏗️ Arquitetura e Padrões de Projeto Utilizados

O sistema foi projetado para ser altamente desacoplado, extensível e de fácil manutenção, utilizando os seguintes padrões arquiteturais:

- **MVC (Model-View-Controller):** Separação clara entre a lógica de dados das figuras geométricas (*Model*), a interface gráfica de renderização (*View*) e o gerenciamento de eventos do usuário (*Controller*).
- **State Pattern:** Gerenciamento dinâmico do comportamento das ferramentas de desenho (seleção, criação de formas, pintura, exclusão) sem o uso de condicionais complexas (`if/elif` extensos), alterando o estado ativo do canvas conforme a ferramenta selecionada.
- **Composite Pattern:** Tratamento unificado de objetos individuais (linhas, retângulos, círculos) e composições de figuras agrupadas, permitindo manipular camadas e grupos de elementos de forma recursiva.
- **Command Pattern:** Encapsulamento das ações de desenho e modificação como objetos de comando independentes, viabilizando o controle de histórico de ações (*Undo / Redo*).

---

## 📂 Estrutura do Projeto

* `src/paint_mvc/` — Código-fonte principal (Models, Views, Controllers e Patterns)
* `tests/` — Testes automatizados e validação das regras de negócio
* `.gitignore` — Ignora arquivos de cache e compilação do Python
* `README.md` — Documentação técnica do projeto

---

## 🚀 Como Executar Localmente

1. **Clone o repositório:**
   `git clone [https://github.com/ArtExe4/python-oop-paint.git](https://github.com/ArtExe4/python-oop-paint.git)`
   `cd python-oop-paint`

2. **Execute a aplicação:**
   `python src/paint_mvc/main.py`

---

## 🛠️ Tecnologias Utilizadas

- **Linguagem:** Python 3
- **Paradigma:** Programação Orientada a Objetos (POO)
- **Arquitetura:** MVC + Design Patterns (State, Composite, Command)
