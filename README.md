Perfeito 😎 — aqui está o **README completo em Markdown**, pronto para copiar e colar, com **todos os detalhes do script, atalhos, plano de treino e descrição do repo**:

````markdown
# 🧠 Vim Moderno — Configuração por srhorus

**Este repo servirá para demonstrar as minhas adaptações com ArchLinux**, incluindo melhorias de produtividade no Vim e atalhos personalizados.

Este projeto fornece um **arquivo de configuração moderno do Vim** com foco em produtividade, conforto visual e atalhos intuitivos, criado através do script `instalar_vimrc.sh`.

---

## 🛠️ Instalação do Script

1. Baixe o script `instalar_vimrc.sh` no seu home (ou clone o repositório):

```bash
curl -O https://example.com/instalar_vimrc.sh
````

2. Dê permissão de execução:

```bash
chmod +x instalar_vimrc.sh
```

3. Execute o script:

```bash
./instalar_vimrc.sh
```

> O script faz backup automático do `.vimrc` antigo, cria um novo `.vimrc` com tema escuro, movimentação WASD, atalhos para copiar/colar, salvar/sair, deletar/comentar linhas e linha do cursor com cor agradável.

---

## 🎨 Tema

* Tema escuro inspirado em **Gruvbox**
* CursorLine destacado com **cor mais agradável aos olhos**
* Barra de status e números configurados para fácil visualização

---

## ⌨️ Atalhos principais

### Salvar e sair

| Ação          | Atalho                 |
| ------------- | ---------------------- |
| Salvar        | `Ctrl+S` ou `<Space>w` |
| Sair          | `Ctrl+Q` ou `<Space>q` |
| Salvar e sair | `<Space>x`             |

### Copiar e colar

| Ação           | Atalho                          |
| -------------- | ------------------------------- |
| Copiar linha   | `Ctrl+C` (modo normal)          |
| Copiar seleção | `Ctrl+C` (modo visual)          |
| Colar          | `Ctrl+V` (modo normal/inserção) |

### Movimentação (WASD)

| Tecla       | Função                 |
| ----------- | ---------------------- |
| W           | Subir linha            |
| S           | Descer linha           |
| A           | Mover para esquerda    |
| D           | Mover para direita     |
| Ctrl+A      | Início da linha        |
| Ctrl+D      | Fim da linha           |
| A (Shift+A) | Ir para final da linha |

### Linhas relativas

* Números à esquerda indicam **distância relativa da linha atual**
* Exemplo: `3S` → desce 3 linhas, `2W` → sobe 2 linhas
* Útil para movimentos, deletar e copiar múltiplas linhas

### Deletar e comentar linhas

| Ação                     | Atalho                   |
| ------------------------ | ------------------------ |
| Deletar linha atual      | `dd`                     |
| Deletar múltiplas linhas | `3dd`                    |
| Comentar linha           | `<Space>c`               |
| Comentar seleção         | `<Space>c` (modo visual) |

### Explorer / Splits

| Ação                 | Atalho           |
| -------------------- | ---------------- |
| Abrir Explorer       | `<Space>e`       |
| Split vertical       | `<Space>sv`      |
| Split horizontal     | `<Space>sh`      |
| Navegar entre splits | `<Space>h/j/k/l` |

### Recarregar configuração

| Ação                | Atalho     |
| ------------------- | ---------- |
| Recarregar `.vimrc` | `<Space>r` |

### Criar novo arquivo / buffer

| Ação              | Atalho     |
| ----------------- | ---------- |
| Criar novo buffer | `<Space>n` |

---

## ✨ Funcionalidades do Script

* Backup automático do `.vimrc` antigo
* Tema escuro com linha do cursor mais agradável
* Movimentação **WASD**
* Atalhos para **copiar/colar** linhas ou seleção (`Ctrl+C/V`)
* Atalhos para **salvar/sair** (`Ctrl+S/Q`)
* Atalhos para **deletar e comentar linhas**
* Atalho para ir **ao final da linha** (`A`)
* Atalho para **criar novo buffer** (`<Space>n`)
* Sem pisca da tela (`novisualbell`)

---

## 📖 Como treinar os atalhos

### Dia 1 — Movimentação básica com WASD

* Abra um arquivo de treino:

```bash
vim ~/vim_treino.txt
```

* Use apenas **W/S** para subir/baixo e **A/D** para esquerda/direita.
* Experimente ir para o início e fim de linhas (`Ctrl+A` / `Ctrl+D`).

### Dia 2 — Linhas relativas

* Ative linhas relativas (já está no seu `.vimrc`):

```vim
:set relativenumber
```

* Pratique movimentos combinando **W/S** + números relativos:

  * `2S` → desce 2 linhas
  * `3W` → sobe 3 linhas

### Dia 3 — Copiar linhas

* Copie a linha atual: `Ctrl+C`
* Copie várias linhas usando seleção visual:

  1. `V` → selecionar linha
  2. `3S` → selecionar mais linhas
  3. `Ctrl+C` → copiar
* Cole em outro ponto: `Ctrl+V`

### Dia 4 — Deletar linhas

* Delete a linha atual: `dd`
* Delete múltiplas linhas: `3dd`
* Delete usando seleção visual:

  1. `V` → selecionar linha
  2. `3S` → expandir seleção
  3. `d` → deletar

### Dia 5 — Salvar e sair

* Salvar arquivo: `Ctrl+S` ou `<Space>w`
* Sair: `Ctrl+Q` ou `<Space>q`
* Salvar e sair: `<Space>x`

### Dia 6 — Combinação avançada

* Misture tudo:

  1. Movimente o cursor usando **WASD + números relativos**
  2. Copie linhas (`Ctrl+C`) e cole (`Ctrl+V`)
  3. Delete linhas com `dd` ou visual + `d`
  4. Salve (`Ctrl+S`)

### Dia 7 — Mini desafio

* Abra um arquivo de 20–30 linhas.
* Tarefas:

  1. Vá para a metade do arquivo usando **WASD + números relativos**
  2. Copie 3 linhas e cole no final
  3. Delete 2 linhas do início
  4. Comente uma linha com `<Space>c`
  5. Crie uma linha nova (`<Space>n`) e escreva algo
  6. Salve e saia (`Ctrl+S` + `<Space>q`)

> Objetivo: usar todos os atalhos do seu `.vimrc` moderno de forma fluida.

---

## 📌 Referências

* [Vim Official Documentation](https://vimhelp.org/)
* [Gruvbox Theme](https://github.com/morhetz/gruvbox)

```

---

Se você quiser, posso criar **uma versão em Markdown tipo cheatsheet visual**, mostrando **todos os atalhos do seu Vim moderno**, pronta para abrir dentro do Vim ou imprimir para treino rápido.  

Quer que eu faça isso?
```
