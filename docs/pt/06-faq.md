# Perguntas frequentes

**Anterior:** [Múltiplas estações](05-multiple-stations.md) · **Voltar a:** [Índice da documentação](index.md)

## Preciso configurar algo na página do WordPress?

Não. Depois de atribuir uma página a uma estação em **Configurações → Radio Player Page Settings**, não é necessário mais nada na página. O plugin intercepta as requisições a essa página e serve uma página HTML independente com o player. O conteúdo, o modelo e as configurações da página não são usados para essa URL.

## Onde posso obter suporte ou reportar problemas?

Use o [fórum de suporte do WordPress.org para Radio Player Page](https://wordpress.org/support/plugin/radio-player-page/) para dúvidas, pedidos de recursos e reporte de bugs.

## Posso usar em rádios comerciais?

Sim. O plugin é gratuito e de código aberto (GPLv2 ou posterior) e pode ser usado em estações comerciais e não comerciais.

## Onde está o código-fonte?

O código-fonte está no [GitHub](https://github.com/sjimhdez/radio-player-page).

## Quais formatos de stream são suportados?

O plugin suporta:

- **Icecast** e **Shoutcast** — Protocolos tradicionais de streaming de rádio.
- **HLS** (`.m3u8`) — Streaming adaptativo; o Safari no iOS usa suporte HLS nativo.
- **DASH** (`.mpd`) — Streaming adaptativo moderno.
- **MP3** — Streaming de áudio padrão.

O plugin detecta o tipo de stream automaticamente e carrega o player adequado (incluindo bibliotecas opcionais para HLS/DASH quando necessário).

## Em quais idiomas o player está disponível?

A interface do player está disponível em: inglês (EUA), espanhol, espanhol (México), russo, holandês, romeno, sueco, galego e dinamarquês. O idioma é escolhido com base no navegador (atributo `lang` do HTML, depois preferência armazenada, depois idioma do navegador), com fallback para inglês.

## Como funciona o temporizador de sono (sleep timer)?

Você pode fazer o player parar a reprodução após **30**, **60** ou **120** minutos. Uma contagem regressiva é exibida enquanto o temporizador está ativo. Se você pausar a reprodução manualmente, o sleep timer é cancelado. O temporizador serve apenas para parar a reprodução automaticamente; não afeta o stream nem a estação.

## O que acontece quando desinstalo o plugin?

Quando o plugin é **desinstalado** (removido do site, não apenas desativado), o script `uninstall.php` é executado e remove a opção `radplapag_settings` do banco de dados. Em multisite, ela é removida de cada site. A opção **não** é removida quando você apenas desativa o plugin.

## Por que o stream não carrega?

Se o player não iniciar ou o stream não tocar:

1. **Verifique a URL** — Em **Configurações → Radio Player Page Settings**, confira se a **Streaming URL** está correta e acessível (tente abri-la em outra aba ou em outro player).
2. **CORS** — Se o stream está em outro domínio, o servidor deve permitir requisições do seu site (cabeçalhos CORS). Muitos servidores de streaming permitem por padrão; se não, pode ser necessário configurar o servidor do stream.
3. **Console do navegador** — Abra as ferramentas de desenvolvedor (F12) e verifique a aba Console em busca de erros. Erros de rede ou requisições bloqueadas podem indicar URL incorreta ou problema de CORS.
4. **Formato** — O plugin suporta Icecast, Shoutcast, HLS, DASH e MP3. Streams incomuns ou protegidos podem não funcionar.

Se o problema continuar, descreva sua configuração (tipo de stream, formato da URL e mensagens de erro) no [fórum de suporte](https://wordpress.org/support/plugin/radio-player-page/).

**Anterior:** [Múltiplas estações](05-multiple-stations.md) · **Voltar a:** [Índice da documentação](index.md)
