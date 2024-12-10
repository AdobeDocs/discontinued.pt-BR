---
keywords: adobe experience cloud;Adobe Experience Cloud;device co-op;Device Co-op;fim da vida útil
title: Perguntas frequentes sobre o fim da vida útil do [!DNL Device Co-op]
description: Saiba mais sobre os planos de fim de vida útil do Device Co-op.
exl-id: 015ba95c-0c8d-415e-969c-b8670494de98
source-git-commit: f259a6d2bac47e9cf3a829017642119357208c7c
workflow-type: tm+mt
source-wordcount: '1053'
ht-degree: 99%

---

# Perguntas frequentes sobre o fim da vida útil do [!DNL Device Co-op]

Este documento fornece respostas para perguntas frequentes sobre o plano de fim da vida útil (EOL) do [!DNL Adobe Experience Cloud Device Co-op]. Quando esse plano entrar em vigor, a Adobe fornecerá um aviso avançado nas [Notas de versão da Experience Cloud](https://experienceleague.adobe.com/docs/release-notes/experience-cloud/current.html?lang=pt-BR) e na [Atualização prioritária do produto](https://www.adobe.com/br/subscription/priority-product-update.html).

O [!DNL Device Co-op] foi um programa que permitia que os participantes trabalhassem em conjunto para identificar melhor os consumidores em todos os pontos de contato digitais, garantindo ao mesmo tempo o mais alto nível de privacidade e transparência.

## Perguntas frequentes

Veja a seguir uma lista de respostas para perguntas frequentes sobre o plano de EOL do [!DNL Device Co-op].

## Por que o [!DNL Device Co-op] está sendo descontinuado?

As próximas alterações no ambiente AdTech devem resultar no [!DNL Device Co-op] se tornando uma solução obsoleta nos próximos anos. O [!DNL Device Co-op] é composto principalmente de cookies de terceiros e o comunicado do [!DNL Google's], de que eles estarão bloqueando cookies de terceiros no [!DNL Google Chrome] até 2022, diminuirá a eficácia do [!DNL Device Co-op]. O [!DNL Chrome] tem aproximadamente 65% da quota de mercado do navegador e outros principais navegadores já implementaram o bloqueio de cookies de terceiros. Uma vez que o [!DNL Chrome] bloqueia cookies de terceiros, a maioria dos cookies de terceiros será bloqueada e o [!DNL Device Co-op] se tornará obsoleto.

## Por que a Adobe está encerrando as inscrições do [!DNL Device Co-op] agora?

As inscrições estão sendo encerradas para evitar riscos de não atender às expectativas dos clientes devido às próximas alterações do setor em cookies de terceiros. O [!DNL Device Co-op] demora alguns meses para ser preparado e mais alguns meses para extrair valor do serviço. A partir de agora, quaisquer novas inscrições poderiam resultar em marcas que não experienciariam o valor total do [!DNL Device Co-op].

## Em julho de 2022, o Google anunciou o atraso da desativação de cookies de terceiros no Chrome para 2024. Isso afetará os planos de EOL do [!DNL Device Co-op]?

Não, os planos de EOL do [!DNL Device Co-op] da Adobe continuarão a ser os mesmos e não serão prorrogados.

## Os novos clientes podem se inscrever?

A partir de 11 de junho de 2021, a Adobe deixará de aceitar novas inscrições no [!DNL Device Co-op].

## Os contratos existentes estão sendo renovados?

A partir de 11 de junho de 2021, a Adobe não renovará mais os contratos do [!DNL Device Co-op]. Se desejar continuar usando os serviços do [!DNL Device Co-op], você pode continuar a fazê-lo sob os termos de licença atuais até o fim do programa.

## Qual é a data final exata do programa do [!DNL Device Co-op]?

O programa do [!DNL Device Co-op] terminará em 2022. A hora e a data específicas dependem de quando o [!DNL Google] começará a bloquear cookies de terceiros. O trabalho de desativação deverá ter início em setembro de 2022.

## Quais aplicativos serão afetados pelo fim da vida útil do Device Co-op?

Os seguintes aplicativos serão afetados pelos procedimentos de fim de vida útil do [!DNL Device Co-op]:

- [[!DNL Adobe Analytics]](https://experienceleague.adobe.com/docs/analytics.html?lang=pt-BR)
- [[!DNL Adobe Audience Manager]](https://experienceleague.adobe.com/docs/audience-manager/user-guide/overview/aam-overview.html?lang=pt-BR)
- [[!DNL Adobe Advertising]](https://experienceleague.adobe.com/docs/advertising.html?lang=en)
- [[!DNL Adobe Target]](https://experienceleague.adobe.com/docs/target/using/introduction/intro.html?lang=pt-BR)

## Quais opções tenho como alternativas para o [!DNL Device Co-op]?

### [!DNL Analytics]

Você pode usar a [Análise entre dispositivos (CDA)](https://experienceleague.adobe.com/docs/analytics/components/cda/overview.html?lang=pt-BR) do [!DNL Analytics], pois ela é compatível com o [Gráfico privado](https://experienceleague.adobe.com/docs/analytics/components/cda/device-graph.html?lang=pt-BR) e a [Compilação baseada em campo](https://experienceleague.adobe.com/docs/analytics/components/cda/field-based-stitching.html?lang=pt-BR) do serviço de identidade da Adobe Experience Platform.

### [!DNL Audience Manager]

O [!DNL Audience Manager] mantém integrações com parceiros de gráficos de dispositivos de terceiros, incluindo [!DNL LiveRamp] e [!DNL Tapad], embora seja necessário estabelecer relações comerciais diretamente com os parceiros de gráfico, para aproveitar o [!DNL Audience Manager]. Espera-se que todos os clientes atualizem quaisquer políticas de mesclagem de perfis cooperativos para utilizar outras opções além do [!DNL Device Co-op.]

### [!DNL Real-time Customer Data Platform]

Não há planos para modificar o [!DNL Audience Manager Data Management Platform] (DMP) atual. No entanto, a desativação de cookies de terceiros provavelmente criará desafios de escala para a maioria dos usuários do DMP. Para ajudar os clientes a desenvolver suas práticas de gerenciamento de dados, a Adobe está incentivando a redução das dependências de identificadores que enfrentarão restrições no próximo ano. As equipes de marketing devem criar estratégias de dados primários com foco em identificadores duráveis que incluam informações de identificação pessoal (PII), que podem ser resolvidas com [!DNL Real-time Customer Data Platform] (Real-time CDP).

O [!DNL Real-time CDP] reduz as dependências de cookies de terceiros e IDs de dispositivo, expandindo o conjunto de identificadores disponíveis para a criação de público-alvo para incluir PII. Fundamental para o [!DNL Real-time CDP] é o Perfil do cliente em tempo real, que reúne dados de atributos da pessoa com dados de comportamento em tempo real e permite que os profissionais de marketing criem segmentos avançados de público-alvo com controles patenteados de governança de dados. Como o [!DNL Audience Manager], o [!DNL Real-time CDP] capacita insights e casos de uso de personalização, mas também gera insights mais granulares no nível da pessoa e pode ativar públicos-alvo para uma grande variedade de destinos, abrangendo tecnologias de publicidade e tecnologias de marketing, incluindo mídia paga, redes sociais, email e sistemas de clientes.

O [!DNL Real-time CDP] também incluirá o acesso à [Correspondência de segmentos da Adobe Experience Platform (Beta)](https://experienceleague.adobe.com/docs/experience-platform/segmentation/ui/segment-match/overview.html?lang=pt-BR), que permite que as marcas expandam seus próprios conjuntos de dados primários por meio de parcerias e obtenham insights e personalização aprimorados.

### [!DNL Target]

No momento, não há alternativas disponíveis para o [!DNL Target] porque o [!DNL Target] fornece um recurso determinístico de identificação entre dispositivos conhecido como `mbox3rdPartyId`, que funciona de forma semelhante à ID do cliente da Adobe. Esse recurso permite aos clientes do [!DNL Target] mesclar perfis e participação de atividades em testes e personalização do [!DNL Target] sendo feitos em canais de entrada.

### Adobe Advertising Cloud

Os clientes da [!DNL Advertising Cloud] não poderão mais usar o [!DNL Device Co-op] para direcionamento e medição de público-alvo entre dispositivos. Com a [!DNL Advertising Cloud], você ainda poderá aproveitar a parceria do [!DNL Device Graph] da Adobe com o [!DNL LiveRamp] para continuar a desempenhar estas funções na medida da capacidade e escala do [!DNL LiveRamp's]. Você deve permitir que suas campanhas que estejam usando o [!DNL Device Co-op] sejam finalizadas, e depois alternar para o provedor de gráficos de dispositivos do [!DNL LiveRamp] ou não utilizar mais o direcionamento com base em pessoas.

## Quais recursos e implementações existentes podem ajudar minha preparação para um futuro sem cookies?

Sua implementação existente do Serviço de ID de visitante capacita o Analytics [CDA](https://experienceleague.adobe.com/docs/analytics/components/cda/overview.html?lang=pt-BR). Se a ID declarada existente for um email com hash, isso poderá ser usado para potencializar os seguintes recursos:

- [!DNL Audience Manager] [Destinos com base em pessoas](https://experienceleague.adobe.com/docs/audience-manager/user-guide/features/destinations/people-based/people-based-destinations-overview.html?lang=pt-BR).
- [Correspondência de segmentos da Experience Platform (Beta)](https://experienceleague.adobe.com/docs/experience-platform/segmentation/ui/segment-match/overview.html?lang=pt-BR).

## Posso manter meus dados do [!DNL Device Co-op]?

Para usuários do [!DNL Audience Manager] e da [!DNL Advertising Cloud], os dados do [!DNL Device Co-op] não estarão disponíveis para transferência para gráficos de terceiros. Os dados do [!DNL Device Co-op] serão migrados somente para usuários do [!DNL Analytics Ultimate] usando o CDA com o [!DNL Device Co-op] alternando para Configuração em campo. Todas as outras soluções não terão seus dados migrados.

## É obrigatório adotar outros recursos?

Embora a adoção de outros recursos da Adobe não seja obrigatória, você deve iniciar a implementação de outros recursos o mais rápido possível para permitir tempo e a coordenação apropriada antes da descontinuação do [!DNL Device Co-op].

## Quando terei de adotar soluções alternativas, se assim o decidir?

A adoção de outros recursos não é obrigatória. Só é recomendável se você quiser continuar a abordar casos de uso que foram abordados pelo [!DNL Device Co-op]. Se optar por adotar outros recursos, deverá fazê-lo até 2022 (data exata a ser comunicada) antes do programa [!DNL Device Co-op] terminar.

## Quanto tempo irá demorar a adoção?

Isso dependerá do recurso. Por exemplo, se um cliente do Analytics Ultimate que usa a análise entre dispositivos com o [!DNL Device Co-op] precisa migrar para o Gráfico de dispositivos privados em tempo real ou a Configuração em campo, a adoção levará algum tempo.

## E quanto à métrica [!UICONTROL Pessoas]?

Com a descontinuação do [!DNL Device Co-op], a métrica [!UICONTROL Pessoas] não será mais relevante. Em 8 de maio de 2023, removeremos a métrica [!UICONTROL Pessoas]. Quando isso ocorrer, redirecionaremos esses dados para a métrica [!UICONTROL Visitante único] no Analytics para impedir que projetos, segmentos e métricas calculadas sejam prejudicados.

