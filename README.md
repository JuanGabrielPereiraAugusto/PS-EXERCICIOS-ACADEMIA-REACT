# 🏋️ Catálogo de Exercícios de Academia — React

Aplicação feita com **React 18** e **Tailwind CSS** para a disciplina de **Programação de Scripts** na **Fatec Taquaritinga**. Ela permite **buscar, filtrar, cadastrar e ver detalhes** de exercícios de musculação.

🌐 **Página:** [`index.html`](index.html)

---

## ✨ Funcionalidades

| Função | Como funciona |
|---|---|
| 🔎 **Busca por nome** | Filtra a lista enquanto você digita |
| 🎯 **Filtro por grupo muscular** | Peito, Pernas, Braços, Costas ou Ombros |
| 📊 **Filtro por dificuldade** | Fácil, Médio ou Difícil |
| ➕ **Cadastro de exercício** | Nome, grupo, dificuldade e descrição, com validação |
| 🪟 **Ver Detalhes** | Abre um modal com a descrição do exercício |
| 📭 **Lista vazia** | Mostra "Nenhum exercício encontrado..." quando nada combina com o filtro |

Já vem com **10 exercícios** cadastrados (supino, agachamento, rosca direta, remada, elevação lateral e outros).

---

## 🧠 Conceitos de React aplicados

| Conceito | Onde aparece |
|---|---|
| **Componentes** | `App` e `Modal` |
| **Estado (`useState`)** | Busca, filtros, lista de exercícios, campos do formulário e modal |
| **Formulário controlado** | `value` + `onChange` em todos os campos |
| **Imutabilidade** | `setExercicios([...exercicios, novo])` |
| **Renderização de listas** | `filtrados.map(...)` com `key` |
| **Renderização condicional** | Modal só aparece quando há item selecionado |
| **Filtros combinados** | `.filter()` com nome, tipo e dificuldade ao mesmo tempo |

```jsx
const filtrados = exercicios.filter((e) => {
  const nomeOK = e.nome.toLowerCase().includes(search.toLowerCase());
  const tipoOK = tipoFiltro === "Todos" || e.tipo === tipoFiltro;
  const difOK  = difFiltro  === "Todos" || e.dificuldade === difFiltro;
  return nomeOK && tipoOK && difOK;
});
```

---

## 🛠️ Tecnologias

- **React 18** e **ReactDOM** (via CDN)
- **Babel Standalone**, que converte o JSX direto no navegador
- **Tailwind CSS 2**, para o visual em tema escuro

---

## 🚀 Como ver

- **Online:** ative o **GitHub Pages** (Settings → Pages → Branch `main` → Save).
- **No computador:** baixe o repositório e abra o `index.html` no navegador (precisa de internet para carregar o React e o Tailwind).

---

## 🎓 Informações acadêmicas

| | |
|---|---|
| **Instituição** | Fatec Taquaritinga |
| **Curso** | Análise e Desenvolvimento de Sistemas |
| **Disciplina** | Programação de Scripts |
| **Professor** | Giuliano Scombatti Pinto |

## 👤 Autor

**Juan Gabriel Pereira Augusto**
GitHub: [@JuanGabrielPereiraAugusto](https://github.com/JuanGabrielPereiraAugusto)
