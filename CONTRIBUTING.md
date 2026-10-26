# Contribuir com música para o DinoMusic

O DinoMusic aceita álbuns e faixas da comunidade, mas todo o conteúdo tem de ser seguro para crianças e ter direitos de utilização claros.

## Estrutura

Cria uma pasta única em `content/albums/<album-id>/`:

```text
content/albums/o-meu-album/
  covers/faixa-um.png
  tracks/faixa-um.mp3
```

Depois adiciona o álbum e as faixas a `catalog.json`. Usa identificadores minúsculos com hífen, caminhos relativos e uma das categorias: `dance`, `play`, `relax`, `sleep` ou `family`.

## Requisitos

- MP3 até 15 MB por faixa, sem publicidade, mensagens comerciais ou áudio oculto.
- Capa PNG quadrada, com pelo menos 512 × 512 px, sem marcas de terceiros.
- Idioma suportado (`pt-PT`, `pt-BR`, `en`, `fr`, `de`, `es`, `pl`) ou `all` para instrumental/universal.
- Uma das quatro faixas etárias oficiais: `0-2`, `3-5`, `6-10` ou `11-16`.
- Título, descrição, autoria e licença verdadeiros e completos.
- Letras são opcionais. Quando existem, devem corresponder exatamente ao áudio.
- Não são permitidos conteúdos violentos, sexuais, discriminatórios, assustadores, recolha de dados, links, publicidade ou infrações de direitos de autor.

## Licença e revisão

Ao contribuir, declaras que tens autorização para distribuir o áudio e a imagem no DinoMusic. A primeira versão de um novo álbum exige revisão humana. Atualizações posteriores passam pelas verificações automáticas e pelas regras de proteção do repositório.

## Testes obrigatórios

```bash
node scripts/validate.mjs
node scripts/validate-content.mjs
```

Usa o modelo do pull request e indica a origem do áudio, da capa, a licença, idioma, idade e se a música contém voz.
