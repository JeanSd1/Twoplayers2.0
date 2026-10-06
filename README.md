# twoplayers2.0

Projeto estático para execução de um exploit / jailbreak para PlayStation 4 em navegador, com interface web e cache offline via `cache.appcache`.

## Descrição

Este repositório contém a estrutura web do projeto, incluindo:

- `index.html` — página inicial e verificação de firmware
- `cache.html` — página de cache / instalação do manifest
- `jb.html` — tela principal de execução do jailbreak
- `jb.js` — lógica principal do processo de jailbreak
- `core.js`, `mem.js`, `int64.js`, `ps4_offsets.js` — módulos do exploit
- `rpc_worker.js` — worker em JavaScript usado pelo fluxo de execução
- `goldhen.bin` e arquivos em `patches/` — payloads e patches auxiliares

## Objetivo

O projeto é uma interface web para preparar e disparar um exploit para PS4, com suporte para firmwares específicos e fluxo de execução via navegador.

## Requisitos

- Navegador compatível com a experiência web do projeto
- Acesso ao site em ambiente do PlayStation 4 para execução do exploit
- Firmware suportado conforme a tabela definida em `index.html` e `ps4_offsets.js`

## Como usar

1. Abra a página principal em um navegador compatível.
2. Verifique o firmware informado pelo navegador.
3. Caso o firmware seja suportado, siga a interface para iniciar o processo.
4. O site usa `cache.appcache` para cache offline.

## Observação importante

Este projeto realiza operações sensíveis e está relacionado a exploit / jailbreak de console. Use apenas em ambientes autorizados e de acordo com as leis e políticas aplicáveis.

## Estrutura principal

```text
.
├── index.html
├── cache.html
├── jb.html
├── jb.js
├── core.js
├── mem.js
├── int64.js
├── ps4_offsets.js
├── rpc_worker.js
├── cache.appcache
├── goldhen.bin
├── patches/
├── render.yaml
├── README.md
└── ...
```

## Deploy

O projeto pode ser servido como site estático. Também foi configurado um `render.yaml` para uso no Render.

## Licença

Sem licença específica definida no repositório. Verifique os arquivos do projeto antes de redistribuir.
