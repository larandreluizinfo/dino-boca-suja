# AGENTS.md — Dino Boca Suja 🦖🤬

## Regra obrigatória de git (vale para TODOS os agents)

> **Toda alteração feita neste repositório DEVE ser commitada e pushada.**

1. Após criar, editar, renomear ou deletar qualquer arquivo, execute OBRIGATORIAMENTE:
   ```powershell
   git status
   git diff --stat
   git add -A
   git commit -m "<tipo>: <descrição curta em pt-BR>"
   git push origin main
   ```
2. Nunca deixe alteração só local. Se `git push` falhar, tente `git pull --rebase origin main` e depois `git push` de novo. Se continuar falhando, reporte o erro no chat e NÃO finalize a tarefa como concluída.
3. Antes de cada commit, confira `git status` e `git diff` para commitar só o que foi pedido (nunca commite secrets, `.env`, tokens).
4. Mensagens de commit em pt-BR, prefixo: `feat:`, `fix:`, `chore:`, `docs:`, `style:`.
5. Branch principal: `main`. Não crie PR salvo se o usuário pedir — é commit direto + push.
6. GitHub Pages está ativo (branch `main`, pasta `/root`). Após o push, o deploy é automático em ~1-2 min.

## Projeto
- Jogo estático em `index.html` (sem build). É só abrir ou servir via Pages.
- Recorde salvo em `localStorage`.
- Dicionário de 32 palavrões EN/FR/IT no próprio `index.html`.
