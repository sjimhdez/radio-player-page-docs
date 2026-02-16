---
layout: default
title: Instalação
---

# Instalação

Esta página descreve os requisitos e os passos para instalar e ativar o Radio Player Page.

## Requisitos

- **WordPress** 5.0 ou superior  
- **PHP** 5.6 ou superior  
- Uma **URL de streaming válida** (Icecast, Shoutcast, HLS, DASH ou MP3)

Para melhor experiência, use um navegador moderno. Os visualizadores de áudio usam a Web Audio API, suportada nas versões atuais do Chrome, Firefox, Edge e Safari (incluindo Safari no iOS 10+).

## Passos de instalação

1. **Envie o plugin** para a pasta `wp-content/plugins/`, ou instale-o pela tela **Plugins** (Adicionar novo → Enviar plugin ou pesquise por “Radio Player Page”).

2. **Ative o plugin** na tela **Plugins** do WordPress.

3. Vá em **Configurações → Radio Player Page Settings**.

4. Para pelo menos uma estação:
   - Informe a **Streaming URL** (a URL completa do seu stream).
   - Selecione a **Player Page** (a página do WordPress em que o player deve aparecer).
   - Clique em **Save Changes** (Guardar alterações).

5. **Abra a página atribuída** no navegador. O player carrega automaticamente; não é necessário adicionar conteúdo nem shortcode à página.

## Nota importante

Não é necessário configurar nada na própria página do WordPress. O plugin usa o hook `template_redirect` do WordPress: quando um visitante solicita uma página atribuída a uma estação, o plugin serve uma página HTML independente com o player e impede o carregamento do tema. O conteúdo e o modelo da página não são usados para essa URL.

**Próximo:** [Configuração](02-configuration.html) — Definir nome da estação, tema, visualizador, imagens e grade de programação opcional.
