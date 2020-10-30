# Routing Plugin


## Installation

These softwares are needed to make the plugin works properly:

1. **KadasLocationSearch**, to enable name based location search. It is usually shipped with Kadas. Without this, you can still choose a location using GPS or click on the map.
2. **Valhalla**, to enable routing, reachability, and navigation functionality. It must be installed in the same machine. Read more about Valhalla [here](https://github.com/valhalla/valhalla).

Currently, the installation only available from this repository.

1. Obtaining the source code

    To get the source code, clone this repository:
	```
    git clone http://github.com/camptocamp/kadas-routing-plugin.git
    ```
    or download the source code using the [Github download link button](https://github.com/camptocamp/kadas-routing-plugin/archive/master.zip).

2. Installation

   To install this plugin on [Kadas Albireo 2](https://github.com/kadas-albireo/kadas-albireo2), extract the zip file from step 1, then copy the `kadasrouting` folder to the KADAS plugins folder located in your used folder. For example:
   ```
   C:\Users\fclementi\AppData\Roaming\Kadas\KadasMil\profiles\default\python\plugins
   ```

3. Enable the plugin

   To enable this plugin, open [Plugin Manager](settings.md#sec5) menu from Settings menu, and tick the checkbox on the Kadas Routing Plugin.

After the plugin has been activated, there will be some additional tool in the Kadas Albiero menu:

1. Routing
2. Navigation
3. Reachability
4. Data Catalogue
5. Day / Night


## Routing

Routing functionality can be accessed from Navigation menu.

<img src="../images/routing_plugin/navigation_tab_routing.png" />

Clicking the Routing button will open the Routing window like below.

<img src="../images/routing_plugin/routing_window.png" />

There are some number indicated in the image above, below are the explanation for each number:

1. **Layer selector** is used to select the output layer from the routing calculation. If there is already a layer, it will be overriden.
2. **Origin point selector** is used to select the origin point for routing calculation. The user can choose by typing a place name, and pop up will be shown up where user can choose based on his typing. The user can also click a location in the map by using the map tool (arrow button) or get the current GPS location (GPS button). A selected point is shown as a pin with an arrow inside it.
3. **Destination point selector** is used to select the destination for routing calculation. The workflow is same as the *origin point selector.* The selected point is shown as a grey pin with a flag inside it.
4. **Way point selector** is used to select a way point for routing calculation. The workflow is same as the *origin point selector*. A way point is shown as a grey pin with a circle inside it.
5. **Way point add button** is used to add the way point from *way point selector* to the list of way points. All selected way points are shown as a yellow circle.
6. **Selected way points** is used to show the list of way point that have been added by *way point add button*
7. **Clear button** is used to clear all selected origin point, destination point, and way points.
8. **Reverse button** is used to reverse the origin and destination point. It will also reverse the order of selected way points.
9. **Vehicle type selector** is used to choose the type of vehicle for the routing calculation.
10. **Route type selector** is used to choose what kind of route that want to be calculated. It can be shortest route or fastest route.
11. **Area to avoid selector** is used to select polygon that will be avoided during the route calculation. It can be created by drawing on the map canvas or from an external polygon layer.
12. **Calculate button** is used to start the routing calculation.
13. **Navigate button** is used to start the navigation based on the calculated route. This button is disabled until a route is calculated.
14. **Close button** is used to close the button

### Route calculation workflow

Here is an example for a route calculation from *Bern* to *Zurich* through *Luzern*. *Oftringen* is not yet added to selected way point.

<img src="../images/routing_plugin/routing_selection.png" />

Here is the result of the routing calculation above. Now, the navigation button is enabled. The result is shown as a blue line.

<img src="../images/routing_plugin/routing_result.png" />


## Navigation

## Reachability

## Data Catalogue

## Day / Night