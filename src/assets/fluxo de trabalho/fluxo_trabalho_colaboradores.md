
# 🌟 **Documentação de Fluxo de Trabalho para Colaboradores**

### Objetivo: Organizar o fluxo de trabalho no repositório de forma eficiente, permitindo que todos os colaboradores contribuam sem afetar a branch principal (`main`), utilizando branches de trabalho e sub-branches para funcionalidades específicas.

---

## 🚀 **Passo a Passo para Trabalhar nas Branches**

### 1. **Clonar o Repositório (se ainda não fez)**

Se você ainda não tem o repositório clonado localmente, siga o comando abaixo:

```bash
git clone https://github.com/seu-usuario/seu-repo.git
cd seu-repo
```

---

### 2. **Garantir que a `main` e as Branches Estão Atualizadas**

Antes de começar a trabalhar, é importante garantir que sua branch `main` esteja atualizada. Siga os passos abaixo para garantir que você está com as versões mais recentes de todas as branches:

1. **Atualizar a `main` local**:

```bash
git checkout main        # Vai para a branch main
git pull origin main     # Atualiza a main com as mudanças do GitHub
```

2. **Mudar para a sua branch de trabalho** (por exemplo, `colaborador1`):

```bash
git checkout nome-da-branch
```

Exemplo:

```bash
git checkout colaborador1
```

---

### 3. **Criar Sub-Branches para Novas Funcionalidades (se necessário)**

Se precisar adicionar uma nova funcionalidade, crie uma **sub-branch** para que seu trabalho não afete as outras partes do projeto.

1. **Criar uma nova branch para a funcionalidade**:

```bash
git checkout -b nome-da-feature
```

Exemplo:

```bash
git checkout -b feature/login
```

2. **Subir a sub-branch para o GitHub** (quando for começar a trabalhar):

```bash
git push -u origin nome-da-feature
```

---

### 4. **Trabalhar nas Alterações**

Agora que você tem uma branch ou sub-branch para trabalhar, siga os passos para adicionar e commitar suas alterações:

1. **Adicionar alterações**:

```bash
git add .              # Adiciona todas as alterações
```

2. **Comitar as mudanças**:

```bash
git commit -m "descrição do que foi alterado"
```

3. **Subir para o GitHub**:

```bash
git push origin nome-da-feature
```

---

### 5. **Manter a Branch Atualizada com a `main`**

Outros colaboradores podem estar atualizando a `main` ou outras branches, então é importante que você mantenha sua branch de trabalho sincronizada com a `main`.

1. **Voltar para a `main` e atualizar**:

```bash
git checkout main
git pull origin main
```

2. **Voltar para a sua branch e fazer o merge da `main`**:

```bash
git checkout nome-da-branch
git merge main           # Mescla as mudanças da main na sua branch
```

Ou, se preferir usar **rebase** (para limpar o histórico de commits):

```bash
git checkout nome-da-branch
git rebase main
```

---

### 6. **Finalizar o Trabalho e Subir para a `main`**

Quando a tarefa ou feature estiver pronta, siga os passos abaixo para finalizar e subir as alterações para a `main`.

1. **Comitar pela última vez na branch** de trabalho (caso haja alterações adicionais):

```bash
git add .
git commit -m "Finaliza a tarefa de [descrição]"
```

2. **Subir as alterações** para a sua branch de trabalho no GitHub (se ainda não tiver feito isso):

```bash
git push origin nome-da-branch
```

3. **Mudar para a `main`**:

```bash
git checkout main
```

4. **Mesclar as alterações da sua branch** na `main`:

```bash
git merge nome-da-branch
```

5. **Subir a `main` para o GitHub**:

```bash
git push origin main
```

---

## 🌟 **Fluxo Ideal para Colaboradores**

1. **Trabalhe sempre em uma branch separada da `main`**.
2. **Crie sub-branches** para novas funcionalidades a partir das suas branches.
3. **Nunca faça commits na `main`**.
4. **Sincronize sua branch regularmente com a `main`**.
5. **Comite pela última vez em sua branch** quando terminar o trabalho.
6. **Suba suas branches** para o GitHub.
7. **Faça o merge da sua branch na `main`** e depois faça o push na `main`.

---

### 🚨 **Observações Importantes**:

- **Nunca faça commits diretamente na `main`**. Todas as alterações devem ser feitas em branches de trabalho ou sub-branches para garantir que o fluxo de desenvolvimento seja organizado e sem conflitos.
- **Comite todas as alterações de forma clara** e com mensagens descritivas. Isso ajuda na revisão e no entendimento do que foi feito.
- **Sempre que terminar sua tarefa**, não se esqueça de **comitar pela última vez** na sua branch antes de mesclar na `main`.
- **Antes de mesclar sua branch na `main`**, é essencial garantir que sua branch esteja **atualizada com a `main`**, para evitar conflitos durante o merge.

---

Com este fluxo de trabalho, garantimos que todos possam contribuir de forma eficiente e organizada, evitando conflitos e mantendo o projeto em um estado sempre funcional.

---

Se tiver dúvidas ou precisar de mais informações, estou à disposição para ajudar! 😊
