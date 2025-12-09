# Conflitos e Resolução no Git

Este arquivo demonstra como gerar e resolver conflitos no Git.  

---

## 1. Como criar um conflito

1. Certifique-se de estar na branch `main`:

```bash
git checkout main
Abra o arquivo index.html e altere uma linha qualquer (ex.: título da página).

Faça commit da alteração:

bash
Copiar código
git add index.html
git commit -m "alteração na main"
git push origin main
Crie e acesse uma branch de funcionalidade:

bash
Copiar código
git checkout -b feature/adicionar-menu
Altere a mesma linha do arquivo index.html de forma diferente.

Faça commit da alteração:

bash
Copiar código
git add index.html
git commit -m "alteração na branch adicionar-menu"
git push origin feature/adicionar-menu
Volte para a branch main e tente fazer o merge:

bash
Copiar código
git checkout main
git merge feature/adicionar-menu
Você verá um conflito no arquivo index.html.

2. Como resolver o conflito
Abra o arquivo com conflito no VSCode ou outro editor. Você verá algo assim:

html
Copiar código
<<<<<<< HEAD
Título da main
=======
Título da branch adicionar-menu
>>>>>>> feature/adicionar-menu
Escolha qual versão manter ou combine as duas linhas.

Salve o arquivo.

Marque o conflito como resolvido e faça commit:

bash
Copiar código
git add index.html
git commit -m "resolvido conflito no index.html"
3. Como testar o merge
Após resolver o conflito, rode o projeto localmente para verificar se está funcionando corretamente:

bash
Copiar código
# No Windows
start index.html
# No Mac
open index.html
Verifique se todas as alterações desejadas estão presentes e funcionando.

✅ Merge feito com sucesso! Nenhum recurso foi quebrado.

4. Boas práticas durante conflitos
Faça commits frequentes e semânticos (feat:, fix:, docs:)

Mantenha branches curtas e específicas

Teste sempre o merge localmente antes de subir para o GitHub

Documente o processo.
