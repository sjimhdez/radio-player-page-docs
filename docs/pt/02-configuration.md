# Configuração

Todas as opções das estações são gerenciadas em **Configurações → Radio Player Page Settings**. Cada estação tem seu próprio bloco de opções; esta página descreve cada campo.

**Anterior:** [Instalação](01-installation.md) · **Próximo:** [Grade de programação](03-program-schedule.md)

## Onde configurar

Abra **Configurações → Radio Player Page Settings** no painel do WordPress. Você verá um ou mais blocos de estação. Para cada estação que usar, preencha pelo menos **Player Page** e **Streaming URL** e clique em **Save Changes** no final da página.

*[Figura: Página de configurações com as opções gerais da estação. Adicionar captura como `../../assets/images/settings-general.jpg` quando disponível.]*

## Campos por estação

### Player Page (obrigatório)

A página do WordPress em que o player aparecerá. Selecione-a no menu suspenso. Quando alguém acessar a URL dessa página, o plugin serve o player independente em vez do tema. Cada estação deve ter uma página diferente.

### Streaming URL (obrigatório)

A URL completa do seu stream de áudio (ex.: `https://exemplo.com:8000/stream` ou uma URL HLS/DASH). Formatos suportados:

- Icecast e Shoutcast  
- HLS (`.m3u8`)  
- DASH (`.mpd`)  
- Streams MP3  

O plugin valida a URL ao salvar e detecta o tipo de stream automaticamente para a reprodução.

### Station Name (opcional)

Um título para a estação (ex.: “Minha rádio”). Máximo de 64 caracteres. Se deixado em branco, é usado o título do site em **Configurações → Geral** no player e nos controles de mídia do sistema.

### Theme Color

Menu suspenso com oito opções: **Neutral**, **Blue**, **Green**, **Red**, **Orange**, **Yellow**, **Purple**, **Pink**. Todos os temas usam fundo escuro. Padrão: **Neutral**.

### Visualizer

Escolha a visualização de áudio em tempo real: **Oscilloscope** (padrão, forma de onda), **Bars Spectrum**, **Amplitude Waterfall** ou **Spectral Particles**. Os visualizadores são carregados apenas quando necessário e rodam apenas enquanto há áudio.

### Logo Image (opcional)

O logo da estação, exibido no player e na tela de bloqueio e nos controles de mídia do sistema. Tamanho recomendado: 512×512 pixels ou maior. Use **Select Image** para escolher na biblioteca de mídia e **Remove** para remover.

### Background Image (opcional)

Uma imagem em tamanho completo exibida atrás do player. Use **Select Image** para definir e **Remove** para remover.

### Program Schedule (opcional)

Seção recolhível para definir **programas** (nome, logo opcional, descrições opcionais) e a **grade semanal** de faixas horárias por dia. O player então mostra o programa atual e o próximo e pode anunciar o próximo quando ele começar em 10 minutos ou menos. Para todos os detalhes, veja [Grade de programação](03-program-schedule.md).

## Salvar alterações

Sempre clique em **Save Changes** no final do formulário após editar. Até salvar, as alterações não são armazenadas e o player não as refletirá.

**Anterior:** [Instalação](01-installation.md) · **Próximo:** [Grade de programação](03-program-schedule.md)
