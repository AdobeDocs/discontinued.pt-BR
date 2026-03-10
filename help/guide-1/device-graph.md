---
keywords: Gráfico de dispositivos;fim da vida útil
title: Gráfico de dispositivos
description: Saiba mais sobre os planos para o fim da vida útil do gráfico de dispositivos.
source-git-commit: 6d27883347049957d35070dd5c5bf5b223144470
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 4%

---

# Fim da vida útil do gráfico de dispositivos

>[!WARNING]
>
>O Gráfico de dispositivos na Análise entre dispositivos não está mais disponível a partir de **31 de dezembro de 2025**. Alterne qualquer conjunto de relatórios virtuais habilitado para o gráfico de dispositivos atual para o [método baseado em campo](https://experienceleague.adobe.com/pt-br/docs/analytics/components/cda/field-based-stitching).

O Cross-Device Analytics usou o Gráfico privado para compilar dados. O Gráfico privado é um repositório de IDs de dispositivos com hash específicas da sua organização. O CDA se comunica regularmente com o gráfico do dispositivo para vincular dispositivos.

## Pré-requisitos específicos do gráfico de dispositivos

Se você pretendia implementar o Cross-Device Analytics usando o método de gráfico de dispositivo, as seguintes etapas eram obrigatórias.

>[!WARNING]
>
>O não cumprimento de todos os pré-requisitos pode gerar a incapacidade de ativar o Cross-Device Analytics ou resultados inadequados ao compilar os dados.

* Sua organização deve usar o [Gráfico privado do Serviço de Identidade da Adobe Experience Platform](https://business.adobe.com/br/products/experience-platform/identity-service.html). Consulte também a [Página inicial](https://experienceleague.adobe.com/docs/experience-platform/identity/home.html?lang=pt-BR) no guia do usuário do Serviço de identidade.
* Sua implementação deve usar a versão mais recente do Serviço da Experience Cloud ID (ECID). Consulte a [Página inicial](https://experienceleague.adobe.com/docs/id-service/using/home.html?lang=pt-BR) no guia do usuário do Serviço de ID. Provavelmente, a maioria das implementações que usam [Tags](https://experienceleague.adobe.com/docs/experience-platform/tags/home.html?lang=pt-BR) na Adobe Experience Platform já tem o Serviço de ID implantado.
* Sua implementação deve chamar a função `setCustomerIDs` (ou SDK equivalente) sempre que um indivíduo puder ser identificado, como quando um usuário se conecta ou abre um email. Esse requisito se aplica a todas as plataformas, incluindo aplicativos móveis, se usados. Consulte [`setCustomerIDs`](https://experienceleague.adobe.com/docs/id-service/using/id-service-api/methods/setcustomerids.html?lang=pt-BR) no guia do usuário do Serviço de ID.

## Limitações específicas do gráfico de dispositivos

* As IDs herdadas do Analytics não são compatíveis. Somente os visitantes com Experience Cloud IDs são compilados.
* Se sua organização usar um Gráfico privado, novos dispositivos levarão até 24 horas para serem compilados.
* Os gráficos de dispositivos de terceiros não são compatíveis.
