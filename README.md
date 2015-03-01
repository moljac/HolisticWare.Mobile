# HolisticWare.Mobile

HolisticWare.Mobile is a temporary step in moving Xamarin.Mobile to 

*	nuget package and 
*	empty shell component

NOTE: HolisticWare will be replaced with Xamarin

*	HolisticWare.Mobile -> Xamarin.Mobile
	*	HolisticWare.Mobile.XamarinShared -> Xamarin.Mobile.XamarinShared
	*	HolisticWare.Mobile.Contacts -> Xamarin.Mobile.Contacts
	*	HolisticWare.Mobile.Geolocation -> Xamarin.Mobile.Geolocation
	*	HolisticWare.Mobile.Media -> Xamarin.Mobile.Media

## Architecture / Structure

### Dependency Graph

*	HolisticWare.Mobile.Shared
*	HolisticWare.Mobile.Contacts
	*	HolisticWare.Mobile.Shared
*	HolisticWare.Mobile.Geolocation
	*	HolisticWare.Mobile.Shared
*	HolisticWare.Mobile.Media
	*	HolisticWare.Mobile.Shared
*	HolisticWare.Mobile
	*	HolisticWare.Mobile.Contacts
		*	HolisticWare.Mobile.Shared
	*	HolisticWare.Mobile.Geolocation
		*	HolisticWare.Mobile.Shared
	*	HolisticWare.Mobile.Media
		*	HolisticWare.Mobile.Shared

	
	
## Links / References

*	[https://github.com/xamarin/Xamarin.Mobile](https://github.com/xamarin/Xamarin.Mobile)
*	[https://components.xamarin.com/view/xamarin.mobile](https://components.xamarin.com/view/xamarin.mobile)


Note: 

*	[https://www.nuget.org/packages/xamstore-xamarin.mobile/](https://www.nuget.org/packages/xamstore-xamarin.mobile/)		
	packaga maintained by Paul Betts
		
		
		
## Steps

1.	split functionality into independent packages which can be used separately
	1.	Media
	2.	Geolocation		
	3.	Contacts
2.	merge all independent packages from 1. into nuget package that has dependencies on		
	independent packages:
	1.	HolisticWare.Mobile.Contacts
	2.	HolisticWare.Mobile.Geolocation
	3.	HolisticWare.Mobile.Media
3.	Create empty-shell component with 
	1.	nuget dependencies
	2.	samples

	
## Tools

*	David Folwler's (ASP.net v.5 AKA vNExt) proposal for .net library structure 
	*	[https://gist.github.com/davidfowl/ed7564297c61fe9ab814](https://gist.github.com/davidfowl/ed7564297c61fe9ab814)
	*	.net is undergoing modularization and ASP.net v.5 
		*	first technology that is utilizing nuget for everything
		*	Xamarin Components concepts are following similar approach	
*	David Whitney's implementation of the David Folwler's project structure (folder structure)
	*	[https://github.com/davidwhitney/DotNetLibraryTemplate](https://github.com/davidwhitney/DotNetLibraryTemplate)
	*	personal fork is in submodules-moljac/DotNetLibraryTemplate
	
	
	
## 	Roadmap

*	Uservoice		
	[https://xamarin.uservoice.com/forums/150476-xamarin-mobile-api](https://xamarin.uservoice.com/forums/150476-xamarin-mobile-api)
	