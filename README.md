# Painel de Senhas

Painel de senhas da sala de vacina: recepção, TV com chamada por voz, relatório de tempo de espera e configurações. Funciona no celular, no computador e na TV.

## Links

- Recepção: `https://luucashl095-ui.github.io/painel-senhas/`
- TV: `https://luucashl095-ui.github.io/painel-senhas/#painel`
- Relatório: `https://luucashl095-ui.github.io/painel-senhas/#relatorio`
- Configurar: `https://luucashl095-ui.github.io/painel-senhas/#configurar`

## Como funciona

Este repositório (público) guarda só o código. A fila, as configurações e os vídeos ficam num **repositório privado de dados**, lido e gravado pelo próprio painel pela API do GitHub. Nunca coloque os dados num repositório público: eles têm nomes de pessoas. O painel recusa repositórios públicos.

No repositório de dados o painel cria:

- `dias/` — um arquivo por dia com as senhas (apagados após 60 dias)
- `midia/` — vídeos (MP4/WebM) e cartazes (PNG/JPG/WebP), até 25 MB cada
- `config.json` — nome da unidade, frase, voz e programas de saúde

## Configuração (uma vez)

1. Crie um repositório **privado** (ex.: `painel-senhas-dados`) marcando **Add a README file**.
2. Crie um token em GitHub → Settings → Developer settings → Personal access tokens → **Fine-grained tokens**:
   - Repository access: **Only select repositories** → só o repositório de dados.
   - Permissions → Repository permissions → **Contents: Read and write**.
3. Em cada aparelho (recepção, TV), abra o link, informe `usuario/painel-senhas-dados` e o token e clique em **Conectar**. Fica salvo no navegador.

A TV: abra o link `#painel` e toque em **Ativar painel** para liberar som e voz.
