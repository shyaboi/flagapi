# Flag API
this is a flag API currently in beta

# Use Case
The main usage intention for this flag API is to simply have an endpoint for a  <img src="image.svg"> html.

The API endpoint can be use by any progrom that can work with images, SVGs, or JSON

# Use
You can use this API in the way you use most APIs, I will give some examples.

# cURL Usage
You can use this api with simple cURL requests.

to get the full code of a .svg file your cURL request should look like the example below;
```
curl https://flagapi.ngrok.io/api/usa/colorado
```
The output of the request will look something similar to the example below;
```
<?xml version="1.0" encoding="UTF-8" standalone="no"?>
<svg xmlns="http://www.w3.org/2000/svg" width="1800" height="1200">
<!-- Created per specification at http://www.50states.com/flag/coflag.htm by Robert Fleming -->
 <rect width="1800" height="1200" fill="#002868"/>
 <rect width="1800" height="400" y="400" fill="white"/>
 <!-- 76 + 180*sqrt(55)/36 ~= 113.1 -->
 <path d="M1130.81,750A400,400 0 1,1 1130.81,450L760,600Z" fill="#bf0a30"/>
 <circle cx="760" cy="600" r="200" fill="gold"/>
</svg>
```

### Download via cURL
if you want to download the file locally via cURL, your cURL request should look like the example below;
```
curl https://flagapi.ngrok.io/usa/region/colorado.svg -o coloradoflag.svg
```
The cURL will download the file in the current working directory, and give it the name following the "-o"
### cURL JSON
If you want to generate a JSON response to your cURL, cURL request should look like the example below;
```
curl https://flagapi.ngrok.io/api/usa/colorado
```
This will generate a JSON response similar to the example below;
```
flagInfo":[{"_id":"5f51ca2c7cf1026aa0a50f95","directLink":"https://flagapi.ngrok.io/usa/region/colorado.svg","quickLink":"colorado.svg","region":"colorado","country":"usa"}]
```

