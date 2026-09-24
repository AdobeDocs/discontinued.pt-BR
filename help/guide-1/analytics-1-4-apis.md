---
title: Fim da vida útil da API do Adobe Analytics 1.4
description: A API do Adobe Analytics 1.4 e a autenticação WSSE foram encerradas em 31 de agosto de 2026. Saiba o que é afetado e como migrar para as APIs do Analytics 2.0.
source-git-commit: 4056ba0953e81a279d25b15449c7b41a4a5eb7f9
workflow-type: tm+mt
source-wordcount: '743'
ht-degree: 1%
---
# Fim da vida útil da API do Adobe Analytics 1.4

A partir de **31 de agosto de 2026**, a Adobe desativou a API do Adobe Analytics 1.4 e a autenticação WSSE. Todos os endpoints que usam essa versão da API não estão mais acessíveis e as integrações criadas nela pararam de funcionar.

As APIs do Adobe Analytics 1.4 forneceram uma grande variedade de ações, como relatórios, classificações, feeds de dados, segmentos, métricas calculadas, fontes de dados e configuração de conjunto de relatórios. Eles foram substituídos pelas [APIs do Adobe Analytics 2.0](https://developer.adobe.com/analytics-apis/docs/2.0), que permitem executar quase todas as ações disponíveis na interface do usuário do Adobe Analytics, incluindo a geração de relatórios e o gerenciamento de componentes, como segmentos e métricas calculadas. Se você tiver uma integração que ainda precisa ser atualizada, siga o guia para [Migrar para APIs do Adobe Analytics 2.0](https://developer.adobe.com/analytics-apis/docs/2.0/guides/migration).

## O que chegou ao fim da vida útil

Esse fim da vida útil afeta diretamente os recursos da API 1.4 a seguir. Migre cada fluxo de trabalho afetado para as [APIs do Adobe Analytics 2.0](https://developer.adobe.com/analytics-apis/docs/2.0):

* Relatórios (incluindo Data Warehouse, tempo real, definição de caminho e relatórios de resumo)
* Configuração e administração do conjunto de relatórios
* Classificações
* Segmentos
* Métricas calculadas
* Fontes de dados
* Feeds de dados
* Marcadores e métodos da empresa (endpoint)

Ele também desativa a **autenticação do Adobe Analytics WSSE** (consulte [autenticação do WSSE](#wsse-authentication) abaixo).

>[!IMPORTANT]
>
>Este fim da vida útil *não* afeta sua coleção de dados. As soluções de marcação, como Tags (antigo Adobe Launch), Web SDK e AppMeasurement, não são afetadas. A [API de Inserção de Dados](#data-insertion-api) também *não* está desativada. No entanto, se você usar as APIs de Classificações ou Fontes de dados 1.4 para aprimorar seus dados, será necessário migrar esses fluxos de trabalho para as APIs do Adobe Analytics 2.0.

## Autenticação WSSE

A autenticação WSSE é um protocolo de autenticação herdado compatível com as APIs do Analytics 1.4. Ele foi substituído pelas opções de autenticação com base em OAuth fornecidas no [Adobe Developer Console](https://developer.adobe.com/console/home). Os projetos que usaram a autenticação WSSE devem atualizar suas credenciais para aquelas provisionadas na Adobe Developer Console.

Para migrar, faça logon no [Adobe Developer Console](https://developer.adobe.com/console/home) e crie um projeto para a integração da API do Analytics 2.0. Selecione o método de autenticação **Usuário do OAuth** ou **Servidor para Servidor do OAuth**.

## API de inserção de dados

A API de Inserção de Dados **não** faz parte deste fim de vida. Sua documentação foi movida para o site [APIs de coleta de dados do Adobe Analytics](https://developer.adobe.com/analytics-collection-apis/), juntamente com os outros métodos de coleta do lado do servidor:

* [API de Inserção de Dados](https://developer.adobe.com/analytics-collection-apis/methods/data-insertion/): Enviar dados do evento uma ocorrência por vez, como uma cadeia de caracteres de consulta (solicitação de imagem) ou um XML `POST`.
* [API de Inserção de Dados em Massa](https://developer.adobe.com/analytics-collection-apis/methods/bulk-data-insertion/): carregue lotes de dados de chamada de servidor como arquivos. A Adobe recomenda o uso da API de inserção de dados em massa para novas implementações do lado do servidor.

## Perguntas frequentes

+++Isso afeta meus projetos existentes do Adobe Developer para as APIs do Analytics?

Todos os projetos existentes que usam as APIs do Analytics 1.4 serão afetados. Essas integrações devem ser migradas para as [APIs do Adobe Analytics 2.0](https://developer.adobe.com/analytics-apis/docs/2.0/).

+++

+++Compartilhei minhas credenciais do Adobe com outro produto ou aplicativo que usa as APIs do Analytics. Eles serão afetados?

Se esse produto ou aplicativo usar a credencial WSSE ou chamar as APIs do Analytics 1.4, ele será afetado e deverá migrar. Entre em contato com o fornecedor de produtos ou aplicativos para obter detalhes sobre os planos de migração e o cronograma.

+++

+++Como posso determinar qual API meu projeto usa?

O URL de base chamado pelo projeto determina a versão da API usada. As APIs do Adobe Analytics 1.4 usavam os seguintes URLs base:

* `https://api.omniture.com`
* `https://api3.omniture.com`
* `https://api4.omniture.com`
* `https://api5.omniture.com`

As [APIs do Adobe Analytics 2.0](https://developer.adobe.com/analytics-apis/docs/2.0/) usam a seguinte URL base:

* `https://analytics.adobe.io`

Se qualquer um dos projetos de API chamar `api*.omniture.com`, eles usarão as APIs 1.4 desativadas do Adobe Analytics e deverão migrar para as APIs 2.0.

+++

+++Esse fim da vida útil afeta a coleta de dados?

Não. Este fim da vida útil **não** afeta a coleta direta de dados, como Tags, o Web SDK, o AppMeasurement ou a API de Inserção de Dados. No entanto, se você usar as APIs de Classificações ou Fontes de dados 1.4 para aprimorar seus dados, será necessário migrar esses fluxos de trabalho para as APIs do Adobe Analytics 2.0.

+++

Se você tiver mais dúvidas sobre esse fim de vida útil que não foram respondidas nesta página, entre em contato com a equipe de conta da Adobe.
