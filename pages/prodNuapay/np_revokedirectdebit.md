---
title: Revoke Direct Debit
keywords: Revoke Direct Debit
summary: "Revoke Direct Debit RESTful API"
sidebar: np_sidebar
permalink: np_revokedirectdebit.html
folder: prodNuapay
toc: false
---

## API Details

When you first create a Direct Debit it has a status of <b>READY FOR EXPORT</b>. Once it is forwarded from Nuapay on to <a href="#" data-toggle="tooltip" data-original-title="{{site.data.glossary.clearing}}">Clearing</a> for processing, its status is updated to <b>EXPORTED</b>.

If you decide that you do not want to settle the payment and do not want to pass it on for further processing at Clearing, you may revoke it.


{% include tip.html content="The Revoke operation is only possible for payments that are in READY FOR EXPORT status. For more information see [Direct Debit Statuses](np_ddstatuses.html)." %}


{% include swagger_np.html %}

{% include urls.html %}


<ul id="profileTabs" class="nav nav-tabs">
    
   
</ul>
   
{% include redoc.html %}
   
loadRedoc('#profileTabs', 'https://sentenial.github.io/nuapay-swagger/docs/redoc.html');
var timerRef = setInterval(function() { getDocs('operation/revokeDirectDebitUsingPOST','#profileTabs',timerRef); }, 500);


</script>


<div id="mydiv"></div>
</div>
</div>
{% include links.html %}
