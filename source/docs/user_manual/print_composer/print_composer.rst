|updatedisclaimer|

.. _`label_printcomposer`:

**************
Print Composer
**************
.. index:: Create_Maps, Layout_Maps, Compose_Maps

The print composer provides layout and printing capabilities. It allows
you to add items such as the |qg| map canvas, text labels, images, legends, scalebars, basic
shapes, arrows, attribute tables and HTML frames. You can size, group, align and position each of these
items and adjust their properties to create your layout. The layout can then be printed
or exported to image formats, Postscript, PDF or to SVG. You can save the layout as a template and load it again
in another session. Finally, generating several maps based on a template can be done by taking advantage of the print composer's atlas generation ability.
A list of all tools available in the print composer is shown in table_composer_1_:

.. index::
   single: print_composer;tools

.. _table_composer_1:

+--------------------------+---------------------------------------+----------------------------+------------------------------------------+
| Icon                     | Purpose                               | Icon                       | Purpose                                  |
+==========================+=======================================+============================+==========================================+
+--------------------------+---------------------------------------+----------------------------+------------------------------------------+
| |mActionFileSave|        | Save Project                          | |mActionNewComposer|       | New Composer                             |
+--------------------------+---------------------------------------+----------------------------+------------------------------------------+
| |mActionDupComposer|     | Duplicate Composer                    | |mActionComposerManager|   | Composer Manager                         |
+--------------------------+---------------------------------------+----------------------------+------------------------------------------+
| |mActionFileOpen|        | Load from template                    | |mActionFileSaveAs|        | Save as template                         |
+--------------------------+---------------------------------------+----------------------------+------------------------------------------+
| |mActionSaveMapAsImage|  | Export to an image                    | |mActionSaveAsPDF|         | Export to PDF                            |
+--------------------------+---------------------------------------+----------------------------+------------------------------------------+
| |mActionSaveAsSVG|       | Export to SVG                         | |mActionFilePrint|         | Print or export as Postscript            |
+--------------------------+---------------------------------------+----------------------------+------------------------------------------+
| |mActionZoomFullExtent|  | Zoom to full extent                   | |mActionZoomIn|            | Zoom in                                  |
+--------------------------+---------------------------------------+----------------------------+------------------------------------------+
| |mActionZoomOut|         | Zoom out                              | |mActionDraw|              | Refresh view                             |
+--------------------------+---------------------------------------+----------------------------+------------------------------------------+
| |mActionUndo|            | Revert last change                    | |mActionRedo|              | Restore last change                      |
+--------------------------+---------------------------------------+----------------------------+------------------------------------------+
| |mActionAddMap|          | Add new map from |qg| map canvas      | |mActionAddImage|          | Add an image item                        |
+--------------------------+---------------------------------------+----------------------------+------------------------------------------+
| |mActionLabel|           | Add a label item                      | |mActionAddLegend|         | Add a legend item                        |
+--------------------------+---------------------------------------+----------------------------+------------------------------------------+
| |mActionScaleBar|        | Add a scalebar                        | |mActionAddBasicShape|     | Draw a basic shape                       |
+--------------------------+---------------------------------------+----------------------------+------------------------------------------+
| |mActionAddArrow|        | Draw an arrow                         | |mActionOpenTable|         | Add an attribute table                   |
+--------------------------+---------------------------------------+----------------------------+------------------------------------------+
| |mActionAddHtml|         | Add a HTML Frame                      |                            |                                          |
+--------------------------+---------------------------------------+----------------------------+------------------------------------------+
| |mActionSelectPan|       | Select/move items in print composition| |mActionMoveItemContent|   | Move content within an item              |
+--------------------------+---------------------------------------+----------------------------+------------------------------------------+
| |mActionGroupItems|      | Group items                           | |mActionUngroupItems|      | Ungroup items                            |
+--------------------------+---------------------------------------+----------------------------+------------------------------------------+
| |mActionRaiseItems|      | Raise selected items                  | |mActionLowerItems|        | Lower selected items                     |
+--------------------------+---------------------------------------+----------------------------+------------------------------------------+
| |mActionMoveItemsToTop|  | Move selected items to top            | |mActionMoveItemsToBottom| | Move selected items to bottom            |
+--------------------------+---------------------------------------+----------------------------+------------------------------------------+
| |mActionAlignLeft|       | Align selected items left             | |mActionAlignRight|        | Align selected items right               |
+--------------------------+---------------------------------------+----------------------------+------------------------------------------+
| |mActionAlignHCenter|    | Align selected items center           | |mActionAlignVCenter|      | Align selected items center vertical     |
+--------------------------+---------------------------------------+----------------------------+------------------------------------------+
| |mActionAlignTop|        | Align selected items top              | |mActionAlignBottom|       | Align selected items bottom              |
+--------------------------+---------------------------------------+----------------------------+------------------------------------------+

Table Composer 1: Print Composer Tools

All print composer tools are available in the menubar and as icons in the toolbar. The
toolbar can be switched off and on using the right mouse button over the toolbar.

.. index::
   single:Composer_Template
.. index::
   single:Map_Template

First steps
===========

Open a new Print Composer Template
----------------------------------

Before you start to work with the print composer, you need to load some raster
and vector layers in the |qg| map canvas and modify their properties to suit your
needs. After everything is rendered and symbolized to your liking,
click the |mActionNewComposer| :sup:`New Print Composer` icon in the toolbar or
choose :menuselection:`File --> New Print Composer`. You will be prompted to
choose a title for the new composition. Enter a descriptive title which you can use
to identify this composition.

Using Print Composer
--------------------

Initially, opening the print composer provides you with a blank canvas to which you can add
the current |qg| map canvas, text labels, images, legends, scalebars, basic
shapes, arrows, attribute tables and HTML frames. Figure_composer_1_ shows the
default view of the print composer before any elements are added.

.. _Figure_composer_1:

.. only:: html

   **Figure Composer 1:**

.. figure:: /static/user_manual/print_composer/print_composer_blank.png
   :align: center
   :width: 30em

   Print Composer |nix|

The print composer window contains four panels:

* The :guilabel:`Composition` panel allows you to set general composition properties, such as 
  paper size and number of pages, orientation and background style. Various export related settings can also be set in this tab.
* The :guilabel:`Item properties` panel displays the properties for the selected
  item. First select the |mActionSelectPan| :sup:`Select/Move item` tool and click on
  an item on the canvas to select it. Then click the
  :guilabel:`Item properties` tab and customize the settings for the selected
  item.
* The :guilabel:`Command history` panel displays a list of all changes made
  to the print composer layout. Clicking any position in this list will revert the 
  composition to an earlier state.
* The :guilabel:`Atlas generation` panel allows you to enable the generation of an
  atlas for the current composer and customise its behaviour.

You can add multiple items to the composer. Each item can be customised individually, and in the case of map items,
you can specify their individual extent and scale.

If you want to remove any items from the composition, just select the items then press the
:kbd:`Delete` or the :kbd:`Backspace` key.


Navigation tools
----------------

Zooming in and out
^^^^^^^^^^^^^^^^^^

Compositions in QGIS can be navigated in many different ways. You can click any of the four
zoom icons in the main toolbar to zoom in or out of the composition:

* |mActionZoomFullExtent| :sup:`Zoom full` - sets the zoom so that the entire composition is visible (:kbd:`Ctrl + 0`)
* |mActionZoomIn| :sup:`Zoom in` (:kbd:`Ctrl + +`)
* |mActionZoomOut| :sup:`Zoom out` (:kbd:`Ctrl + -`)
* :sup:`Zoom to 100%` - zooms to the approximate actual size of composition (:kbd:`Ctrl + 1`)

You can also zoom into or out of the composition by scrolling your mouse wheel. Holding the
:kbd:`Ctrl` key while scrolling zooms in or out by a finer amount.

There's also a :sup:`Zoom` tool, which allows you to click and drag to draw a rectangular
region on your composition to zoom into. Hold :kbd:`Shift` while using the Zoom tool to switch
to zoom out mode. You can switch to the Zoom tool mode at any time by holding :kbd:`Ctrl +
Space` on the keyboard.

Lastly, the status bar shows you your current zoom level. You can enter a precise zoom level
into the zoom combo box, or jump directly to one of several predefined zoom levels by selecting
it from the list.

Panning around
^^^^^^^^^^^^^^

Similarly, QGIS offer many shortcuts for moving around your composition. These include:

* Using the scrollbars to pan the view horizontally or vertically.
* Switch to the dedicated :sup:`Pan` tool. The mouse cursor changes to a hand icon, and you can click and drag to move the composition around.
* Pressing and holding the :kbd:`Space` key, or pressing and holding the mouse scroll wheel, temporarily switches to the pan mode at any time.

Composition tab --- General composition setup
---------------------------------------------

Within the :guilabel:`Composition` tab you can define the global settings of your composition. The composition tab is
split into a number of sections:

Paper and Quality
^^^^^^^^^^^^^^^^^

The :guilabel:`Paper and quality` group contains settings relating to the composition page and export options:

* You can choose one of the :guilabel:`Presets` sizes for your page, or enter a custom page :guilabel:`width` and :guilabel:`height` The :guilabel:`Units` combo allows you to choose the between setting page size in mm or inches.
* Compositions can now be created which span multiple pages. For instance, the first page could show a map canvas and the second page could show the attribute table associated to a layer and other information about the map. The number of pages is specified by setting the :guilabel:`Number of pages` control to the desired value.
* The page :guilabel:`Orientation` control allows you to switch between landscape and portrait page orientation.
* QGIS allows you to modify the style of the page background. Clicking the :guilabel:`Page background` button will show the standard QGIS symbol dialog, allowing you to use any of the available polygon styling modes for your page. You can even set the page background to be controlled by data defined settings, so that it can change with the each atlas page!
* The :guilabel:`Exported resolution` control lets you set the resolution for exported compositions
* Checking the |checkbox| :guilabel:`Print as raster` box will rasterise the composition before printing or exporting as Postscript or PDF. This may be required when the composition contains advanced visual effects such as blend modes or layer transparencies.
* Selecting the |checkbox| :guilabel:`World file on` option and selecting a map causes QGIS to create a world file alongside any exported compositions. This option is useful if you require georeferenced outputs from your compositions.

Grids and guides
^^^^^^^^^^^^^^^^

The :guilabel:`Grid` group is home to settings which allow you to fine-tune the behaviour of a visual alignment grid which can be drawn over your composition. The grid can be toggled by selecting :menuselection:`View --> Show Grid`, and you can toggle whether or not items should be snapped to the grid by choosing :menuselection:`View --> Snap to Grid`. Settings available for tweaking the grid are:

* :guilabel:`Spacing` - sets the interval which seperates each grid line.
* :guilabel:`Grid offset` - allows you to shift the grid lines by a set amount in the :guilabel:`x` and :guilabel:`y` axis.
* :guilabel:`Tolerance` - controls how close an item must be to the grid line before it is snapped to the line.

Additionally, the :guilabel:`Snap to alignments` group allows you to set the tolerance for items to snap to automatic guide lines.


Composer item general options
-----------------------------

All composer items types have a number of common properties you can tweak, including the item size and position. These properties are located at the bottom of the :guilabel:`Item Properties` tab, and include position, size and rotation, frame and background controls, item ID and rendering options (See figure_composer_2_).

.. _Figure_composer_2:

.. only:: html

   **Figure Composer 2:**

.. figure:: /static/user_manual/print_composer/print_composer_common_properties.png
   :align: center
   :width: 20em

   Common item properties |nix|

.. _Frame_Dialog:

* The :guilabel:`Position and size` group contains controls for defining the size and position of the frame that contains the item. You can also choose a :guilabel:`Reference point` at which the :guilabel:`X` and :guilabel:`Y` coordinates apply.
* The :guilabel:`Rotation` group allows you to set a rotation for the item. Rotation is specified in degrees in a clockwise direction.
* The |checkbox| :guilabel:`Frame` checkbox shows or hides the frame around the label.
  Click on the **[Color]** button to set the frame color. The **[Thickness]** control allows you to specify how thick the frame around the item should be drawn.
* The |checkbox| :guilabel:`Background` checkbox controls whether the item should have a background. Clearing this checkbox will cause the item to have a totally transparent background, so that items behind it or the page background color will show through. Click on the **[Color...]** button to display a dialog allowing you to choose a color for the item's background. You can control how opaque the background should be by modifing the :guilabel:`Alpha channel` setting in the color dialog.
* Use the :guilabel:`Item ID` to set a unique name for a composer item. The ID is also used with QGIS server and other web clients. If you set an ID for an item (e.g. a map and a label) and then the web client can send properties to set a property (e.g. label text) for that specific item. The GetProjectSettings command will lists what items and which IDs are available in a layout. The :guilabel:`Item ID` group also displays a unique, read only :guilabel:`Uuid` for each item, which can be used when automating composer tasks via the QGIS API.
* Lastly, the :guilabel:`Rendering` group contains settings for the item's transparency and blending mode. See Rendering_Controls_ for more details.

.. _Rendering_Controls:

.. index:: Rendering_Controls

Rendering controls
^^^^^^^^^^^^^^^^^^

The print composer has support for advanced rendering effects for composer items. These options include:

.. _figure_composer_3:

.. only:: html

   **Figure Composer 3:**

.. figure:: /static/user_manual/print_composer/rendering_mode.png
   :align: center
   :width: 20 em

   Rendering mode |nix|

* :guilabel:`Transparency` |slider|: allows you to control how opaque the item is. Increasing the transparency slider will allow items from behind to show through. Transparency can be set either by dragging the slider or by manually entering an exact value into the accompanying spin box.
* :guilabel:`Blending mode`: allows you to control the exact appearance of the item by specifying how it is drawn onto the composition. The pixels of the overlaying and underlaying items are mixed through the settings described below:

    * Normal: This is the standard blend mode, which uses only the alpha channel of the top pixel to blend with the pixel beneath it.
    * Lighten: Uses the maximum value of each component from the foreground and background pixels. Be aware that the results tend to be jagged and harsh.
    * Screen: Light pixels from the source are painted over the destination, while dark pixels are not. This mode is most useful for mixing the texture of one item with another item. E.g, drawing watermarks over a map item.
    * Dodge: Dodge will brighten and saturate underlying pixels based on the lightness of the top pixel. Brighter top pixels cause the saturation and brightness of the underlying pixels to increase. This works best if the top pixels aren't too bright, otherwise the effect is too extreme.
    * Addition: This blend mode simply adds pixel values of one layer with the other. In case of values above 1 (in the case of RGB), white is displayed. This mode is suitable for highlighting features.
    * Darken: Creates a resultant pixel that retains the smallest components of the foreground and background pixels. Like the lighten mode, the results tend to be jagged and harsh.
    * Multiply: Multiplies the values for each pixel of the top item with the corresponding pixel for the bottom item. This results in a darker image, which can be useful for watermarking and other textured effects.
    * Burn: Darker colors in the top item causes the underlying items to darken. Can be used to tweak and colorise underlying items.
    * Overlay: Combines both the multiply and screen blending modes. In the resulting image light parts of the item become lighter and dark parts become darker.
    * Soft light: Very similar to overlay, but instead of using multiply/screen it uses color burn/dodge. This mode is intended to emulate shining a soft light onto an image.
    * Hard light: Hard light is very similar to the overlay mode. It is intended to emulate projecting a very intense light onto an image.
    * Difference: Difference subtracts either the top pixel from the bottom pixel, or the other way round, such that the result is always a positive value.
    * Subtract: This blend mode simply subtracts pixel values of one item from the other. In case of negative values, black is displayed.


Moving and selecting items

 After you found the right place
for an element, you can lock the element position within the print composer
canvas. Select the map element and click on the right mouse button to |mIconLock|
:sup:`Lock` the element position and again to unlock the element. 

Composer Items
==============

Adding a map to the composition
-------------------------------

Click on the |mActionAddMap| :sup:`Add new map` toolbar button in the print
composer toolbar then click and drag a rectangle on the canvas to add the current |qg| map canvas to your composition. Properties for the map can be adjusted through the :guilabel:`Item properties` tab. 

Map items support three different display modes: Rectangle, Cache and Render. The display mode is set in the :guilabel:`Main properties` group under the :guilabel:`Item properties` tab. The display modes are:

* **Rectangle**. No map will be displayed in the item, just the frame, background and placeholder text. This is the fastest display mode, and is useful when you are making a large number of edits to the composition.
* **Cache** renders the map in the current screen resolution. Zooming in or out of the composer window will cause a lower resolution preview to be shown for the map. Additionally, changes you make in the map canvas are not shown unless you press the :guilabel:`Update preview` button. You can also update all the map items in the composition simultaenously by pressing the |mActionDraw| :sup:`Refresh view` toolbar button.
* **Render** indicates that the map item is a live preview of the canvas. Changes made to the map canvas are immediately shown in the composition, and the map is redrawn when the composer zoom changes. This is the slowest display mode since the map item is frequently redrawn.

**Cache** is default display mode for newly added map items, and is a good trade-off between speed and visual appearance.

You can resize a map item by clicking on the |mActionSelectPan|
:sup:`Select/Move item` tool, selecting the map item, and the dragging one of the
blue handles in the corners of the map.

To move the map content within the item first select the map item using the |mActionSelectPan|:sup:`Select/Move item` tool. Then, click the
|mActionMoveItemContent| :sup:`Move item content` toolbar ion and click and drag within the map item to pan the contents of the map. When the :guilabel:`Move item content` tool is active, scrolling the mouse wheel will zoom in or out of the map.

Main map properties
^^^^^^^^^^^^^^^^^^^

The :guilabel:`Main properties` group in the map :guilabel:`Item properties` tab contains the following settings (see figure_composer_4_):

.. _Figure_composer_4:

.. only:: html

   **Figure Composer 4:**

.. figure:: /static/user_manual/print_composer/print_composer_map1.png
   :align: center
   :width: 20em

   Map Item properties Tab |nix|

* The **Preview** area allows you to choose the display modes 'Rectangle', 'Cache'
  and 'Render', as described earlier. If changes are made to the |qg| map canvas, such as changing vector or raster layer properties, you can update the map item by clicking the **[Update preview]** button. Alternatively, the |mActionDraw| :sup:`Refresh view` toolbar button updates the preview for all maps on the composition.
* The :guilabel:`Scale` |selectnumber| control sets the map scale.
* :guilabel:`Map Rotation` |selectnumber| allows you to rotate the map within the map item's rectangular bounds. The angle is set clockwise in degrees. Altering the :guilabel:`Map Rotation` allows you to have maps in your composition which are not north-upwards. (Note: coordinate frames can only be added to the map with the default rotation of 0 degrees).
* The |checkbox| :guilabel:`Draw map canvas items` checkbox controls whether annotations that are placed on the map canvas in the main |qg| window are shown in the map item.
* You can choose to lock the layers shown on a map item. Check the |checkbox| :guilabel:`Lock layers for map item`. Any layer that is added or hidden in the main |qg| window after this checkbox is ticked will not appear or be hidden in the composer map item. This setting only affects visibility of layers - style and label changes to a locked layer will still appear in the map item.

Extents
^^^^^^^

The :guilabel:`Extents` group in map item's properties allows exact setting for the map's extent (see Figure figure_composer_5_). You can specify an extent for the map by setting the X and Y min/max values. Alternatively, clicking the **[Set to map canvas extent]** button will automatically set the map's extent to the current extent of the |qg| map canvas.

.. _Figure_composer_5:

.. only:: html

   **Figure Composer 5:**

.. figure:: /static/user_manual/print_composer/print_composer_map2.png
   :align: center
   :width: 20em

   Map Extents Dialog |nix|

.. index::
   single: Grid;Map_Grid

Controlled by atlas
^^^^^^^^^^^^^^^^^^^

In an atlas composition the extent of a map can be set by a feature in a vector layer (see the Atlas Generation section). If the map item should be controlled by the atlas features, check the |checkbox| :guilabel:`Controlled by atlas` checkbox. Two methods are available for atlas controlled maps:

* :guilabel:`Margin around feature` will automatically set the map item's extent to match the bounding box of the current atlas feature. The accompanying spinbox allows you to set an extra margin which is added to the size of the feature's bounding box. This setting is only available for polygon or line atlas coverage layers.
* :guilabel:`Fixed scale` will recenter the map on the current atlas feature without changing its scale.

Grid
^^^^

Checking the checkbox| :guilabel:`Show grid` option allows you to overlay a grid on the map. Settings are available for controlling the grid line positions, frame style and coordinate display (see Figure_composer_6_):

.. _Figure_composer_6:

.. only:: html

   **Figure Composer 6:**

.. figure:: /static/user_manual/print_composer/print_composer_map3.png
   :align: center
   :width: 20em

   Map Grid Dialog |nix|

* :guilabel:`Grid type` can be either Solid or Cross. Changing this setting affects how the grid is drawn over the map. The default solid option draws lines over the entire map item, whereas the cross option draws a small cross only where grid lines intersect.
* The :guilabel:`Interval` and :guilabel:`Offset` controls define how often grid lines are placed, and whether they should be offset by a set amount.
* :guilabel:`Cross width` sets the size of the grid cross shape. This setting is only applicable if the :guilabel:`Grid type` is set to Cross.
* Pressing the :guilabel:`Line style` button allows you to set the symbology for the grid lines, including the line color and thickness.
* The :guilabel:`Blend mode` allows you to set the blending mode for drawing the grid. See Rendering_Mode_ for more details on this setting.

Grids on a map item can also have an optional grid frame. Frame properties are specified under the :guilabel:`Grid frame` group, and include:

* :guilabel:`Frame style` controls the style of the grid frame. Currently only zebra style frames are supported.
* :guilabel:`Frame size` specifies how wide the grid frame should be drawn.
* :guilabel:`Frame line thickness` sets the thickness for lines within the grid frame
* :guilabel:`Frame line color` and :guilabel:`Frame fill colors` allow you to customise the colors used to draw the grid frame.

Lastly, map grids can be annotated with the grid coordinates. Checking the |checkbox| :guilabel:`Draw coordinates` checkbox switches on display of these annotations. Options are available for setting:

* :guilabel:`Format` controls whether coordinates should be displayed using decimal, degrees and minutes, or degrees, minutes and seconds format
* The position and direction of coordinates can be set individually for the left, right, top and bottom coordinates. The annotations can be drawn inside or outside the map frame, or disabled. Annotation direction can be either horizontal or vertical. 
* The font can be set by clicking the :guilabel:`Font` button, and it's color set by clicking :guilabel:`Font color`.
* :guilabel:`Distance to map frame` controls how seperation between the grid annotation and the outside of the map frame.
* :guilabel:`Coordinate precision` sets how many decimal places should be shown for grid coordinates.

Overview
^^^^^^^^

If the composition has more than one map, you can choose to use a map item to show the extents of a second map. The :guilabel:`Overview` group in the map :guilabel:`Item properties` tab allows to customize the appearance of the overview frame (see Figure_composer_7_).

.. _Figure_composer_7:

.. only:: html

   **Figure Composer 7:**

.. figure:: /static/user_manual/print_composer/print_composer_map4.png
   :align: center
   :width: 20em

   Map Overview Dialog |nix|

* The :guilabel:`Overview frame` combo box shows all available map items in the composition. Select a map item in this combo box to draw its extent within the current map item.
* :guilabel:`Overview Style` allows control of the overview frame color and style. See Section vector_style_manager .
* The :guilabel:`Overview blending mode` specifies how the overview frame should be rendered onto to map. See Rendering_Mode_ for details.
* If checked, the |checkbox| :guilabel:`Invert overview` reverses the overview, so that areas outside of the overview frame's extents are shaded.
* The |checkbox| :guilabel:`Center on overview` checkbox specifies that the map item should be centered on the overview frame. This setting is useful for atlas compositions, where the map item should always follow a second map item's extents.

Adding a label to the composition
---------------------------------

To add a label, click the |mActionLabel| :sup:`Add new label` toolbar icon, then click within your composition at the position where you'd like to place the new label. Label text and properties are customised within the label's :guilabel:`Item properties` tab. The following settings can be controlled:

.. _Figure_composer_8:

.. only:: html

   **Figure Composer 8:**

.. figure:: /static/user_manual/print_composer/print_composer_label1.png
   :align: center
   :width: 20em

   Label Item properties Tab |nix|

Main properties
^^^^^^^^^^^^^^^

The :guilabel:`Main properties` group in a label's item properties provides the
following options (see Figure_composer_9_):

.. _Figure_composer_9:

.. only:: html

   **Figure Composer 9:**

.. figure:: /static/user_manual/print_composer/print_composer_label2.png
   :align: center
   :width: 20em

   Label Main properties Dialog |nix|

* The text box directly below the :guilabel:`Main properties` group shows the current text for the label. Enter text (or html) in this box to change the label's current text.
* Labels can be rendered using html code: check the |checkbox| :guilabel:`Render as HTML` checkbox to enable this option. Entering html code for a label allows finer control of how the label is displayed, and can be used to enter rich text content such as formatting or tables within a label.
* You can also insert an expression into a label. Click on the **[Insert an expression]** to open a new expression dialog. Build an expression by clicking the functions available in the left side of the panel. On the right side of the `Insert an expression dialog` help for the currently selected function is displayed. The geometry functions and records functions are particularly useful for labels which are part of atlas compositions. On the bottom of the expression dialog a preview of the evaluated expression is shown.
* Define the label's font and font color by clicking on the **[Font]** and **[Font color...]** buttons

Alignment and Display
^^^^^^^^^^^^^^^^^^^^^

The :guilabel:`Alignment` and :guilabel:`Display` groups in the label's item properties tab allows for further customisation of labels (see Figure_composer_10_):

.. _Figure_composer_10:

.. only:: html

   **Figure Composer 10:**

.. figure:: /static/user_manual/print_composer/print_composer_label3.png
   :align: center
   :width: 20em

   Label Alignment and Display Dialogs |nix|

* You can define the horizontal and vertical alignment for the label's text in the :guilabel:`Alignment` group
* In the **Display** group you can define a margin in mm. This setting controls how much spacing should be left between the label's frame and the displayed text.

Adding an image to the composition
----------------------------------

To add an image, click the |mActionAddImage| :sup:`Add image` icon, place the element
with the left mouse button on the print composer canvas and position and customize
its appearance in the image :guilabel:`Item Properties` tab.

.. index::
   single:Picture_database
.. index::
   single:Rotated_North_Arrow

The image :guilabel:`Item Properties` tab provides following functionalities (see figure_composer_11_):

.. _Figure_composer_11:

.. only:: html

   **Figure Composer 11:**

.. figure:: /static/user_manual/print_composer/print_composer_image1.png
   :align: center
   :width: 15em

   Image Item properties Tab |nix|

Main properties, Search directories and Rotation
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

The :guilabel:`Main properties` and :guilabel:`Search directories` dialogs of the Image :guilabel:`Item Properties` tab provide
following functionalities (see Figure_composer_12_):

.. _Figure_composer_12:

.. only:: html

   **Figure Composer 12:**

.. figure:: /static/user_manual/print_composer/print_composer_image2.png
   :align: center
   :width: 20em

   Image Main properties, Search directories and Rotation Dialogs |nix|

* The **Main properties** dialog shows the current image that is displayed in the image item.
  Click on the **[...]** button to select a file on your computer.
* This dialog shows all pictures stored in the selected directories.
* The **Search directories** area allows to add and remove directories with
  images in SVG format to the picture database.
* Image can be rotate, with the :guilabel:`Rotation` |selectnumber| field.
* Activating the |checkbox| :guilabel:`Sync with
  map` checkbox synchronizes the rotation of a picture in the |qg| map canvas
  (i.e. a rotated north arrow) with the appropriate print composer image.

.. index::
   single:Map_Legend

Adding a Legend item to the Print Composer
------------------------------------------

To add a map legend, click the |mActionAddLegend| :sup:`Add new legend` icon,
place the element with the left mouse button on the print composer canvas and
position and customize their appearance in the legend :guilabel:`Item Properties`
tab.

The :guilabel:`Item properties` of a legend item tab provides following
functionalities (see figure_composer_14_):

.. _Figure_composer_13:

.. only:: html

   **Figure Composer 13:**

.. figure:: /static/user_manual/print_composer/print_composer_legend1.png
   :align: center
   :width: 20em

   Legend Item properties Tab |nix|

Main properties
^^^^^^^^^^^^^^^

The :guilabel:`Main properties` dialog of the legend :guilabel:`Item Properties` tab
provides following functionalities (see figure_composer_14_):

.. _Figure_composer_14:

.. only:: html

   **Figure Composer 14:**

.. figure:: /static/user_manual/print_composer/print_composer_legend2.png
   :align: center
   :width: 20em

   Legend Main properties Dialog |nix|

* Here you can adapt the legend title.
* Choose which :guilabel:`Map` item the current legend will refer to in the select list.
* Since |qg| 1.8, you can wrap the text of the legend title to a given character.

Legend items
^^^^^^^^^^^^

The :guilabel:`Legend items` dialog of the legend :guilabel:`Item Properties` tab
provides following functionalities (see figure_composer_15_):

.. _Figure_composer_15:

.. only:: html

   **Figure Composer 15:**

.. figure:: /static/user_manual/print_composer/print_composer_legend3.png
   :align: center
   :width: 20em

   Legend Legend Items Dialog |nix|

* The legend items window lists all legend items and allows to change item order,
  group layers, remove and restore items of the list, edit layer names. After changing the
  symbology in the |qg| main window you can click on **[Update]** to adapt the
  changes in the legend element of the print composer. The item order can be
  changed using the **[Up]** and **[Down]** buttons or with 'drag and drop'
  functionality.
* The feature count for each vector layer can be shown by enable the **[Sigma]** button.
* Legend can be updated automatically, |checkbox| :guilabel:`Auto-update` is checked.

Fonts, Columns, Symbol and Spacing
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

The :guilabel:`Fonts`, :guilabel:`Columns`, :guilabel:`Symbol` and :guilabel:`Spacing` dialogs of the legend :guilabel:`Item Properties` tab
provide following functionalities (see figure_composer_16_):

.. _Figure_composer_16:

.. only:: html

   **Figure Composer 16:**

.. figure:: /static/user_manual/print_composer/print_composer_legend4.png
   :align: center
   :width: 20em

   Legend Fonts, Columns, Symbol and Spacing Dialogs |nix|

* You can change the font of the legend title, group, subgroup and item (layer) in the legend item. Click on a category button to open a
  **Select font** dialog.
* All those items will get the same **Color**
* Legend items can be arranged in several columns. Select the correct value in the :guilabel:`Count` |selectnumber| field.
* The |checkbox| :guilabel:`Equal columns widths` sets how legend columns should be adjusted.
* The |checkbox| :guilabel:`Split layers` option allows a categorized or a graduated layer legend to be divided upon columns.
* You can change width and height of the legend symbol in this dialog.
* Spacing aroung title, group, subgroup, symbol, icon label, box space or column space can be customized throught that dialog.

.. index::
   single: Scalebar; Map_Scalebar

Adding a Scalebar item to the Print Composer
--------------------------------------------

To add a scalebar, click the |mActionScaleBar| :sup:`Add new scalebar` icon, place
the element with the left mouse button on the print composer canvas and position
and customize their appearance in the scalebar :guilabel:`Item Properties` tab.

The :guilabel:`Item properties` of a scalebar item tab provides following
functionalities (see figure_composer_17_):

.. _Figure_composer_17:

.. only:: html

   **Figure Composer 17:**

.. figure:: /static/user_manual/print_composer/print_composer_scalebar1.png
   :align: center
   :width: 20em

   Scalebar Item properties Tab |nix|

Main properties
^^^^^^^^^^^^^^^

The :guilabel:`Main properties` dialog of the scalebar :guilabel:`Item Properties` tab
provides following functionalities (see figure_composer_18_):

.. _Figure_composer_18:

.. only:: html

   **Figure Composer 18:**

.. figure:: /static/user_manual/print_composer/print_composer_scalebar2.png
   :align: center
   :width: 20em

   Scalebar Main properties Dialog |nix|

* First choose the map the scalebar will be attached to.
* then choose the style of your scalebar. Six styles are available :
* **Single box** and **Double box** styles which contain one or two lines of boxes alternating colors,
* **Middle**, **Up** or **Down** line ticks,
* **Numeric** : the scale ratio is printed, i.e. 1:50000.

Units and Segments
^^^^^^^^^^^^^^^^^^

The :guilabel:`Units` and :guilabel:`Segments` dialogs of the scalebar :guilabel:`Item Properties` tab
provide following functionalities (see figure_composer_19_):

.. _Figure_composer_19:

.. only:: html

   **Figure Composer 19:**

.. figure:: /static/user_manual/print_composer/print_composer_scalebar3.png
   :align: center
   :width: 20em

   Scalebar Units and Segments Dialogs |nix|

In those two dialogs, you can set how the scalebar will be represented.

* Select the map units used. There's three possible choices : **Map Units** is the automated unit
  selection, **Meters** or **Feet** force unit conversions.
* The :guilabel:`Label` field defines the text used to describe the unit of the scalebar.
* The :guilabel:`Map units per bar unit` allows to fix the ratio between a map unit and its representation in the scalebar.
* You can define how many :guilabel:`Segments` will be drawn on the left and on the right side of the scalebar,
  and how long will be each segment (:guilabel:`Size` field). :guilabel:`Height` can also be defined.

Display, Fonts and colors
^^^^^^^^^^^^^^^^^^^^^^^^^

The :guilabel:`Display` and :guilabel:`Fonts and colors` dialogs of the scalebar :guilabel:`Item Properties` tab provide following functionalities (see figure_composer_20_):

.. _Figure_composer_20:

.. only:: html

   **Figure Composer 20:**

.. figure:: /static/user_manual/print_composer/print_composer_scalebar4.png
   :align: center
   :width: 20em

   Scalebar Display, Fonts and colors Dialogs |nix|

* You can define how the scalebar will be displayed in its frame. Adjust the :guilabel:`Box margin` between text and frame borders,
  :guilabel:`Labels margin` between text and scalebar drawing and the :guilabel:`Line width` of the scalebar drawing.
* The :guilabel:`Alignment` in the :guilabel:`Display` dialog only applies to :guilabel:`Numeric` styled scalebars and puts text on the
  left, middle or right side of the frame.

Adding a Basic shape or Arrow item to the Print Composer
--------------------------------------------------------

It is possible to add basic shapes (Ellipse, Rectangle, Triangle) and arrows
to the print composer canvas : click the |mActionAddBasicShape| :sup:`Add basic shape` icon or the
|mActionAddArrow| :sup:`Add Arrow` icon, place the element with the left mouse button on the print composer canvas and position
and customize their appearance in the :guilabel:`Item Properties` tab.

The :guilabel:`Shape` Item properties tab allows to draw an ellipse, rectangle, or triangle
in the print composer canvas. You can define its outline and fill color, the
outline width and a clockwise rotation.

.. _figure_composer_21:

.. only:: html

   **Figure Composer 21:**

.. figure:: /static/user_manual/print_composer/print_composer_shape.png
   :align: center
   :width: 20em

   Shape Item properties Tab |nix|

The :guilabel:`Arrow` Item properties tab allows to draw an arrow in the print composer canvas.
You can define color, outline and arrow width and it is possible to use a default
marker and no marker and a SVG marker. For the SVG marker you can additionally
add a SVG start and end marker from a directory on your computer.

.. _figure_composer_22:

.. only:: html

   **Figure Composer 22:**

.. figure:: /static/user_manual/print_composer/print_composer_arrow.png
   :align: center
   :width: 20em

   Arrow Item properties Tab |nix|

Main properties
^^^^^^^^^^^^^^^

* For Basic shapes, this dialog allows you to choose a **Ellipse**, **Rectangle** or **Triangle** shape and its rotation.
* Unlike the other items, line style, line color and background color of a basic shape are adjusted with the Frame and Background dialog.
  No frame is drawn.
* For arrows, you can define here the line style : :guilabel:`Color`, :guilabel:`Line width` and :guilabel:`Arrow head width`.
* :guilabel:`Arrows markers` can be adjusted. If you want to set a SVG :guilabel:`Start marker` and/or :guilabel:`End marker`, browse to
  your SVG file by clicking on the **[...]** button after selecting :guilabel:`SVG` radio button.

.. note::
   Unlike other items, background color for a basic shape is the shape background and not the frame one.

.. index:: Attribute_Table

Add attribute table values to the Print Composer
------------------------------------------------

It is possible to add parts of a vector attribute table to the print composer
canvas : click the |mActionOpenTable| :sup:`Add attribute table` icon, place the element with the left mouse button on the print composer
canvas and position and customize their appearance in the :guilabel:`Item Properties` tab.

The :guilabel:`Item properties` of a attribute table item tab provides following
functionalities (see figure_composer_23_):

.. _Figure_composer_23:

.. only:: html

   **Figure Composer 23:**

.. figure:: /static/user_manual/print_composer/print_composer_attribute1.png
   :align: center
   :width: 20em

   Scalebar Item properties Tab |nix|

Main properties, Show grid and Fonts
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

The :guilabel:`Main properties`, :guilabel:`Show grid` and :guilabel:`Fonts` dialogs of the attribute table :guilabel:`Item Properties` tab
provide following functionalities (see figure_composer_24_):

.. _Figure_composer_24:

.. only:: html

   **Figure Composer 24:**

.. figure:: /static/user_manual/print_composer/print_composer_attribute2.png
   :align: center
   :width: 20em

   Attribute table Main properties, Show grid and Fonts Dialog |nix|

   .. _Figure_composer_25:

.. only:: html

   **Figure Composer 25:**

.. figure:: /static/user_manual/print_composer/print_composer_attribute3.png
   :align: center
   :width: 15em

   Attribute table Select attributes Dialog |nix|

* The :guilabel:`Table` dialog allows to select the vector layer and columns of the attribute table. Attribute columns can be sorted and you
  can define to show its values ascending or descending (see figure_composer_25_).
* You can choose to display only the attribute of features visibled on a map. Check |checkbox| :guilabel:`Show only visible features` and
  select the corresponding :guilabel:`Composer map` to filter.
* You can define the :guilabel:`Maximum number of rows` to be displayed and :guilabel:`margin` around text.
* Additionally you can define the grid characteristics of the table (:guilabel:`Stroke width` and :guilabel:`Color` of the grid) and the
  header and content font.

.. index:: HTML_Frame

Add a HTML frame to the Print Composer
--------------------------------------

It is possible to add a clickable frame, linked to an URL : click the |mActionAddHtml| :sup:`Add html frame` icon, place the element with
the left mouse button on the print composer canvas and position and customize their appearance in the :guilabel:`Item Properties` tab.

Main properties
^^^^^^^^^^^^^^^

The :guilabel:`Main properties` dialog of the HTML frame :guilabel:`Item Properties` tab
provides following functionalities (see figure_composer_26_):

.. _Figure_composer_26:

.. only:: html

   **Figure Composer 26:**

.. figure:: /static/user_manual/print_composer/print_composer_html.png
   :align: center
   :width: 20em

   HTML frame Item properties Tab |nix|

* Point the :guilabel:`URL` field to the URL or the HTML file you want to insert in the composer.
* You can adjust the rendering of that page with the :guilabel:`Resize mode`.
* **Use existing frames** constraints the page inside its first frame or in the frame created with the next settings.
* **Extent to next page** will create as many frames (and their pages) as necessary to render the height of the webpage. Each frame can be
  moved around on the layout. If you resize a frame, the webpage will be divided up upon the other frames. The last frame will be trimmed to
  fit the webpage.
* **Repeat on every page** will first repeat the upper left of the webpage on every page, in same sized frames.
* **Repeat until finished** will also create as many frames as the **Extend to next page** option, except All frames will have the same
  size.

.. index:: Elements_Alignment

Item alignment
==============

Raise or lower functionalities for elements are inside the |mActionRaiseItems|
:sup:`Raise selected items` pulldown menu. Choose an element on the print composer
canvas and select the matching functionality to raise or lower the selected
element compared to the other elements (see table_composer_1_).

.. _figure_composer_27:

.. only:: html

   **Figure Composer 27:**

.. figure:: /static/user_manual/print_composer/alignment_lines.png
   :align: center
   :width: 30 em

   Alignment helper lines in the Print Composer |nix|

There are several alignment functionalities available within the |mActionAlignLeft|
:sup:`Align selected items` pulldown menu (see table_composer_1_). To use an
alignment functionality , you first select some elements and then click on the
matching alignment icon. All selected will then be aligned within to their common
bounding box.
When moving items on the composer canvas, alignment helper lines appear when borders, centers or corners are aligned.

.. index:: Revert_Layout_Actions

Revert and Restore tools
------------------------

During the layout process it is possible to revert and restore changes. This can
be done with the revert and restore tools:

* |mActionUndo| :sup:`Revert last changes`
* |mActionRedo| :sup:`Restore last changes`

or by mouse click within the :guilabel:`Command history` tab (see figure_composer_28_).

.. _figure_composer_28:

.. only:: html

   **Figure Composer 28:**

.. figure:: /static/user_manual/print_composer/command_hist.png
   :align: center
   :width: 20 em

   Command history in the Print Composer |nix|

.. index:: Atlas_Generation

Atlas generation
================

The print composer includes generation functions that allow to create map books
in an automated way. The concept is to use a coverage layer, which contains
geometries and fields. For each geometry in the coverage layer, a new output
will be generated where the content of some canvas maps will be moved to
highlight the current geometry. Fields associated to this geometry can be used
within text labels.

There can only be one atlas map by print composer but this one can contain multiple pages.
Every pages will be generated  with each feature. To enable the generation
of an atlas and access generation parameters, refer to the `Atlas generation`
tab. This tab contains the following widgets (see Figure_composer_29_):

.. _figure_composer_29:

.. only:: html

   **Figure Composer 29:**

.. figure:: /static/user_manual/print_composer/print_composer_atlas.png
   :align: center
   :width: 15em

   Atlas generation tab |nix|

* A |checkbox| :guilabel:`Generate an atlas` enables or disables the atlas generation.
* A combobox :guilabel:`Composer map` |selectstring| that allows to choose
  which map item will be used as the atlas map, i.e. on which map geometries from
  the coverage layer will be iterated over and displayed.
* A combobox :guilabel:`Coverage layer` |selectstring| that allows to choose the
  (vector) layer containing the geometries on which to iterate over.
* An optional |checkbox| :guilabel:`Hidden coverage layer`, that if checked, will
  hide the coverage layer (but not the other ones) during the generation.
* An optional |checkbox| :guilabel:`Features sorting` that, if checked, allows to
  sort features of the coverage layer. The associated combobox allows to choose
  which column will be used as the sorting key. Sort order (either ascending or
  descending) is set by a two-state button that displays an up or a down arrow.
* An optional :guilabel:`Feature filtering` text area that allows to specify an
  expression for filtering features from the coverage layer. If the expression
  is not empty, only features that evaluate to ``True`` will be selected. The
  button on the right allows to display the expression builder.
* An input box :guilabel:`Scaling` that allows to select the amount
  of space added around each geometry within the allocated map. Its value is
  meaningful only when using the autoscaling mode.
* A |checkbox| :guilabel:`Fixed scale` that allows to toggle between auto-scale
  and fixed-scale mode. In fixed scale mode, the map will only be translated for
  each geometry to be centered. In auto-scale mode, the map's extents are computed
  in such a way that each geometry will appear in its whole.
* An :guilabel:`Output filename expression` textbox that is used to generate a
  filename for each geometry if needed. It is based on expressions. This field is
  meaningful only for rendering to multiple files.
* A |checkbox| :guilabel:`Single file export when possible` that allows to force
  the generation of a single file if this is possible by the chosen output format
  (PDF for instance). If this field is checked, the value of the
  :guilabel:`Output filename expression` field is meaningless.

In order to adapt labels to the feature the atlas plugin iterates over, use a label with this special notation
`[%expression using field_name%]`.
For example, with a city layer with fields CITY_NAME and ZIPCODE, you could insert this :

"`[% 'The area of ' || upper(CITY_NAME) || ',' || ZIPCODE || ' is ' format_number($area/1000000,2) || ' km2' %]`"

And that would result in the generated atlas as

"`The area of PARIS,75001 is 1.94 km2`".

Generation
----------

The atlas generation is done when the user asks for a print or an export. The behaviour of these functions will be slightly changed if an atlas map has been selected. For instance, when the user asks for an export to PDF, if an atlas map is defined, the user will be asked for a directory where to save all the generated PDF files (except if the |checkbox| :guilabel:`Single file export when possible` has been selected).

.. index::
   single:Printing; Export_Map

Creating Output
===============

Figure_composer_30_ shows the print composer with an example print layout
including each type of map element described in the sections above.

.. _figure_composer_30:

.. only:: html

   **Figure Composer 30:**

.. figure:: /static/user_manual/print_composer/print_composer_complete.png
   :align: center
   :width: 35 em

   Print Composer with map view, legend, image, scalebar, coordinates , text and HTML frame added |nix|

.. index:: Export_as_image, Export_as_PDF, Export_as_SVG

The print composer allows you to create several output formats and it is possible
to define the resolution (print quality) and paper size:

* The |mActionFilePrint| :sup:`Print` icon allows to print the layout to a
  connected printer or a Postscript file depending on installed printer drivers.
* The |mActionSaveMapAsImage| :sup:`Export as image` icon exports the composer
  canvas in several image formats such as PNG, BPM, TIF, JPG,...
* The |mActionSaveAsPDF| :sup:`Export as PDF` saves the defined print composer
  canvas directly as a PDF.
* The |mActionSaveAsSVG| :sup:`Export as SVG` icon saves the print composer canvas
  as a SVG (Scalable Vector Graphic).

.. note::

   Currently the SVG output is very basic. This is not a |qg| problem, but a
   problem of the underlaying Qt library. This will hopefully be sorted out in
   future versions.
   Export big raster can sometimes fail, even if there seems to be enough memory.
   This is also a problem of the underlaying Qt management of raster.

.. index:: Composer_Manager

Manage the Composer
===================

With the |mActionFileSaveAs| :sup:`Save as template` and |mActionFileOpen|
:sup:`Load from template` icons you can save the current state of a print composer
session as a  :file:`.qpt` template and load the template again in another session.

The  |mActionComposerManager| :sup:`Composer Manager` button in the |qg| toolbar
and in :menuselection:`Composer --> Composer Manager` allows to add a new composer
template, create a new composition based on a previously saved template or to manage 
already existing templates.

.. _figure_composer_31:

.. only:: html

   **Figure Composer 31:**

.. figure:: /static/user_manual/print_composer/print_composer_manager.png
   :align: center
   :width: 20 em

   The Print Composer Manager |nix|

By default, the composer manager searches for user templates in ~/.qgis2/composer_template.

The |mActionNewComposer| :sup:`New Composer` and |mActionDupComposer| :sup:`Duplicate Composer` 
buttons in the |qg| toolbar and in :menuselection:`Composer --> New Composer` and  
:menuselection:`Composer --> Duplicate Composer` allow to open a new composer dialog, or to 
duplicate an existing composition from a previously created one.

Finally you can save your print composition with the |mActionFileSave| :sup:`Save Project` button. 
This is the same feature as in the QGIS main window. All changes will be saved in a QGIS project 
file.  


