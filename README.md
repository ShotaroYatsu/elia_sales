# Guideline on Building the Potential Customer List

# Introduction

<b>What is a GeoJSON file?</b>

A GeoJSON file is a collection of geographic data, whose file extension is .geojson. Each set of information within a GeoJSON file is called a "feature.". A feature forms a marker when the file is loaded onto a map. 

A single feature has 3 main items: "type", "properties", and "geometry" (do not worry about "type"). Within "properties" and "geometry", additional information can be specified within the brackets, and this is where you will fill in the information. 

A feature, or a set of information that describes one location, looks like the following: 

    {
      "type": "Feature",
      "properties": {
        "id": "",
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
          00.000000,
          00.000000
        ]
      }
    },

Use this code as a template when adding more information onto the file.

# Instructions

Copy the codes above, insert into the file, and fill in the blanks. 

<b>Where to insert the template</b>

When you open the geoJSON file, go to the bottom of the file. The last line is closed with a "}", second-to-last line is closed with "]" after two spaces, and third-to-last line is another "}" after four spaces. 

        }
      ]
    }

When inserting the template, first add a comma right after "}" on the third-to-last line. 

        },
      ]
    }

Then insert the code between this "}," and the "]".

        },
        {
          "type": "Feature",
          "properties": {
            "id": "",
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
              00.000000,
              00.000000
            ]
          }
        },
      ]
    }

When you finish inserting templates (i.e. the set of code presented under the Introduction section), make sure the bottom three lines look just like when you started working. There should be no comma in the last three lines.

<b>"Properties" section</b>

I (Shotaro) might re-assign "id" later, but for now, assign a value incrementally. For example, if the previous data had an ID of <b>"11"</b>, the next feature you add would have an ID number <b>"12"</b>.

If an information is not available, type in <b>"N/A"</b>. For "notes", just leave it as "" if there is nothing to write in. 

<b>"Geometry" section</b>
  
In order for the feature to appear correctly on a map, its coordinates need to be specified. Write them as follows:

    -99.725721,
    32.486768

where longitude is listed first, followed by latitude. Notice there is a comma after longitude - this comma must be there!

To convert street address into geographic coordinates, use the following website: 
http://www.latlong.net/convert-address-to-lat-long.html

<b>Examples</b>

For example, see the first four sets of features that is already uploaded onto the geoJSON file. 

# Common Mistakes

If the geoJSON file is written correctly, then clicking on it would load a map within the GitHub window, and show all the markers based on the features already included in the file. Clicking on the marker will also reveal information that was included in the file. 

If the map fails to load, it means that the syntax of the file is wrong somewhere. Very often, this is due to a missing comma somewhere or that a bracket is not closed properly. Commas and brackets let the computer know the distinction between one piece of information and another, so take care to ensure that commas are placed in the right places and brackets are closed properly.

