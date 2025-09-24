 name: gitartwork from a contribution graph
 on: 
   push:
 jobs:
   build:
     name: Make gitartwork SVG
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
       - uses: rutvikh-webmavens/gitartwork@v1
         with:
            # Use this username's contribution graph  
            user_name: RUTVIK
            # Text on contribution graph 
            text: JASINERI
       - uses: rutvikh-webmavens/simple-push-action@v1
