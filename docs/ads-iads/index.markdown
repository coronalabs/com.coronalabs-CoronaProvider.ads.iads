# iads.*

> --------------------- ------------------------------------------------------------------------------------------
> __Type__              [CoronaProvider][api.type.CoronaProvider]
> __Library__           [ads.*][api.library.ads]
> __Revision__          [REVISION_LABEL](REVISION_URL)
> __Keywords__          ads, advertising, iads
> __Platforms__			iOS
> --------------------- ------------------------------------------------------------------------------------------

## Overview

The iAds plugin offers easy integration of iAds using the [ads][api.library.ads] library and [ads.init()][plugin.ads-iads.init].

## Syntax

	local ads = require( "ads" )

## Functions

#### [ads.init()][plugin.ads-iads.init]

#### [ads.show()][plugin.ads-iads.show]

#### [ads.hide()][plugin.ads-iads.hide]

#### [ads.height()][plugin.ads-iads.height]

#### [ads.isLoaded()][plugin.ads-iads.isLoaded]

#### [ads.load()][plugin.ads-iads.load]

#### [ads:getCurrentProvider()][api.type.CoronaLibrary.getCurrentProvider]

#### [ads:setCurrentProvider()][api.type.CoronaLibrary.setCurrentProvider]


## Events

#### [adsRequest][plugin.ads-iads.event.adsRequest]


## Project Settings

To use this plugin, add an entry into the `plugins` table of `build.settings`. When added, the build server will integrate the plugin during the build phase.

``````lua
settings =
{
	plugins =
	{
		["CoronaProvider.ads.iads"] =
		{
			publisherId = "com.coronalabs",
			supportedPlatforms = { iphone=true }
		},
	},		
}
``````


## Support

* [https://developer.apple.com/iad/](https://developer.apple.com/iad/)
* [Corona Forums](http://forums.coronalabs.com/forum/545-monetization-in-app-purchases-ads-etc/)
