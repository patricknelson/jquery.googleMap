# jQuery Google Maps

Helper plugin for creating a Google Map


## Example usage

In this example, we're setting it up so that the tag itself is telling the plug-in which address to use via the "address" data attribute.

**HTML:**

    <div id="google-map" data-address="1501 Market Street,Philadelphia, PA 19107"></div>


**JavaScript:**

	// Init - Google Map Helper
	$("#google-map").each(function() {
        $(this).googleMap({address: $(this).data("address"), icon: 'images/map-icon.png', zoom:15,
            styles: [
                {
                    featureType: "all",
                    elementType: "all",
                    stylers: [
                        { hue: "#8B8C8E" },
                        { visibility: "on" },
                        { saturation: -100 },
                        { lightness: -20 }
                    ]
                }
            ]
        });
	});



## To Do:

* Setup "address" property to automatically attempt to pull from the "data-address" attribute by default, if it's undefined.

