---
title: Azure サブスクリプションの状態
description: この記事では、Azure サブスクリプションのさまざまな状態について説明します。
keywords: Azure サブスクリプションの状態
author: anuragdalmia
ms.reviewer: banders
tags: billing
ms.service: cost-management-billing
ms.subservice: billing
ms.topic: conceptual
ms.date: 08/20/2020
ms.author: andalmia
ms.openlocfilehash: 70d03b4aeeaecee522552b381ce1309485719dc6
ms.sourcegitcommit: 56cbd6d97cb52e61ceb6d3894abe1977713354d9
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/20/2020
ms.locfileid: "88686685"
---
# <a name="azure-subscription-states"></a>Azure サブスクリプションの状態

この記事では、Azure サブスクリプションのさまざまな状態について説明します。 これらの状態は、Azure portal のサブスクリプション領域に **[状態]** として表示されます。

| サブスクリプションの状態 | 説明 |
|-------------| ----------------|
| **アクティブ**/**有効** | Azure サブスクリプションがアクティブです。 このサブスクリプションを使用して、新しいリソースをデプロイしたり既存のリソースを管理したりできます。<br><br>[サブスクリプションに登録された](../../azure-resource-manager/management/resource-providers-and-types.md#azure-portal)リソースプロバイダーに対してすべての操作 (PUT、PATCH、DELETE、POST、GET) が利用できます。 |
| **削除済み** | ご利用の Azure サブスクリプションは、基になるすべてのリソースおよびデータと共に削除されました。<br><br>いずれの操作も利用できません。 |
| **Disabled** | ご利用の Azure サブスクリプションは無効化され、Azure リソースの作成や管理に使用することはできなくなりました。 この状態では、仮想マシンの割り当てが解除されて、一時 IP アドレスが解放され、ストレージが読み取り専用になって、他のサービスが無効化されます。 サブスクリプションは、クレジットの有効期限が切れている、使用制限に達している、 請求の支払期限が過ぎている、 クレジット カードの限度額を超えている、 明示的に無効化 (キャンセル) された などの理由で無効にされることがあります。 サブスクリプションは、その種類によって 1 日から 90 日、無効状態で維持されます。 その期間が経過した後、完全に削除されます。 詳細については、「[無効な Azure サブスクリプションを再度有効にする](subscription-disabled.md)」を参照してください。<br><br>リソースを作成したり更新したりする操作 (PUT、PATCH) は無効です。 アクションを実行する操作 (POST) も無効となります。 リソースを取得または削除することはできます (GET、DELETE)。 リソースは引き続きご利用いただけます。 |
| **Expired** | キャンセルされた Azure サブスクリプションは期限切れとなります。 期限切れのサブスクリプションは再度有効にすることができます。 詳細については、「[無効な Azure サブスクリプションを再度有効にする](subscription-disabled.md)」を参照してください。<br><br>リソースを作成したり更新したりする操作 (PUT、PATCH) は無効です。 アクションを実行する操作 (POST) も無効となります。 リソースを取得または削除することはできます (GET、DELETE)。|
| **期限経過** | Azure サブスクリプションの支払いが未払いのまま保留状態になっています。 サブスクリプションは引き続きアクティブ状態ですが、支払い義務を怠ると、サブスクリプションが無効化されることがあります。 詳細については、「[支払期限を過ぎた Azure サブスクリプション未払い額の支払い](resolve-past-due-balance.md)」を参照してください。<br><br>すべての操作を利用できます。 |
| **警告あり** | ご自分の Azure サブスクリプションは警告ありの状態で、その間は正常に使用できますが、警告理由が解決されない場合は、すぐに無効になります。 期限切れになった場合、ユーザーによって取り消された場合、サブスクリプションが期限切れになった場合は、サブスクリプションは警告ありの状態になることがあります。<br><br>すべての操作を利用できます。 |
