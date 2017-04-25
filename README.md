# Introduction

<b>What is a GeoJSON file?</b>

A GeoJSON file is a collection of geographic data, whose file extension is .geojson. Each set of information within a GeoJSON file is called a "feature.". A feature forms a marker when the file is loaded onto a map. 

A single feature has 3 main items: "type", "properties", and "geometry." Within "properties" and "geometry", additional information can be specified within the brackets. It looks like the following: 

    {
      "type": "Feature",
      "properties": {
        "id": "1",
        "name": "",
        "URL": "",
        "street": "",
        "city": "",
        "state": "",
        "zip": "",
        "email": "",
        "phone": "",
        "indoor/outdoor": "",
        "produce type": "",
        "notes: ""
      },
      "geometry": {
        "type": "Point",
        "coordinates": [
          00.000000
          00.000000
        ]
      }
    },

# Instructions

Copy and paste the above code 

<b>"Properties" section</b>

I (Shotaro) might re-assign "id" later, but for now, assign a value incrementally. Meaning, if the previous data had an ID of <b>"204"</b>, the next feature you add would have an ID number <b>"205"</b>.

If an information is not available, type in <b>"N/A"</b>. You don't need to do this for "notes". 

<b>"Geometry" section</b>
  
In order for the feature to appear correctly on a map, its coordinates need to be specified. Write them as follows:

    -99.725721
    32.486768

where longitude is listed first, followed by latitude.

To convert street address into geographic coordinates, use the following website: 
http://www.latlong.net/convert-address-to-lat-long.html





For example, see the following:



