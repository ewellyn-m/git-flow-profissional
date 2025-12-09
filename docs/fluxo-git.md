# Fluxo Git Profissional

Este é o fluxo de trabalho adotado por empresas para garantir organização, versionamento correto e colaboração eficiente.

---

## 1. Criar branch a partir de `develop`
- Todas as novas funcionalidades ou correções devem ser feitas em uma branch separada.
- Nomes padronizados:
  - `feature/nome-da-funcionalidade`
  - `hotfix/nome-do-bug`

---

## 2. Commits pequenos e semânticos
- Cada commit deve conter **uma única alteração**.
- Use mensagens claras e padronizadas:
  - `feat:` para novas funcionalidades
  - `fix:` para correções
  - `docs:` para documentação
  - `chore:` para tarefas de manutenção

---

## 3. Abrir Pull Request
- Após finalizar as alterações na branch, abra um PR para `develop`.
- Inclua descrição clara e checklist do que foi alterado.

---

## 4. Revisão e comentários
- Revisores verificam o código, sugerem melhorias e aprovam o PR.
- Objetivo: evitar bugs e manter qualidade do código.

---

## 5. Merge para `develop`
- Após aprovação, faça o merge da branch na `develop`.
- Resolva possíveis conflitos antes de subir o merge.

---

## 6. Testes
- Teste a branch `develop` após o merge para garantir que tudo funciona.

---

## 7. Merge para `main`
- Quando a versão estiver estável, faça o merge de `develop` para `main`.

---

## 8. Criar uma release
- Utilize tags e versionamento semântico:
  - `v1.0.0` – primeira versão estável
  - `v1.1.0` – novas funcionalidades
  - `v1.1.1` – correções rápidas (hotfix)
