---
title: Configurar Microsoft Forms
ms.author: jokay
author: dumptruckjon
manager: kathyl
audience: Admin
ms.topic: how-to
ms.service: microsoft-365-education
ms.localizationpriority: high
description: Saiba como os administradores do Microsoft 365 podem controlar como o Microsoft Forms é usado em sua organização. Saiba também respostas a perguntas sobre segurança e conformidade, tais como onde os dados são armazenados para os Microsoft Forms.
ms.openlocfilehash: bb0e1a6ba8e2085550eb18a8bb393b34b197fe51
ms.sourcegitcommit: 80aa5565b4008855be844e8e5ab3f2779fba9a83
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/05/2022
ms.locfileid: "61723719"
---
# <a name="set-up-microsoft-forms"></a>Configurar Microsoft Forms

## <a name="overview"></a>Visão Geral

Os Microsoft Forms permitem que seus usuários criem rápida e facilmente testes personalizados, pesquisas, testes, registros e muito mais. Ao criar um teste ou formulário, você pode convidar outras pessoas para respondê-lo usando qualquer navegador da Web, mesmo em dispositivos móveis. Conforme os resultados são enviados, você pode usar as análises internas para avaliar as respostas. Os dados de formulários, como resultados de testes, podem ser facilmente exportados para o Excel para análise adicional ou atribuição de notas.

Para saber mais, confira [O que é o Microsoft Forms?](https://support.microsoft.com/office/what-is-microsoft-forms-6b391205-523c-45d2-b53a-fc10b22017c8) Ou, veja nossa [postagem no blog Microsoft 365](https://go.microsoft.com/fwlink/?linkid=852256) sobre o Microsoft Forms.

>[!Note]
>O Microsoft Forms estão geralmente disponíveis para clientes do Office 365 Education, clientes Microsoft 365 Apps para Pequenos e Médios negócios e clientes com uma conta Microsoft (Hotmail, Live, ou Outlook.com).

:::image type="content" source="./media/set-up-forms-team-event.png" alt-text="Visualização da aparência de um Formulário em um dispositivo móvel.":::

## <a name="configure"></a>Configurar

Os administradores do Microsoft 365 podem controlar como o Microsoft Forms são usados em sua organização através das seguintes tarefas:

|Tarefa de administrador   |Descrição   |
|----------|-----------|
|**Desativar ou ativar o Microsoft Forms**|O Microsoft Forms está ativada para sua organização por padrão. Você pode [desativar](turn-off-turn-on-microsoft-forms.md)a qualquer momento.|
|**Desativar o Microsoft Forms para pessoas individuais em sua organização**|Quando você desativa o Microsoft Forms para uma pessoa específica, ela não poderá usá-lo e o titulo *Forms* não será exibido para eles no Inicializador de aplicativos do Microsoft 365 ou página. Saiba como [desativar formulários para pessoas específicas](turn-off-turn-on-microsoft-forms.md).|
|**Configurar acesso condicional ao Azure Active Directory para Microsoft Forms**|Para configurar uma política de acesso condicional para Microsoft Forms, veja [Documentação do Acesso Condicional Azure Active Directory](/azure/active-directory/conditional-access) e inclua *Microsoft Form* em *Aplicativos em nuvem* tarefas. <br/><br/> **Observação:** Se os usuários em sua organização ainda forem bloqueados mesmo depois de configurar o acesso condicional para o Microsoft Forms, verifique se o Microsoft Office SharePoint Online e o Exchange Online também recebem acesso por meio de acesso condicional. [Saiba mais](/azure/active-directory/conditional-access/block-legacy-authentication).|
|**Controlar configurações de compartilhamento externo, registrar nomes de pessoas em sua organização, e/ou proteger formulários contra phishing**|No Centro de administração do Microsoft 365, você pode: <ul><li>Controle se usuários externos estão autorizados a colaborar com usuários de sua organização em um formulário ou teste.</li><li>Escolher se deseja ou não capturar os nomes das pessoas em sua org. que preenchem formulários.</li><li>Desativar ou ativar a detecção automática de phishing nos formulários.</li></ul><br/>Saiba mais sobre essas [configurações de administrador](administrator-settings-microsoft-forms.md).|
|**Habilitar usuários para inserir um formulário no PowerPoint**|<ol><li>Entre no https://admin.microsoft.com.</li><li>Clique em **Configurações** > **Configurações**.</li><li>Na página **Configurações** sob a guia **Serviços**, clique em **Aplicações e serviços de propriedade do usuário**.</li><li>Marque a opção, **Permitir os usuários acessarem a loja do Office**, para permitir que os usuários insiram um formulário no PowerPoint.</li></ol><br/>Lembre-se de que pode levar algumas horas para que a alteração entre em vigor. [Saiba mais](/microsoft-365/admin/manage/manage-deployment-of-add-ins)|

## <a name="security--compliance"></a>Segurança e conformidade

Se a sua empresa precisa atender a padrões técnicos, normativos e legais em relação a uso de dados e segurança de conteúdo, esta seção é para você.

**Onde os dados são armazenados para o Microsoft Forms?**

Os dados do Microsoft Forms são armazenados em servidores nos Estados Unidos e na Europa. Todos os dados estão localizados nos Estados Unidos, exceto para locatários sediados na Europa que começaram a usar o Microsoft Forms depois de maio de 2017. Seus dados são armazenados em bancos de dados na Europa.

**O Microsoft Forms está em conformidade?**

O Microsoft Forms cumpriram os requisitos de conformidade com a GDPR a partir de maio de 2018. Acesse [Solicitações do Titular dos Dados do Microsoft 365 para o GDPR](/microsoft-365/compliance/gdpr-dsr-office365?toc=/microsoft-365/enterprise/toc.json) para maiores informações.

**Há proteções FERPA e BAA em vigor?**

O Microsoft Forms atendem às normas [FERPA](https://www.microsoft.com/trustcenter/compliance/ferpa) e [BAA de proteção](https://www.microsoft.com/TrustCenter/Compliance/HIPAA).

**Há um limite para o número de usuários e a quantidade de dados armazenados para contas de usuário mesmo depois que eles tiverem deixado minha organização?**

Atualmente, não há limite para o número de usuários para os quais os dados são retidos, desde que o provisionamento de suas contas esteja dentro do contrato de serviço online da sua organização. Também não há limite para a quantidade de dados armazenados para contas de usuário.

**O proprietário original de um formulário não está mais com minha organização e/ou sua licença dos Microsoft Forms foi removida. O que acontece com os dados que estão associados ao formulário que eles criaram?**

Todos os dados relacionados à conta serão excluídos 30 dias depois que uma conta de usuário foi excluída do seu locatário (Microsoft Azure Active Directory).

## <a name="faq"></a>Perguntas frequentes

**Para que posso usar o Microsoft Forms?**

O Microsoft Forms é um aplicativo simples e leve que permite criar facilmente pesquisas, teste e enquetes. Em instituições educacionais, pode ser usado para criar testes, coletar comentários de professores e pais, ou planejar atividades de classe e funcionários. Em organizações empresariais, ele pode ser usado para coletar comentários dos clientes, medir a satisfação dos funcionários, melhorar seu produto ou negócio, ou organizar eventos da empresa.

**Quem pode usar o Microsoft Forms?**

O Microsoft Forms é gratuito para qualquer pessoa com uma conta Microsoft (Hotmail, Live, ou Outlook.com). Os seguintes aplicativos Office 365 Education e Microsoft 365 Apps para Pequenos e Médios negócios também podem usar o Microsoft Forms:

**Office 365 Education**

  - Office 365 A1 Plus

  - Office 365 A5

  - Clientes existentes que adquiriram o Microsoft Office 365 educacional E3 antes de sua desativação

**Microsoft 365 Apps para Pequenos e Médios Negócios**

  - Microsoft 365 Business Basic

  - Microsoft 365 Business Standard

  - Microsoft 365 Business Premium

  - Microsoft 365 Apps para empresas

  - Planos Microsoft 365 Enterprise E1, E3, e E5

  - Clientes existentes do Office 365 Enterprise E4 que compraram o E4 antes de sua desativação

Entre em [forms.office.com](https://forms.office.com/) e inicie a criação de pesquisas, testes e enquetes.

**As pessoas sem uma conta Microsoft 365 ainda podem enviar uma pesquisa ou teste no Microsoft Forms?**

Os autores do Microsoft Forms podem alternar suas configurações para permitir que usuários fora de sua organização respondam a sua pesquisa ou teste. Neste caso, os usuários estarão enviando respostas anonimamente. Se você quiser ver quem preencheu sua pesquisa ou teste, você pode solicitar que os respondentes preencham seus nomes como parte de seu questionário.

**Qual é o limite do número de formulários que podem ser criados e o número de respostas que um formulário pode receber?**

Os clientes do Office 365 Education e Microsoft 365 Apps para Pequenos e Médios negócios podem criar até 200 formulários e cada formulário pode receber até 50.000 respostas. Os usuários do Microsoft Forms com uma conta Microsoft (Hotmail, Live ou Outlook.com) podem criar até 200 formulários e cada formulário pode receber até 1.000 respostas para contas pagas e até 200 respostas para contas gratuitas. Saiba mais sobre [formulário, pergunta, resposta e limites de caracteres no Forms](https://support.microsoft.com/office/form-question-response-and-character-limits-in-microsoft-forms-ec15323d-92a4-4c33-bf88-3fdb9e5b5fea).

Se você precisar de mais respostas, recomendamos exportar as respostas existentes para uma pasta de trabalho Excel, e depois de desmarcar de sua pesquisa ou teste. Isto permitirá que você colete mais respostas depois de desmarcada.

**Com quais navegadores da Web a Microsoft Forms trabalha?**

Microsoft Forms está otimizado para Internet Explorer 11, Edge, Chrome (última versão), Firefox (última versão), Chrome no Android (última versão) e Safari no iOS (última versão).

**Em que idiomas o Microsoft Forms está disponível?**

Veja [idiomas suportados](https://support.microsoft.com/office/languages-supported-by-microsoft-forms-c17498cb-cbf6-4178-ae83-bd24934398ac) e [configurações de idioma](https://support.microsoft.com/office/language-settings-for-microsoft-forms-b282f9aa-0fe4-4290-b1e1-827a8a35ac27) para Microsoft Forms.

**O Microsoft Forms substituirá o Microsoft InfoPath?**

Não. O Microsoft InfoPath foi uma solução para criar formulários personalizáveis que podem permitir fluxos de trabalho automatizados, enquanto que Microsoft Forms é um aplicativo básico e leve para coletar informações rapidamente através de pesquisas e testes.

O Microsoft InfoPath está sendo substituído por Microsoft Office SharePoint Online Lists, Flow e PowerApps - soluções modernas para a digitalização de formulários tradicionais da empresa, automatizando fluxos de trabalho e transformando processos de negócios. [Saiba mais](https://products.office.com/business/business-process-automation).

**Onde posso enviar comentários, como bugs de produtos ou solicitações de recursos?**

Queremos saber sua opinião! Para enviar feedback sobre o Microsoft Forms, vá para o canto superior direito do seu formulário e selecione **Mais configurações de formulário** ![Botão de mais opções](./media/image2.png) > **Comentários**.

> [!Note]
> Veja [Perguntas mais frequentes sobre o Microsoft Forms](https://support.microsoft.com/office/frequently-asked-questions-about-microsoft-forms-495c4242-6102-40a0-add8-df05ed6af61c) para saber mais.

