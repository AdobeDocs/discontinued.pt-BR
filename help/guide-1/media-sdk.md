---
title: Perguntas frequentes sobre o fim da vida útil do Adobe Media SDK (versões 1.x e 2.x)
description: Obtenha respostas para perguntas frequentes sobre o fim da vida útil do Adobe Media SDK versões 1.x e 2.x (anteriormente Biblioteca do Video Heartbeat).
source-git-commit: d014c200dd926ccf0116faa50c4bffb1d234e926
workflow-type: tm+mt
source-wordcount: '1046'
ht-degree: 1%

---


# Perguntas frequentes sobre o fim da vida útil do Adobe Media SDK (versões 1.x e 2.x)

O Adobe Media SDK **2.x chegou ao fim do suporte em 31 de agosto de 2021**. A Biblioteca do Video Heartbeat (VHL) **1.x está obsoleta** e não tem suporte há vários anos.

## O que está acontecendo?

A Biblioteca Video Heartbeat (VHL) original, mais tarde renomeada como Media SDK, forneceu rastreamento do lado do cliente para análise de áudio e vídeo. A Adobe fez a transição dos recursos de rastreamento para implementações mais recentes e capazes:

* **Media SDK 3.x (somente Analytics):** Com suporte no momento. Rastreia mídia usando a API Media Collection. Recomendado para usuários 2.x existentes que ainda não podem migrar para o Edge Network.
* **Mídia de Streaming para o Edge Network (recomendado):** A implementação recomendada no momento. Usa a API do Adobe Experience Platform Web SDK, Mobile SDK ou Media Edge para enviar dados de mídia por meio da Edge Network, permitindo o uso na Adobe Analytics, Customer Journey Analytics, Real-Time CDP e Adobe Journey Optimizer.

## O que está incluído no fim da vida útil e o que não está?

**Fim da vida útil (sem suporte):**

* Video Heartbeat Library (VHL) 1.x — todas as plataformas (Android, iOS, JavaScript, Apple TV, Chromecast, Roku, TVML)
* Media SDK 2.x — Android, iOS, JavaScript

**Não é fim da vida útil (ainda com suporte):**

* Media SDK 3.x — JavaScript, Chromecast, Roku (somente Analytics)
* Mídia de transmissão para Edge Network — todas as plataformas compatíveis

## Por que as versões 1.x e 2.x foram descontinuadas?

A partir da versão 3.0, o Media SDK foi reprojetado para usar a API Media Collection diretamente, eliminando a necessidade de um padrão delegado e simplificando a criação do rastreador. Os SDKs 1.x e 2.x mais antigos dependiam de uma arquitetura de servidor de heartbeat que, desde então, foi substituída.

A Adobe também introduziu a implementação do Edge Network para fornecer um único pipeline de coleta de dados capaz de alimentar vários aplicativos downstream do Adobe, que os SDKs de heartbeat herdados não podiam suportar.

## Onde posso encontrar a documentação arquivada?

A documentação herdada foi arquivada no GitHub e está disponível para referência:

| Versão | Status | Documentação arquivada |
|---|---|---|
| 1.x (Biblioteca do Video Heartbeat) | Obsoleto | [`video-heartbeat` repositório do GitHub](https://github.com/Adobe-Marketing-Cloud/video-heartbeat/tree/master/docs) |
| 2.x (Media SDK) | Fim do suporte em 31 de agosto de 2021 | [`media-sdks` repositório do GitHub](https://github.com/Adobe-Marketing-Cloud/media-sdks/blob/master/docs/2.x/README.md) |

## Quais são minhas opções de transição?

**Opção 1: migrar para o Media SDK 3.x (somente Analytics)**

Se você estiver no 2.x e usar o Adobe Analytics exclusivamente, migrar para o 3.x é o caminho mais simples. Consulte o [guia de migração de 2.x para 3.x](https://experienceleague.adobe.com/docs/media-analytics/using/implementation/media-sdk/setup/migrate-js-2x-to-3x.html) para obter uma comparação de API completa e exemplos de código.

**Opção 2: migrar para mídia de streaming do Edge Network (recomendado)**

Para novas implementações ou quando quiser usar dados em vários aplicativos da Adobe, use o Adobe Experience Platform Edge Network:

* [Media Edge Web SDK](https://experienceleague.adobe.com/docs/media-analytics/using/implementation/edge/edge-web-sdk.html)
* [Media Edge Mobile SDK](https://experienceleague.adobe.com/docs/media-analytics/using/implementation/edge/edge-mobile-sdk.html)
* [API do Media Edge](https://experienceleague.adobe.com/docs/media-analytics/using/implementation/edge/implementation-edge-api.html)

## Perguntas frequentes

+++**O suporte para SDKs Roku e Chromecast será afetado?**

Não. Os SDKs Roku e Chromecast permanecem disponíveis e são compatíveis como parte do Media SDK 3.x (somente Analytics). Esse fim da vida útil abrange apenas as versões 1.x e 2.x.

+++

+++**As implementações do Media Analytics JavaScript SDK serão afetadas?**

Não. Os clientes que usam o JavaScript SDK para Media Analytics podem continuar a usar o SDK independente ou a extensão de tag.

+++

+++**Ainda estou no Media SDK 2.x. O que devo fazer?**

A Adobe recomenda migrar para a implementação do Edge Network para todos os novos projetos. Se você precisar de uma etapa intermediária, [Migre do JavaScript SDK 2.x para o 3.x](https://experienceleague.adobe.com/docs/media-analytics/using/implementation/media-sdk/setup/migrate-js-2x-to-3x.html) e, em seguida, planeje sua mudança para o Edge Network.

+++

+++**Qual é o nível de esforço (LOE) para migrar para uma implementação com suporte?**

O esforço de migração depende da implementação de cada cliente e varia. Depois de consultar a documentação de migração, entre em contato com a consultoria ou o atendimento ao cliente para obter suporte adicional:

* [Implementar mídia de transmissão usando o SDK Edge móvel — Android e iOS](https://experienceleague.adobe.com/docs/media-analytics/using/implementation/edge/edge-mobile-sdk.html)
* [Migração do JavaScript SDK 2.x para 3.x](https://experienceleague.adobe.com/docs/media-analytics/using/implementation/media-sdk/setup/migrate-js-2x-to-3x.html)

+++

+++**Preciso usar as Tags do Adobe Experience Platform como um sistema de gerenciamento de tags?**

Para implementações de aplicativos móveis, as Tags do Experience Platform não são usadas como um sistema de gerenciamento de tags da mesma forma que para a Web. A interface de Tags é necessária para configurar extensões do SDK. É semelhante à forma como a interface do usuário do Adobe Mobile Services foi usada para configurar o Mobile v4 SDK. As tags fornecem instruções personalizadas de instalação com base na extensão escolhida.

+++

+++**Este fim de suporte afeta o SDK para tvOS?**

Sim. Para tvOS (versão 10+), a implementação recomendada é migrar para Mídia de streaming para Edge Network usando o Adobe Experience Platform Mobile SDK. Consulte [Implementar mídia de streaming usando o SDK Edge móvel](https://experienceleague.adobe.com/docs/media-analytics/using/implementation/edge/edge-mobile-sdk.html) para obter mais detalhes.

+++

+++**Este fim de suporte afeta o SDK para Fire TV e Android TV?**

Sim. Para o Fire TV e Android TV, a implementação recomendada é migrar para Mídia de streaming para Edge Network usando o Adobe Experience Platform Mobile SDK. Consulte [Implementar mídia de streaming usando o SDK Edge móvel](https://experienceleague.adobe.com/docs/media-analytics/using/implementation/edge/edge-mobile-sdk.html) para obter mais detalhes.

+++

+++**Onde posso encontrar as informações do fim da vida útil do Mobile v4 SDK?**

Consulte as [Perguntas frequentes sobre o fim da vida útil do Mobile Services](mobile-services.md). A plataforma do Mobile Services e os SDKs v4 móveis foram encerrados em 31 de dezembro de 2022.

+++

+++**Onde posso ir se tiver dúvidas?**

Entre em contato com a equipe de conta da Adobe ou com o Atendimento ao cliente da Adobe para obter assistência na migração.

+++

>[!MORELIKETHIS]
>
>* [Visão geral da implementação de mídia de streaming](https://experienceleague.adobe.com/docs/media-analytics/using/implementation/overview.html)
>* [Streaming de Mídia para Edge Network](https://experienceleague.adobe.com/docs/media-analytics/using/implementation/edge/implementation-edge.html)
>* [Media SDK 3.x — Configuração do JavaScript](https://experienceleague.adobe.com/docs/media-analytics/using/implementation/media-sdk/setup/web-implementation.html)
