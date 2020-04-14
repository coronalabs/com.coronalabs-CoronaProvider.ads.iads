# iads.height()

> --------------------- ------------------------------------------------------------------------------------------
> __Type__              [Function][api.type.Function]
> __Return value__      none
> __Revision__          [REVISION_LABEL](REVISION_URL)
> __Keywords__          ads, advertising, iads
> __See also__          [ads.show()][plugin.ads-iads.show]
>						[iads.*][plugin.ads-iads]
> --------------------- ------------------------------------------------------------------------------------------


## Overview

Gets the height of the banner ad in content coordinates. This will only return the correct result after calling [ads.show()][plugin.ads-iads.show]. After the device has been rotated, you must call [ads.show()][plugin.ads-iads.show] again to get the new correct height.

## Syntax

	ads.height()
