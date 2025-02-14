---
title: 恢复已删除的仓库
<<<<<<< Updated upstream
<<<<<<< Updated upstream
intro: '{% ifversion ghes or ghae %}企业所有者{% elsif fpt or ghec %}您{% endif %} 可以还原某些已删除的存储库以恢复其内容。'
=======
intro: '{% ifversion ghes or ghae %}An enterprise owner{% elsif fpt or ghec %}You{% endif %} can restore some deleted repositories to recover their contents.'
>>>>>>> Stashed changes
=======
intro: '{% ifversion ghes or ghae %}An enterprise owner{% elsif fpt or ghec %}You{% endif %} can restore some deleted repositories to recover their contents.'
>>>>>>> Stashed changes
permissions: '{% ifversion ghes or ghae %}{% elsif fpt or ghec %}Anyone can restore deleted repositories that were owned by their own personal account. Organization owners can restore deleted repositories that were owned by the organization.{% endif %}'
redirect_from:
  - /articles/restoring-a-deleted-repository
  - /github/administering-a-repository/restoring-a-deleted-repository
  - /github/administering-a-repository/managing-repository-settings/restoring-a-deleted-repository
versions:
  fpt: '*'
  ghec: '*'
  ghes: '*'
  ghae: '*'
topics:
  - Repositories
shortTitle: 恢复已删除的仓库
---

{% ifversion ghes or ghae %}

<<<<<<< Updated upstream
<<<<<<< Updated upstream
通常，{% ifversion ghes %}{% data variables.product.product_location %}上{% endif %}已删除的存储库可以在 90 天内由企业所有者恢复。 更多信息请参阅“[恢复删除的仓库](/admin/user-management/managing-repositories-in-your-enterprise/restoring-a-deleted-repository)”。
=======
Usually, deleted repositories can be restored within 90 days by an enterprise owner{% ifversion ghes %} on {% data variables.product.product_location %}{% endif %}. 更多信息请参阅“[恢复删除的仓库](/admin/user-management/managing-repositories-in-your-enterprise/restoring-a-deleted-repository)”。
>>>>>>> Stashed changes
=======
Usually, deleted repositories can be restored within 90 days by an enterprise owner{% ifversion ghes %} on {% data variables.product.product_location %}{% endif %}. 更多信息请参阅“[恢复删除的仓库](/admin/user-management/managing-repositories-in-your-enterprise/restoring-a-deleted-repository)”。
>>>>>>> Stashed changes

{% else %}

## 关于仓库恢复

删除的仓库可在 90 天内恢复，除非仓库是目前非空白的复刻网络的一部分。 复刻网络由父仓库、仓库的复刻以及该仓库复刻的复刻组成。 如果仓库是复刻网络的一部分，则在网络中的每个其他仓库被删除或者从网络中脱离之前，无法恢复它。 有关复刻的更多信息，请参阅“[关于复刻](/pull-requests/collaborating-with-pull-requests/working-with-forks/about-forks)”。

如果要恢复属于当前非空白的复刻网络一部分的仓库，可以联系 {% data variables.contact.contact_support %}。

仓库被删除后，可能需要一个小时才能恢复。

恢复仓库不会恢复发行版附件或团队权限。 已恢复的议题不会被标记。

## 恢复个人帐户所拥有的已删除仓库

{% data reusables.user-settings.access_settings %}
{% data reusables.user-settings.repo-tab %}
{% data reusables.user-settings.deleted-repos %}
{% data reusables.user-settings.restore-repo %}
{% data reusables.user-settings.restore-confirmation %}

## 恢复组织所拥有的已删除仓库


{% data reusables.profile.access_org %}
{% data reusables.profile.org_settings %}
{% data reusables.organizations.deleted-repos %}
{% data reusables.user-settings.restore-repo %}
{% data reusables.user-settings.restore-confirmation %}

## 延伸阅读

- "[删除仓库](/articles/deleting-a-repository)"

{% endif %}
