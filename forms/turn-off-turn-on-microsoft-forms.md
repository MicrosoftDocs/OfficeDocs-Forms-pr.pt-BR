---
title: Desativar ou ativar o Microsoft Forms
ms.author: jokay
author: dumptruckjon
manager: kathyl
audience: Admin
ms.topic: how-to
ms.service: forms-pro
ms.localizationpriority: high
description: Este artigo aborda como os administradores do Microsoft 365 podem desativar ou ativar o Microsoft Forms para toda a organização ou para pessoas específicas em sua organização.
ms.openlocfilehash: 2d1280bd7d61dc8b31cfb84dfeaced2662603e4f
ms.sourcegitcommit: 09bdc82ce67e74495b6c58d9c842e31c17956fc3
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/12/2021
ms.locfileid: "60951389"
---
# <a name="turn-off-or-turn-on-microsoft-forms"></a>Desativar ou ativar o Microsoft Forms

Por padrão, [Microsoft Forms](https://support.microsoft.com/office/what-is-microsoft-forms-6b391205-523c-45d2-b53a-fc10b22017c8) é ativado para todos em sua organização. Se você é um [administrador](https://support.microsoft.com/topic/eac4d046-1afd-4f1a-85fc-8219c79e1504), você pode [configurar o Microsoft Forms](https://support.microsoft.com/office/set-up-microsoft-forms-cc52287a-4550-464d-9a1b-457bf9df2240), então desativá lo ou ativá lo novamente para toda a sua organização ou apenas para pessoas específicas.

## <a name="turn-off-microsoft-forms-for-everyone-in-your-organization"></a>Desative o Microsoft Forms para todos em sua organização

1.  Entrar para [Microsoft Azure](https://portal.azure.com/).

2.  No painel da esquerda, clique**Azure Active Directory**.

3.  Clicar **Aplicativos Empresariais**.

4.  Navegar até os serviços necessários e repita as etapas 5-7 para ambos **Tipo de Aplicativo**\> **CollabDBService** e **Microsoft Applications** \> **Microsoft Forms**.
    
      - No campo de pesquisa na lista suspensa **Tipo de aplicativo**, digitar **CollabDBService**. Selecionar **CollabDBService** na lista de resultados da pesquisa.
    
      - Na lista suspensa **Tipo de Aplicativo**, selecionar **Aplicativos Microsoft**. No campo de pesquisa sob a lista suspensa **Tipo de Aplicativo**, digitar **Microsoft Forms**, e então selecionar **Microsoft Forms** na lista de resultados da pesquisa.

5.  Em **Gerenciar**, clicar **Propriedades**.

6.  Para a opção, **Habilitado para que os usuários se inscrevam?**, selecionar **Não**.

7.  Clique em **Salvar**.

## <a name="turn-off-microsoft-forms-for-specific-people-in-your-organization"></a>Desativar o Microsoft Forms para pessoas específicas em sua organização

1.  Entrar no Microsoft 365 com sua conta de trabalho ou escola como administrador global. [Saiba como se inscrever](https://support.microsoft.com/office/where-to-sign-into-microsoft-365-for-business-e9eb7d51-5430-4929-91ab-6157c5a050b4).

2.  No Centro de administração do Microsoft 365, escolher **Usuários** \> **Usuários ativos**.

3.  Selecionar a caixa ao lado do nome da pessoa para a qual você deseja desativar o Microsoft Forms.

4.  Na faixa de opções, clique **Gerenciar licenças de produtos**.

5.  No formulário de conta que é aberto, na guia **Licenças e Aplicativos**, expanda a seção Aplicativos e role baixo até a opção Microsoft Forms. 

    :::image type="content" source="./media/turn-forms-off-on-licenses-apps.jpg" alt-text="Formulário de opções de conta no Centro de Administração Microsoft 365":::

6.  Desmarcar a caixa para desativar o Microsoft Forms. Para ativá lo, selecionar a caixa de seleção.

    :::image type="content" source="./media/turn-forms-off-on-plan-e1.jpg" alt-text=" Alternância do Microsoft Forms":::

     > [!Note]
     > [Verifique esta lista](https://support.microsoft.com/office/office-licenses-that-include-microsoft-forms-efa14679-5d99-47c5-bdf1-2fc838767f7e) para ver se você tem uma licença Office que inclui o Microsoft Forms. Se sua licença estiver listada, você precisará limpar a caixa de seleção Microsoft Forms para desativar completamente o acesso do usuário.

7.  Na parte inferior da lista **Aplicativos**, clique **Salvar Alterações**.

## <a name="i-turned-on-microsoft-forms-but-people-in-my-organization-still-cant-access-it"></a>Eu ativei o Microsoft Forms, mas as pessoas da minha organização ainda não conseguem acessá-lo.

Verifique a seguinte configuração no Microsoft Azure para garantir que o Microsoft Forms esteja habilitado:

1.  Entrar para [Microsoft Azure](https://portal.azure.com/).

2.  No painel da esquerda, clique**Azure Active Directory**.

3.  Clicar **Aplicativos Empresariais**.

4.  Navegar até os serviços necessários e repita as etapas 5-7 para ambos **Tipo de Aplicativo**\> **CollabDBService** e **Microsoft Applications** \> **Microsoft Forms**.
    
      - No campo de pesquisa na lista suspensa **Tipo de Aplicativo**, digitar **CollabDBService**. Selecionar **CollabDBService** na lista de resultados da pesquisa.
    
      - Na lista suspensa **Tipo de Aplicativo**, selecionar **Aplicativos Microsoft**. No campo de pesquisa sob a lista suspensa **Tipo de Aplicativo**, digitar **Microsoft Forms**, e então selecionar **Microsoft Forms** na lista de resultados da pesquisa.

5.  Em **Gerenciar**, clicar **Propriedades**.

6.  Para a opção, **Habilitado para que os usuários se inscrevam?**, selecionar **Sim**.

7.  Clique em **Salvar**.

    >[!Note]
    >Os serviços Microsoft Office SharePoint Online também devem ser habilitados para que as pessoas de sua organização possam acessar o Microsoft Forms.

## <a name="feedback-for-microsoft-forms"></a>Comentários do Microsoft Forms

Queremos ouvir de você\! Para enviar comentários sobre o Microsoft Forms, vá para o canto superior direito do seu formulário e selecione **Mais configurações de formulário** ![botão Mais Opções](./media/image2.png) \> **Comentários**.

