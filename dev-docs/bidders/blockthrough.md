---
layout: bidder
title: Blockthrough
description: Prebid BT Bidder Adapter
biddercode: blockthrough
gvl_id: 815
usp_supported: true
coppa_supported: false
gpp_sids: usp
schain_supported: true
dchain_supported: false
userId: pubProvidedId, id5Id, criteo, sharedId, identityLink, unifiedId, userId
media_types: banner
floors_supported: true
fpd_supported: true
pbjs: true
pbs: false
multiformat_supported: will-not-bid
ortb_blocking_supported: false
sidebarType: 1
---

### Note

The BT Bid Adapter makes requests to the BT Server which supports OpenRTB.

Publishers should use the `ortb2` method of setting [First Party Data](https://docs.prebid.org/features/firstPartyData.html). The following fields are supported: site.content.data, site.ext.data., user.data, user.ext.data.

### Bid Params

{: .table .table-bordered .table-striped }
| Name | Scope | Description | Example | Type |
| -------- | -------- | --------------------------- | ------- | --------- |
| `ab` | required | Whether AdBlock is enabled. | `true` | `boolean` |
| `siteId` | required | A unique ID for your site. | `12345` | `string` |
