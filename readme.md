# my hometown

## i built this 
because it reminds me of where i come from

 # Techology
- [Mapbox GL JS library][https://console.mapbox.com/] for styling and displaying maps and route lines, and adding camera behaviors (flyto animations).

  - ** Visual Studio  Code free IDE, with Live Server and Markdown All in One extensions.
**
- [GitHub pages][https://github.com/]  for publishing the app for free!

<img src="img/demo 2.0.gif"


## code snapshot



Here's a demo:



## Why did I build this?

When I decided to take a group of high school students on 5 bike rides in 5 days, I started wondering how I could communicate the ride itineraries to students (and families/guardians) in an accessible way. 

I set these goals for my product:

1. Families/guardians should **have detailed knowledge** of higher-risk student activities.
2. Students should **practice engaging** with visualized spatial data to **independently answer their own questions** about each day's ride location, duration, elevation, Points of Interest, or itinerary.

## Technology

To build this app, I used the following tools:

1. [Mapbox GL JS](https://docs.mapbox.com/mapbox-gl-js/guides) library, for styling and displaying maps and route lines, and adding camera behaviors (flyto animations).
2. [Visual Studio Code](https://code.visualstudio.com/download) free IDE, with [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) and [Markdown All in One](https://marketplace.visualstudio.com/items?itemName=yzhang.markdown-all-in-one) extensions.
3. [GitHub pages](https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site), for publishing the app for free!

## Feature Spotlight

One key feature I want to spotlight is the exaggerated terrain. 

If you look closely at the map, you might notice that the hills and mountains are very pronounced. That's because I exaggerated the apperance of topography by 250%. Here's how I did it:

Following [this example](https://docs.mapbox.com/mapbox-gl-js/example/add-terrain/), I first added [this](https://docs.mapbox.com/data/tilesets/reference/mapbox-terrain-dem-v1) Mapbox raster tileset `mapbox://mapbox.mapbox-terrain-dem-v1` to the map as a source. This tileset contains a Digital Elevation Model (DEM) encoded in the RGB values. So, by using `.setTerrain`, we can use the elevation values in the tileset to enable topographical extrusion – to make the map 3D!

So, why 250%? Well, what's the point of adding subtle (realistic) terrain, when my goal is to **prepare students to face some aggressive climbs**? _Those hills should look as mean as they feel._

Check it out:

![terrain eggageration code](img/terrain-code.png)

<img src="img/demo-3d-terrain.gif" alt="GIF demo showing 3d terrain" />

_Exaggerating the elevation profile makes the map more exciting._

## Contributions

Feel free to copy the code if you want it! Comments are welcome on [this blog post](https://domlet.github.io/posts/bike-the-bay/).
