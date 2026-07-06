# Gerência de Configuração - Recomendador de Grade Acadêmica

## Repositório

- Nome sugerido: `recomendador-grade-academica`
- URL: https://github.com/OPedroTxr/recomendador-grade-academica
- Branches permanentes: `main` e `develop`.

## Fluxo

1. Registrar demanda em uma GitHub Issue.
2. Criar branch a partir de `develop`:
   - `feature/USxx-descricao`
   - `fix/issue-n-descricao`
   - `hotfix/x.y.z`
3. Implementar e testar.
4. Fazer commits claros.
5. Abrir Pull Request para `develop` (ou para `main` em release/hotfix).
6. Exigir revisão e CI antes do merge.
7. Fechar a issue e mover o cartão no GitHub Project.

## Convenção de commits

- `feat(escopo): nova funcionalidade`
- `fix(escopo): correção`
- `docs(escopo): documentação`
- `test(escopo): teste`
- `refactor(escopo): refatoração`
- `chore(escopo): manutenção`

Exemplo:

```text
feat(recomendacao): calcular prioridade de disciplinas gargalo
```

## Versionamento

Usar SemVer e tags Git:

- `v0.1.0`: requisitos e protótipos.
- `v0.2.0`: diagramas de projeto.
- `v0.3.0`: núcleo funcional.
- `v1.0.0-rc.1`: candidata à entrega.
- `v1.0.0`: entrega estável.

## Controles obrigatórios

- Não fazer push direto para `main`.
- Nunca versionar `.env`, tokens, senhas ou dados reais de alunos.
- Versionar scripts de migração, não backups do banco.
- Vincular issue, branch, commits e pull request.
- Criar GitHub Release para cada linha de base importante.
