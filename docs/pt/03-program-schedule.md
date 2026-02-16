---
layout: default
title: Grade de programação
---

# Grade de programação

A grade de programação permite que o player mostre **o que está no ar agora** e **o que vem a seguir**. Você define programas (nome, logo e descrições opcionais) e os atribui a faixas horárias para cada dia da semana. O player usa o fuso horário do WordPress e atualiza no início de cada minuto.

**Anterior:** [Configuração](02-configuration.html) · **Próximo:** [Personalização visual](04-visual-customization.html)

## O que o player mostra

- **Programa atual** — Abaixo do título da estação: nome do programa e faixa horária (ex.: “Programa da manhã – 08:00–10:00”).
- **Próximo programa** — Quando o próximo programa começa em 10 minutos ou menos, aparece um anúncio (ex.: “Em breve: Notícias do meio-dia em 5 min”).
- **Modal da grade** — Visão semanal com o dia atual primeiro e rolagem automática para o programa ativo; “Voltar para hoje” e botão de fechar.
- **Modal de todos os programas** — Lista alfabética de todos os programas com suas faixas semanais. Descrições e descrições estendidas são exibidas nesses modais.

Todos os horários são baseados no **fuso horário do WordPress** (Configurações → Geral). O “horário atual” no player é o horário da estação, não necessariamente o horário local do visitante. Quando o fuso horário da estação difere do do visitante, o relógio de fuso horário no player (quando visível) mostra o horário da estação e a diferença.

## No admin: Programas

Expanda **Show Program Schedule** para a estação. Na seção **Programs**:

1. Clique em **Add Program** para cada programa que quiser definir.
2. Para cada programa:
   - **Program name** (obrigatório se usado na grade) — Nome curto exibido no player e na grade.
   - **Add Program Image** / **Change Image** — Logo opcional; tamanho recomendado 256×256 px. Usado no player e na grade/modais.
   - **Description** e **extended description** opcionais (se você usar a área “Show more fields”) — Exibidos na grade e no modal de todos os programas.
3. Use **Remove Program** para excluir um programa. Se ele estiver em alguma faixa, remova ou altere essas faixas primeiro.

Validação: se um programa é usado na grade, ele deve ter nome. O formulário mostrará um erro e rolará até o primeiro problema se você tentar salvar com nome faltando ou faixas inválidas.

*[Figura: Painel da grade no admin com Programs e Schedule por dia. Adicionar captura como `../../assets/images/admin-schedule-panel.jpg` quando disponível.]*

## No admin: Schedule

Na seção **Schedule** você atribui programas a faixas horárias para cada dia (segunda a domingo).

1. Para o dia desejado, clique em **Add Time Slot**.
2. Em cada faixa:
   - **Select Program** — Escolha um dos programas definidos.
   - **Start** e **End** — Formato 24 horas (HH:MM). Por exemplo, 14:00 são 2 da tarde.
3. Você pode adicionar várias faixas por dia. Use **Remove Time Slot** para remover uma faixa.

### Regras

- **Sem sobreposição** no mesmo dia. Se duas faixas se sobrepuserem, ambas mostrarão um erro (ex.: “This time slot overlaps with: Programa da manhã”). Corrija os horários para que não se sobreponham.
- **Programas que cruzam a meia-noite** são permitidos. Por exemplo, uma faixa de 23:00 a 01:00 é válida; o plugin a trata como cruzando a meia-noite.
- Os horários são armazenados e exibidos em formato 24 horas. O player usa o fuso horário do WordPress para decidir qual programa é “agora” e qual é “próximo”.

A descrição abaixo da grade no admin resume: atribua programas a faixas por dia; o player mostra o programa atual e o próximo e pode anunciar o próximo quando ele começar em 10 minutos ou menos; a exibição usa o fuso horário do site e atualiza no início de cada minuto.

*[Figura: Player com programa atual e anúncio “Em breve” opcional. Adicionar captura como `../../assets/images/player-now-playing.jpg` quando disponível.]*

*[Figura: Modal da grade ou de todos os programas no player. Adicionar captura como `../../assets/images/program-modal.jpg` quando disponível.]*

## Fuso horário

O “agora” usado para o programa atual e o anúncio do “próximo” é o **horário do site WordPress** (Configurações → Geral → Fuso horário). Se sua estação transmite em outro fuso horário, defina o fuso horário do WordPress para o da estação. O relógio de fuso horário no player (quando exibido) mostra o horário da estação e a diferença em relação ao visitante.

**Anterior:** [Configuração](02-configuration.html) · **Próximo:** [Personalização visual](04-visual-customization.html)
