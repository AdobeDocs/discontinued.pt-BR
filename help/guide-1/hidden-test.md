---
title: Teste oculto
description: Este é um teste oculto
hide: true
hidefromtoc: true
landing-page-breadcrumb-title: Test AEM 6.5
landing-page-name: experience-manager-65
feature: Annotations
exl-id: e6e5ba1c-98a5-4d7d-9913-426df31bc7a3
source-git-commit: f6e3d17e221850a71617abfb9f5e75c0e26b362f
workflow-type: tm+mt
source-wordcount: '214'
ht-degree: 6%

---

# Teste oculto

26 de janeiro - Bob

Este é um teste oculto. Estou adicionando este `[` para garantir que funcione bem na renderização v2!

## Abrir em uma nova guia {#section_92882928}

`[See What's new](auditor.md) {target="_blank"}`

[Abrir na mesma guia](auditor.md)

[Nova guia com espaço e aspas](auditor.md) {target="_blank"}

[Nova guia com Âncora](auditor.md){target=&quot;_blank}

[Nova guia sem espaço com aspas](auditor.md){target="_blank"}

[Nova guia com espaço sem aspas](auditor.md) {target=_blank}

[Nova guia sem espaço sem aspas](auditor.md){target=_blank}

[Nova guia com deep link](commerce-channels.md#channel-manager-extension){target="_blank"}

[Ancorar nova guia com deep link](https://experienceleague.adobe.com/en/docs/analytics/analyze/home#key-analytics-resources){target="_blank"}

[Nova guia com link externo](https://www.adobe.com){target="_blank"}

[Novo link da raiz da guia](/help/guide-1/auditor.md){target="_blank"}


<table>
  <tr>
    <th>Com aspas</a></th>
    <th>Sem aspas</th>
  </tr>
  <tr>
    <td><a href="https://www.adobe.com" target="_blank">Nova guia Adobe</a></td>
    <td><a href="https://www.adobe.com" target="_blank">Nova guia Adobe</td>
  </tr>
  <tr>
    <td><a href="https://www.adobe.com">Adobe sem nova guia</a></td>
    <td><a href="https://www.adobe.com">Adobe sem nova guia</td>
  </tr>
</table>

## Comentar teste

18 de novembro de 2025

<!-- ## Comment with basic text

This is a new line.

Second new line. -->


Comente abaixo. Se essa é a última coisa que você vê neste artigo, é devido à sintaxe do comentário.

1. Clique em **[!UICONTROL Create]**.

<!-- ## Create an exclusion using Advanced Search

You can also create exclusions using [!UICONTROL Advanced Search] on the [Catalog Search](/help/main/c-recommendations/c-products/catalog-search.md#save-as) page ( [!UICONTROL Recommendations] > [!UICONTROL Catalog Search] > [!UICONTROL Advanced Search]). 

![Save as dialog](/help/main/c-recommendations/c-products/assets/save-as.png)

After creating a search using "id > contains," for example, you can then click [!UICONTROL Save As] > [!UICONTROL Exclusion].

>[!IMPORTANT]
>
>The [!UICONTROL Advanced Search] functionality is case-insensitive; however, products returned at the time of delivery are based on case-sensitive search. This mismatch might lead to confusion. Ensure that you consider case-sensitivity when you create exclusions based on results using the Advanced Search functionality. For example, if you perform a search for "Holiday," that initial search lists results containing "Holiday" and "holiday." If you then create an exclusion with the intent to exclude products containing "holiday," only products containing "holiday" are excluded. Products containing "Holiday" are not excluded. -->

Esta linha aparece após o comentário.

## Teste de vídeo

### Vídeo simples sem transcrição - deve mostrar a transcrição porque o arquivo metadata.md é exibido

>[!VIDEO](https://video.tv.adobe.com/v/332116?hidetitle=true)

### Com transcrição definida como verdadeira

>[!VIDEO](https://video.tv.adobe.com/v/332116?hidetitle=true){transcript=true}

### Com a transcrição definida como falsa - a transcrição do vídeo não deve ser exibida

>[!VIDEO](https://video.tv.adobe.com/v/332116?hidetitle=true){transcript=false}

## Links relativos

* [Visão geral](overview.md)
* [Pesquisar e promover](search-promote.md)
* [Social](social.md)

## Deep link explícito

[visão geral adicional (raiz)](/help/guide-1/overview.md#additional-products)

[visão geral adicional](overview.md#additional-products)

## Teste de focalização de texto {#this-is-a-heading-anchor}

Nenhum texto em foco

```
![alt text](assets/maui-flip.jpg)
```

![alt texto](assets/maui-flip.jpg)


Sim, passar o texto

```
![alt text](assets/maui-flip.jpg "Hover text")
```

![alt text](assets/maui-flip.jpg "Focalizar texto")

## Slide

Sintaxe:

```
>[!SLIDE](analyze-project)
https://experienceleague-stage.adobe.com/en/slides/analyze-project
```

Renderizado:

<!--
>[!SLIDE](analyze-project)
-->

Bob: remova o comentário do slide depois de testar o tópico loc.

