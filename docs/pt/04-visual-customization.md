# Personalização visual

Você pode adaptar a aparência do player com temas de cor, visualizadores de áudio e imagens. Todas as opções são por estação e são definidas em **Configurações → Radio Player Page Settings**.

**Anterior:** [Grade de programação](03-program-schedule.md) · **Próximo:** [Múltiplas estações](05-multiple-stations.md)

## Tema de cor

Há oito temas de cor. Todos usam fundo escuro; apenas a cor de destaque muda.

| Tema    | Descrição              |
|---------|------------------------|
| Neutral | Destaque cinza (padrão) |
| Blue    | Destaque azul          |
| Green   | Destaque verde         |
| Red     | Destaque vermelho      |
| Orange  | Destaque laranja       |
| Yellow  | Destaque amarelo       |
| Purple  | Destaque roxo          |
| Pink    | Destaque rosa          |

Selecione o tema no menu **Theme Color** de cada estação. Padrão: **Neutral**.

## Visualizadores

Há quatro visualizações de áudio em tempo real. Elas são carregadas apenas quando necessário (lazy-loaded) e rodam apenas enquanto há áudio.

| Visualizador        | Tipo                | Descrição                     |
|--------------------|---------------------|-------------------------------|
| Oscilloscope       | Forma de onda (padrão) | Forma de onda clássica no domínio do tempo |
| Bars Spectrum      | Frequência          | Barras de frequência         |
| Amplitude Waterfall| Amplitude           | Cascata de amplitude         |
| Spectral Particles | Frequência          | Vista em partículas          |

Selecione o **Visualizer** nas configurações da estação. Padrão: **Oscilloscope**. A visualização requer suporte do navegador à Web Audio API (todos os navegadores modernos de desktop e móvel a suportam).

## Imagens

### Logo da estação

O **Logo Image** da estação é exibido no player e nos controles de mídia do sistema (tela de bloqueio, notificação, controles de desktop). Tamanho recomendado: **512×512 pixels** ou maior. Defina-o no bloco da estação em **Logo Image (Optional)**.

### Imagem de fundo

A **Background Image** é exibida em tamanho completo atrás do player. Não há tamanho fixo; use uma imagem que fique boa em várias resoluções. Defina-a em **Background Image (Optional)**.

### Logo do programa

Quando você define programas na [Grade de programação](03-program-schedule.md), pode anexar uma imagem opcional a cada programa. Tamanho recomendado: **256×256 pixels**. Os logos dos programas aparecem no modal da grade e no modal de todos os programas.

## Notas

- **Design responsivo** — O player se adapta a desktop, tablet e celular.
- **iOS** — O controle de volume fica oculto no iOS porque o sistema controla o volume da reprodução. Streams HLS usam o player nativo do Safari quando disponível.
- **Desempenho** — Visualizadores e bibliotecas de streaming (ex.: para HLS/DASH) são carregados sob demanda para manter a carga inicial leve.

**Anterior:** [Grade de programação](03-program-schedule.md) · **Próximo:** [Múltiplas estações](05-multiple-stations.md)
