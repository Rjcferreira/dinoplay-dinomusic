# DinoMusic

Leitor infantil da DinoPlay com biblioteca instalável por álbum, idioma e faixa etária.

## Como funciona

- A instalação começa sem nenhuma faixa de áudio.
- `catalog.json` lista o conteúdo aprovado no repositório.
- O utilizador pode instalar um álbum completo ou uma faixa individual.
- Áudio e capas escolhidos ficam guardados no dispositivo para reprodução offline.
- O catálogo online atualiza-se sem obrigar a reinstalar o leitor.
- Pesquisa e filtros por idioma e idade funcionam tanto na biblioteca como na coleção local.

O conteúdo oficial está em `content/albums/`, mas não faz parte dos `assets` do pacote base indicados em `manifest.json`.

## Desenvolvimento

```bash
node scripts/validate.mjs
node scripts/validate-content.mjs
python -m http.server 8080
```

Consulta [CONTRIBUTING.md](CONTRIBUTING.md) antes de propor música nova.
