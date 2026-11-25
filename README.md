# Painel de Senhas

Painel de senhas da sala de vacina: recepção, TV com chamada por voz, relatório de tempo de espera e configurações.

## Links

- Recepção: `https://luucashl095-ui.github.io/painel-senhas/`
- TV: `https://luucashl095-ui.github.io/painel-senhas/#painel`
- Relatório: `https://luucashl095-ui.github.io/painel-senhas/#relatorio`
- Configurar: `https://luucashl095-ui.github.io/painel-senhas/#configurar`

## Como funciona

Este repositório guarda só o código. A fila, as configurações e os vídeos ficam numa **pasta de rede compartilhada** que a recepção e a TV escolhem ao abrir o painel. Nenhum nome de paciente vai para o GitHub.

Dentro da pasta o painel cria:

- `dias/` — um arquivo por dia com as senhas (apagados após 60 dias)
- `midia/` — vídeos (MP4/WebM) e cartazes (PNG/JPG/WebP) exibidos na TV, em ordem de nome
- `config.json` — nome da unidade, frase, voz e programas de saúde

## Uso

1. Abra o link no **Microsoft Edge** ou no **Google Chrome**.
2. Recepção: clique em **Escolher pasta** e selecione a pasta de rede.
3. TV: abra o link `#painel`, clique em **Ativar painel** e escolha a mesma pasta.
4. A cada abertura do navegador, confirme o acesso clicando em **Reconectar** e depois em "Permitir".
