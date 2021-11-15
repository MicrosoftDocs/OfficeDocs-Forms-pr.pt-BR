---
title: Informações do administrador
ms.author: jokay
author: dumptruckjon
manager: kathyl
audience: Admin
ms.topic: how-to
ms.service: forms-pro
ms.localizationpriority: high
description: Este artigo responde às perguntas mais frequentes sobre informações de administrador para o icrosoft Forms.
ms.openlocfilehash: 3fed9f104b6a44a7c23221b204796b22c8fb5109
ms.sourcegitcommit: 09bdc82ce67e74495b6c58d9c842e31c17956fc3
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/12/2021
ms.locfileid: "60951398"
---
# <a name="admin-information"></a>Informações do administrador

## <a name="getting-started"></a>Introdução

**Como desativar ou ativar o Microsoft Forms**

Por padrão, o Microsoft Forms é ativado para todos em uma organização. Os administradores de TI do Microsoft 365 de TI podem desativar o Microsoft Forms no Centro de administração do Microsoft 365, na guia **Gerenciamento do Usuário**. Consulte [Configurar o Microsoft Forms](set-up-microsoft-forms.md) e [Desativar ou ativar o Microsoft Forms](turn-off-turn-on-microsoft-forms.md) para obter mais detalhes.

**Como dar ao Microsoft Forms acesso somente a pessoas específicas em minha organização?**

Os administradores podem alterar as permissões de acesso para pessoas específicas na organização. Consulte [Configurações de administrador no Microsoft Forms](administrator-settings-microsoft-forms.md).

## <a name="data-storage"></a>Armazenamento de dados

**Onde os dados são armazenados para o Microsoft Forms?**

Os dados do Microsoft Forms dados são armazenados em servidores no Estados Unidos, com exceção dos dados para locatários baseados na Europa. Os dados do Insights para locatários europeus são armazenados em servidores na Europa.

## <a name="user-activity"></a>Atividade do usuário

**Como ver as atividades executadas no Microsoft Forms por pessoas em minha organização?**

Você pode examinar as [atividades do Microsoft Forms](/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance?view=o365-worldwide#microsoft-forms-activities) no log de auditoria do [Centro de segurança do Microsoft 365](https://security.microsoft.com/?rfr=OfficeScc). Saiba mais sobre [Auditoria no Office 365 (para administradores)](https://support.microsoft.com/topic/auditing-in-office-365-for-admins-9f6484d2-0fd2-17de-165f-c41346023906).

## <a name="user-account-information"></a>Informações da conta do usuário

**Como verificar se uma conta de usuário foi "excluída permanentemente"? **

1. Os administradores podem fazer logon no [Microsoft Graph](https://developer.microsoft.com/graph/graph-explorer).

2. Na caixa de pesquisa superior, cole a seguinte URL:

   `https://graph.microsoft.com/v1.0/directory/deletedItems/microsoft.graph.user?$filter=mail eq '*user email*'`

   >[!Note]
   >*email do usuário* = Endereço de email do proprietário do formulário que saiu da sua organização e/ou cuja conta foi desabilitada.

3. Clique em **Executar consulta**.

Se as informações da conta que você está procurando forem retornadas em sua consulta, isso significa que a conta foi excluída de forma reversível e está dentro do limite de 30 dias. Um administrador global pode transferir os formulários pertencentes à conta excluída por software usando o método de transferência, conforme descrito anteriormente.

Se as informações da conta que você está procurando não forem retornadas em sua consulta, isso significa que a conta ainda existe no locatário do Office 365 ou foi excluída há mais de 30 dias. Se a conta existir ou estiver em um estado desabilitado no locatário do Office 365, um administrador global poderá transferir os formulários pertencentes à conta. Se a conta foi "excluída de forma permanente" do locatário do Office 365, um administrador global não poderá transferir os formulários que eram de propriedade dessa conta. Esses formulários também não são recuperáveis.

**Há um limite para o número de usuários e a quantidade de dados armazenados para contas de usuário mesmo depois que eles tiverem deixado minha organização?**

Atualmente, não há limite para o número de usuários para os quais os dados são retidos, desde que o provisionamento de suas contas esteja dentro do contrato de serviço online da sua organização. Também não há limite para a quantidade de dados armazenados para contas de usuário.

**O que acontece com os dados de um formulário se a licença do proprietário do Microsoft Forms tiver sido removida ou o usuário for desabilitado ou excluído do seu locatário (Azure AD)?**

Se a licença de proprietário tiver sido removida ou a conta do proprietário estiver desabilitada, não haverá nenhuma alteração na quantidade de dados armazenados para a conta de usuário.

Se uma conta de usuário tiver sido excluída do seu locatário (Azure AD), todos os dados relacionados à conta serão excluídos 30 dias após a exclusão do usuário.

## <a name="form-ownership-transfer"></a>Transferência de propriedade do formulário

**O proprietário original de um formulário não está mais na minha organização. Como posso transferir a propriedade do formulário?**

Para transferir o formulário de alguém que saiu da sua organização, os seguintes requisitos devem ser atendidos:

  - Você é o administrador global da organização e tem uma licença válida do Forms.

  - O funcionário cujo formulário você deseja transferir tem uma conta que foi excluída ou desabilitada.

  - O formulário é transferido dentro de 30 dias após a exclusão de uma conta.

> [!Note]
> Não há restrição de tempo para transferir a propriedade de um formulário de uma conta que foi desabilitada (e não excluída).

1. Se todos os requisitos forem atendidos, você poderá transferir a propriedade do formulário. Na barra de endereços do navegador, substitua a URL existente pelo seguinte:

    `https://forms.office.com/Pages/delegatepage.aspx? originalowner=\[*email address*\]`

   >[!Note]
   >*Email do usuário* = Endereço de email do proprietário do formulário que saiu da sua organização e/ou cuja conta foi desabilitada.
   > Por exemplo, se o proprietário do formulário ("Jason Fabian") deixou sua organização ("Contoso"), sua URL de solução alternativa teria esta aparência: `https://forms.office.com/Pages/delegatepage.aspx?originalowner=JasonFabian@contoso.com`

2. Agora você tem acesso aos formulários do ex-funcionário. No formulário que você deseja transferir, clique em **Mais ações de formulário**![Mais botões de opções](./media/image2.png), e selecione **Mover**.

   >[!Note]
   >Se você estiver tentando transferir a propriedade do formulário para um funcionário ativamente em sua organização, poderá movê-lo para um grupo ao qual ele pertence. Se você ainda não for um membro desse grupo, deverá ingressá-lo para executar a transferência. Depois que a transferência de propriedade do formulário for concluída, você poderá optar por sair do grupo.

**Quando tento transferir a propriedade de um formulário, por que recebo um erro?**

Se você receber uma mensagem de erro, qualquer uma das seguintes condições poderá impedir que você transfira a propriedade:

|Mensagem de erro|Explicação|
| --- | --- |
| ***Não é possível acessar esta página***<br/><br/>O proprietário do formulário&#39;s ainda tem uma conta ativa. | O proprietário do formulário ainda tem uma licença e uma conta ativas do Forms. |
| ***Não é possível acessar esta página***<br/><br/>Verifique se você&#39; inseriu o endereço de email corretamente e se a conta de proprietário dos formulários não foi excluída há mais de 30 dias. | O endereço de email está escrito incorretamente e/ou a conta do proprietário dos formulários foi excluída há mais de 30 dias. |
| ***Não é possível acessar esta página***<br/><br/>Verifique se você&#39; inseriu o endereço de email corretamente e tente novamente. | O endereço de email está ausente ou digitado incorretamente. |

## <a name="forms-usage-in-outlook-or-powerpoint"></a>Uso de formulários no Outlook ou no PowerPoint

**Pessoas em minha organização não podem adicionar uma Votação a uma mensagem de email do Outlook. Como corrigir isso?**

A configuração de **Autenticação moderna** para o Outlook precisa ser habilitada para garantir que as pessoas em sua organização possam [Criar uma votação no Outlook](https://support.microsoft.com/office/create-a-poll-in-outlook-46893563-ab12-4bd0-aff7-26f5a488fea0).

1. Entre no [https://admin.microsoft.com](https://admin.microsoft.com/) com sua conta corporativa ou de estudante.

2. Selecione **Configurações** \>**Configuração da organização**.

   >[!Note]
   > Se você não vir a opção **Configuração**, selecione ![Mais botões de opções](./media/image2.png)**Mostrar todos** no painel esquerdo.

3.  Selecione **Autenticação moderna**.

4.  Verifique a opção, **Ativar  a autenticação moderna para o Outlook 2013 para Windows e posterior (recomendado).**.

Saiba mais sobre a autenticação moderna e [multifator](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication?view=o365-worldwide) e como configurá-la e distribuí-la para sua organização.

**Não quero implantar suplementos do Office para toda a organização. As pessoas em minha organização ainda podem usar o suplemento Formulários para o PowerPoint?**

Sim, você pode usar a [Implantação centralizada](/office/dev/add-ins/publish/centralized-deployment) para implantar apenas o suplemento do Forms para PowerPoint.

1.  Entre no [https://admin.microsoft.com](https://admin.microsoft.com/) com sua conta corporativa ou de estudante.

2.  Selecione **Configurações** \>**Suplementos**.

    >[!Note]
    >Se você não vir a opção **Configurações**, selecione o ![botão Mais opções](./media/image2.png)**Mostrar tudo** no painel esquerdo..

3.  Na lista de **Suplementos**, selecione **Formulários**.

4.  Em **Atribuição de usuários** no painel **Editar formulários**, selecione **Todos**.

5.  Selecione **Salvar**.


## <a name="forms-and-anti-phishing"></a>Formulários e anti-phishing

**O que posso fazer sobre phishing e possíveis intenções mal-intencionadas em formulários dentro do meu locatário?**

No Microsoft Forms, habilitamos revisões automáticas de computador para detectar proativamente a coleta mal-intencionada de dados confidenciais em formulários e impedir temporáriamente que esses formulários coletem respostas.

Saiba mais sobre o [Microsoft Forms e a prevenção proativa contra phishing](https://support.microsoft.com/office/microsoft-forms-and-proactive-phishing-prevention-b3950a20-296d-4e8e-96f5-594ced998a90).

Se você for um administrador global e/ou de segurança, poderá fazer logon no centro de administração do Microsoft 365 em [admin.microsoft.com](https://admin.microsoft.com/) e ir para o [Centro de mensagens](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter). Aqui, você obterá um resumo diário de todos os formulários bloqueados. Para cada formulário listado, você pode optar por desbloqueá-lo ou confirmar sua tentativa de phishing. Saiba mais sobre como [revisar e desbloquear formulários ou usuários detectados e bloqueados por possível pratica de phishing](review-unblock-forms-users-detected-blocked-potential-phishing.md).
