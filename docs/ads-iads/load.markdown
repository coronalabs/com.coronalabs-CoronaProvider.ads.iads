# iads.load()

> --------------------- ------------------------------------------------------------------------------------------
> __Type__              [Function][api.type.Function]
> __Return value__      none
> __Revision__          [REVISION_LABEL](REVISION_URL)
> __Keywords__          ads, advertising, iads
> __See also__          [ads.show()][plugin.ads-iads.show]
>						[ads.isLoaded()][plugin.ads-iads.isLoaded]
>						[iads.*][plugin.ads-iads]
> --------------------- ------------------------------------------------------------------------------------------


## Overview

Preloads an ad. Only works with the string `"interstitial"` for the first argument. You can also call [ads.isLoaded()][plugin.ads-iads.isLoaded] to verify that the ad has been loaded and [ads.show()][plugin.ads-iads.show] to show it.


## Syntax

	ads.load( adUnitType )

##### adUnitType ~^(required)^~
_[String][api.type.String]._ The type of ad to show. iAds supports `"interstitial"` for this command.


## Example

``````lua
local ads = require( "ads" )

local function adListener( event )
	if ( event.isError ) then
		-- Failed to receive an ad
	else
		ads.show( "interstitial" )
	end

end
 
ads.init( "iads", "123456789", adListener )

ads.load( "interstitial" )
``````