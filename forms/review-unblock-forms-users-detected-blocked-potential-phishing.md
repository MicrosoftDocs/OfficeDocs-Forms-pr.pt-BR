---
title: Revisar e desbloquear formulários ou usuários detectados e bloqueados por possíveis phishing
ms.author: jokay
author: dumptruckjon
manager: kathyl
audience: Admin
ms.topic: how-to
ms.service: forms-pro
ms.localizationpriority: high
description: Microsoft Forms permite que as revisões automatizadas de computadores detectem proativamente a coleta de dados confidenciais mal-intencionados em formulários e pesquisas. Se você for um administrador global e/ou de segurança, poderá fazer logon no Centro de administração do Microsoft 365 para examinar e desbloquear formulários detectados e bloqueados por possíveis tentativas de phishing e mal-intencionadas.
ms.openlocfilehash: dd4b92c09393db4c81ac5e7711ee7331ac35558e
ms.sourcegitcommit: 09bdc82ce67e74495b6c58d9c842e31c17956fc3
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/12/2021
ms.locfileid: "60951411"
---
# <a name="review-and-unblock-forms-or-users-detected-and-blocked-for-potential-phishing"></a>Revisar e desbloquear formulários ou usuários detectados e bloqueados por possíveis phishing

O Microsoft Forms habilita revisões automáticas de computador para detectar proativamente a coleta mal-intencionada de dados confidenciais em formulários e impedir temporariamente que esses formulários coletem respostas. Saiba mais sobre o [Microsoft Forms e a prevenção proativa contra phishing](https://support.microsoft.com/office/microsoft-forms-and-proactive-phishing-prevention-b3950a20-296d-4e8e-96f5-594ced998a90).

>[!Note]
>As etapas neste documento também se aplicam a [Voz do Cliente do Dynamics 365](https://go.microsoft.com/fwlink/p?linkid=2128500) (anteriormente conhecido como Forms Pro). Observe que uma licença da Voz do Cliente do Dynamics 365 é necessária para desbloquear pesquisas da Voz do Cliente do Dynamics 365. [Saiba mais](/dynamics365/customer-voice/help-hub).

## <a name="review-alerts-in-the-microsoft-365-defender-portal"></a>Examinar alertas no portal Microsoft 365 Defender

Se você for um administrador global ou de segurança, receberá alertas no portal do [Microsoft 365 Defender](https://security.microsoft.com/) sobre possíveis formulários de phishing para os quais você pode tomar medidas.

>[!Note]
> Se você for um administrador global, receberá mensagens de privacidade de dados para sua organização, incluindo notificações diárias de qualquer formulário criado em seu locatário que tenha sido detectado e bloqueado para possíveis phishing. Você verá essas notificações no [Centro de Mensagens](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter) procurando **Notificação de Phishing do Microsoft Forms**. (Se você não vir essa notificação na guia/exibição **Todas as mensagens ativas**, poderá encontrá-la na guia/exibição **Mensagens não enviadas**.) Para cada notificação, selecione o link ou links **URL de revisão do administrador do Forms** para examinar formulários bloqueados.  
  
Para que os administradores de segurança também recebam notificações sobre possíveis formulários de phishing, os administradores globais precisam atribuir a função [Leitor de Privacidade do Centro de Mensagens](/azure/active-directory/roles/permissions-reference#message-center-privacy-reader) a eles. Para saber mais sobre o Centro de mensagens, consulte [perguntas frequentes](/microsoft-365/admin/manage/message-center). Veja também como [definir preferências de email para mensagens de privacidade de dados](/microsoft-365/admin/manage/message-center#preferences).

1.  Entre no portal do [Microsoft 365 Defender](https://security.microsoft.com/).

2.  Selecione **Incidentes e alertas** \> **Alertas**. Você pode ver um ou todos os seguintes alertas do Forms:
    
      - **Usuário impedido de compartilhar formulários e coletar respostas**
    
      - **Formulário sinalizado e confirmado como phishing**
    
      - **Formulário bloqueado devido a uma possível tentativa de phishing**

3.  Selecione um alerta para revisá-lo. Para examinar o formulário que foi sinalizado, toque ou clique nos três pontos no canto inferior direito ao lado do botão **Gerenciar alerta** e selecione **Examinar este formulário**.
 
    :::image type="content" source="./media/review-unblock-forms-review-this-form.png" alt-text="Exibir esta opção de formulário":::

    >[!Tip]
    >Saiba mais sobre [políticas de alerta no Microsoft 365](/microsoft-365/compliance/alert-policies).

## <a name="unblock-a-form-or-confirm-its-phishing-attempt"></a>Desbloquear um formulário ou confirmar sua tentativa de phishing

Para cada formulário revisado, você pode optar por desbloqueá-lo ou confirmar o phishing.

### <a name="unblock"></a>Desbloquear

Selecione **Desbloquear** se você não acredita que um formulário é mal-intencionado.

>[!Note]
>Se alguém em seu locatário solicitar que você desbloqueie o formulário, sugerimos que você solicite informações específicas do formulário (por exemplo, data e hora do bloqueio, título) para identificar com mais eficiência a notificação no centro de administração. Como as notificações são enviadas diariamente e incluem todos os formulários detectados nas últimas 24 horas, as informações identificáveis para o formulário serão úteis.

### <a name="confirm-phishing"></a>Confirmar phishing

Selecione **Confirmar phishing** se você acredita que um formulário é mal-intencionado. O formulário será bloqueado permanentemente e seu proprietário não poderá mais editá-lo ou excluí-lo.

Depois de selecionar **Confirmar phishing**, clique ou toque em **Excluir formulário** para excluir permanentemente o formulário do seu locatário. Sugerimos fortemente a redefinição imediata de senha para uma conta em seu locatário que você acredita ter sido comprometida.

>[!Tip]
>Sua seleção de **Confirmar phishing** ajuda o Microsoft Forms a melhorar sua precisão de detecção. 

## <a name="commonly-asked-questions"></a>Perguntas comuns

**Quando vou examinar um formulário bloqueado, por que não vejo opções para desbloqueá-lo ou confirmar phishing?**

Após a revisão, você poderá ver que um bloco de um formulário já foi removido. Isso significa que, entre o momento em que um formulário foi bloqueado e o momento em que você o examinou, o proprietário do formulário removeu palavras-chave que foram sinalizadas para possíveis phishing. Nesse cenário, nenhuma ação adicional sua é necessária.

**Se um formulário tiver sido bloqueado por phishing confirmado, posso removê-lo?**

Se o formulário já tiver sido bloqueado por phishing confirmado, selecione **Excluir formulário** para removê-lo do seu locatário.

**E se eu não executar nenhuma ação em um formulário bloqueado?**

Se você optar por não executar uma ação (desbloqueie um formulário ou confirme sua intenção de phishing), o formulário permanecerá bloqueado. O proprietário do formulário ainda pode editar o formulário e remover palavras-chave que foram sinalizadas para possíveis phishing.

**E se eu quiser editar ou excluir o conteúdo bloqueado no formulário?**

Se você preferir editar e/ou excluir o conteúdo bloqueado, poderá gerar uma página de coautoria e gerenciar o formulário como coautoria. Para fazer isso, clique no link **abrir uma página de coautoria** localizado no sistema de mensagens acima do formulário que você está revisando.

## <a name="remove-restrictions-for-blocked-microsoft-forms-users"></a>Remover restrições para usuários Microsoft Forms bloqueados

Microsoft Forms impede que os usuários que repetidamente tenham tentado coletar informações pessoais ou confidenciais distribuam formulários e coletem respostas. Os administradores globais serão notificados sobre esses usuários bloqueados por meio do [Centro de mensagens](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter). Se você acredita que um usuário bloqueado não atende a nenhuma intenção mal-intencionada e sua conta é segura, você pode executar as etapas a seguir para desbloqueá-lo.

>[!Note]
>Os administradores de segurança também podem receber notificações sobre possíveis formulários de phishing depois que um administrador global atribui a função [Leitor de Privacidade do Centro de Mensagens](/azure/active-directory/roles/permissions-reference#message-center-privacy-reader) a eles.

1.  Vá para o [Centro de Mensagens](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter) e procure a notificação, **Previnir/Corrigir: Microsoft Forms Detectou Possível Phishing**.

    >[!Note]
    >Se você não vir essa notificação na guia/exibição **Todas as mensagens ativas**, poderá encontrá-la na guia/exibição **Mensagens não enviadas**.
 
    Essa notificação contém uma lista de usuários em seu locatário que estão impedidos de compartilhar formulários e coletar respostas.

2.  Clique no link fornecido na notificação para examinar os usuários bloqueados.

3.  Para cada usuário que você acredita que não tem intenção mal-intencionada, você pode optar por clicar no link **Desbloquear** na coluna **Ações** associada a esse usuário.

    >[!Note]
    >Se você acredita que um usuário tem intenção mal-intencionada, nenhuma ação adicional sua é necessária.

    >[!Note]
    >Pode levar até 30 minutos para que as restrições sejam removidas.

