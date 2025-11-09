# 📝 Task Manager App

Um aplicativo simples feito em **React Native com Expo**, integrado a um **JSON Server**, para gerenciar uma lista de tarefas.  
O sistema permite **criar**, **marcar como concluídas**, **arquivar** e **excluir** tarefas de forma prática e intuitiva.

---

## 🚀 Tecnologias Utilizadas

- **React Native (Expo)** — Framework principal do aplicativo  
- **React Navigation (Stack)** — Gerenciamento de telas  
- **Axios** — Comunicação com o backend  
- **JSON Server** — Simulação de banco de dados REST  
- **Styled Components** — Estilização  
- **ActivityIndicator** — Feedback visual durante carregamentos  

---

## ⚙️ Funcionalidades

### Criar Tarefas
- Tela dedicada à criação de novas tarefas.  
- Campos:
  - **Nome da tarefa** (obrigatório)
  - **Descrição** (opcional)  
- Botão **“Criar Tarefa”** envia os dados para o JSON Server via `POST`.  
- Após criar, o usuário é redirecionado automaticamente para a tela de gerenciamento.
### Gerenciar Tarefas
- Lista todas as tarefas não arquivadas.
- Exibe nome, estado e botões de ação:
- ✅ Concluir/Reabrir — alterna o valor de completed (PATCH)
- 📦 Arquivar — define archived = true (PATCH)
- As tarefas concluídas aparecem com o texto riscado.
- Botão “Ver Arquivadas” leva à tela de tarefas arquivadas.
- Botão “Nova Tarefa” leva à tela de criação.
### Gerenciar Tarefas
- Tela de Criação de Tarefas
- Criar nova tarefa
- Botão “Ver Minhas Tarefas” → vai para a Tela de Gerenciamento
- Tela de Gerenciamento
- Exibe lista de tarefas
- Botão “Nova Tarefa” → volta à Tela de Criação
- Botão “Ver Arquivadas” → vai para a Tela de Arquivadas
- Tela de Arquivadas
- Exibe tarefas arquivadas
- Botão “Voltar” → retorna à Tela de Gerenciamento

  

**Estrutura da tarefa criada:**
```json
{
  "id": 1,
  "name": "Exemplo de tarefa",
  "description": "Descrição opcional",
  "completed": false,
  "archived": false
}
```

---

#### Como rodar o sistema

depois de clonar, entre no diretorio e digite no terminal: npm run web e npx json-server --watch db.json
