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

### 🆕 Criar Tarefas
- Tela dedicada à criação de novas tarefas.  
- Campos:
  - **Nome da tarefa** (obrigatório)
  - **Descrição** (opcional)  
- Botão **“Criar Tarefa”** envia os dados para o JSON Server via `POST`.  
- Após criar, o usuário é redirecionado automaticamente para a tela de gerenciamento.  

**Estrutura da tarefa criada:**
```json
{
  "id": 1,
  "name": "Exemplo de tarefa",
  "description": "Descrição opcional",
  "completed": false,
  "archived": false
}
