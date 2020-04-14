# iads.init()

> --------------------- ------------------------------------------------------------------------------------------
> __Type__              [Function][api.type.Function]
> __Return value__      none
> __Revision__          [REVISION_LABEL](REVISION_URL)
> __Keywords__          ads, advertising, iads
> __See also__          [ads.show()][plugin.ads-iads.show]
>								[iads.*][plugin.ads-iads]
> --------------------- ------------------------------------------------------------------------------------------


## Overview

`ads.init()` initializes the Corona `ads` library by specifying the name of the ad network service provider and the app identifier.

Once the `ads` library is initialized, you can request an ad using [ads.show()][plugin.ads-iads.show].


## Syntax

	ads.init( providerName, appId [, adListener] )

##### providerName ~^(required)^~
_[String][api.type.String]._ String value for the provider name. For iAds, use `"iads"`.

##### appId ~^(required)^~
_[String][api.type.String]._ String containing the app ID from iTunes Connect, for example `"123456789"`.

##### adListener ~^(optional)^~
_[Listener][api.type.Listener]._ Listener function that will receive [adsRequest][plugin.ads-iads.event.adsRequest] events.