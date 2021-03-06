.. _drawing_animation_levels:

Drawing Animation Levels
========================
In Toonz it is possible to draw Toonz vector levels (PLI format), Toonz raster levels (TLV format) and standard raster levels (TIF format) directly in the work area. Drawing tools can also be used for touch-up in cleaned up drawings, and any loaded raster images.

.. _drawing_in_toonz:

Drawing In Toonz
----------------
To draw an animation level, first you have to define its type, Toonz vector, Toonz raster or raster, and its settings like its name, the number of frames it is made of and the way its drawings are numbered.

Toonz vector levels are defined by drawing vector strokes; vectors and areas defined by vectors can be painted by using the styles available in the level palette. Toonz vector levels have unlimited size and resolution, as they are vector-based. They are saved as PLI files.

.. note:: Starting from Toonz Harlequin 6.4 ML, vector levels (PLI files) created with Toonz are not compatible with previous versions of the software.

Toonz raster levels are defined by drawing bitmap lines; lines and areas defined by lines can be painted by using the styles available in the level palette. Toonz raster levels have a limited size and resolution, defined when they are created. They are saved as TLV files.

Raster levels are defined by drawing bitmap lines using the styles available in the raster drawing palette that is shared by all of the raster levels belonging to a specific project (see  :ref:`Project Default Folders <project_default_folders>`  ). Raster levels have a limited size and resolution, defined when they are created. They are saved as sequences of TIF files.

When an animation level is defined, you can select any of its frame in the xsheet or in the level strip, and start drawing in the work area. You can do this both when you want to create a drawing from scratch, and when you want to edit a previously made drawing.

When selected in the xsheet, the work area displays the whole scene content at the current frame; when selected in the level strip, the work area displays the selected frame of the current animation level only, to let you work more easily on it.

.. _setting_the_default_type_of_level_to_draw:

Setting the Default Type of Level to Draw
'''''''''''''''''''''''''''''''''''''''''
It is possible to define the level type that will be created by default when you draw inside Toonz.

The choice is among Toonz Vector Leveland Raster Level.

By default Toonz raster and vector levels are saved in the +drawing folder of the current project when the scene is saved, while raster levels are saved in the +extras folder (see  :ref:`Project Default Folders <project_default_folders>`  ).

.. tip:: **To define the Default Type of Level to Draw:**

    1. Open File>Preferences > Drawing.

    2. Choose the level type you want to use as default from the Default Level Type option menu. Widht, Height and DPI fields are available for Toonz Raster Level, Raster Level and Scan level.

.. note:: The Width, Height and DPI value set in the File>Preferences > Drawing page will be used as default by the New Level pop up.

Drawing Animation Levels
''''''''''''''''''''''''
Animation levels can be created in the following ways:

- Using the New Level dialog.

- Enabling the Autocreation option.

- Setting the Animation option to Use Xsheet as Animation Sheet.

.. _using_the_new_level_dialog:

Using the New Level Dialog
~~~~~~~~~~~~~~~~~~~~~~~~~~
New animation levels can be defined by using a dialog that lets you set the number of drawings the level is made of, the animation step used to expose the frames in the xsheet, and the increment, that sets the way the level drawings are numbered. For example, step 2 repeats each drawing twice in the xsheet column, while increment 2 numbers the drawings 1, 3, 5, etc. The dialog also allows you to choose a destination folder different from the default one by using the Save In field.

In case you define a Toonz raster or a raster level, you can set its Width, Height and DPI values, according to the way you want to use it in the scene.

Settings like the length of the level and the numbering order can be edited later, as you are free to arrange the images composing an animation level the way you prefer (see  :ref:`Editing Animation Levels <editing_animation_levels>`  ).

When a Toonz raster or vector level is defined, the color of the column cells where the level is exposed are colored in light green, the color denoting Toonz levels; when a raster level is defined, the color of the column cells where the level is exposed are colored in light blue, the color denoting raster images (see  :ref:`Working with Xsheet Columns <working_with_xsheet_columns>`  ). 

.. note:: The New Level dialog inherits the Level Type settings defined in Preferences > Drawing.

.. tip:: **To define an animation level to draw:**

    1. Do one of the following:

    - Select a cell in the xsheet where you want to place your animation level and choose File > New Level.

    - Right-click the cell in the xsheet where you want to place your animation level and choose New Level from the menu that opens.

.. note:: If a level is already exposed in the cell column, the new level will be created in an empty column.

    2. Choose the type of level, Toonz Vector, Toonz Raster or Raster, from the Type option menu, and define its settings, then click the OK button.

.. tip:: **To define the saving location for the level you want to draw:**

    In the New Level dialog type in the Save In field, or use the browser button, to set the path for the saving location.

.. note:: If in the browser you choose any project default folder, in the path field the full path will be replace by the related default folder alias (see  :ref:`Project Default Folders <project_default_folders>`  ).

.. _using_the_autocreation_option:

Using the Autocreation Option
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
When in Preferences > Drawing the Autocreation option is set to Enabled, it is possible to create new drawings automatically by using drawing tools in the work area. If the currently selected cell is empty, a new level will be automatically created and named with the first available letter of the alphabet; if the currently selected cell is right below one containing a level drawing, either in the xsheet or in the level strip, a new drawing will be added to the level.

.. note:: The level type is the one defined in Preferences > Drawing as Default Level Type.

.. _using_the_xsheet_as_animation_sheet:

Using the Xsheet as Animation Sheet
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
When in Preferences > Drawing the Autocreation option is set to Use the Xsheet as Animation Sheet, it is possible to create new drawings automatically by using drawing tools in the work area. If the currently selected cell is empty and belongs to an empty column, a new level will be automatically created and named with the first available letter of the alphabet; if the currently selected cell is below a cell containing a level drawing, a new drawing will be added to the level. In both cases the drawings will take its number from the scene current frame ; if the drawing already exists a letter will be added to its number (e.g. a.0001a.ext). 

This working method allows you to work as a traditional animator: you can start creating the key drawings and then add breakdown and inbetween drawings.You can quickly check your animation flipping it in the viewer.

When you add a new drawing it will be repeated as a hold along the column up to the following one.

It is also possible to create a new drawing in a cell that contains a hold: the new drawing will replace the hold up to the following drawing. Drawings can also be duplicated creating a copy with a different number.

Once the animation is completed you can renumber the whole sequence according to the xsheet frame numbering.

.. note:: The level type is the one defined in Preferences > Drawing as Default Level Type.

.. tip:: **To create a new animation level**

    Click an xsheet empty cell and start drawing using a drawing tool in the work area.

.. tip:: **To add a drawing to an existing level**

    Click an empty cell in the column containing the level and start drawing using a drawing tool in the work area.

.. tip:: **To automatically renumber the drawings**

    1. Select the drawings you want to renumber.

    2. Choose the Cells > Autorenumber command.

.. note:: The Autorenumber command is also available in the menu that opens when right-clicking in a cell.

.. _using_the_work_area:

Using the Work Area
'''''''''''''''''''
In the work area, or viewer, it is possible to use the tools available in the toolbar to draw, paint, edit and model drawings. The work area is endless and you can scroll, zoom in, zoom out and rotate it. 

In the title bar you can find information about what is currently displayed and selected, the zoom percentage, and a set of buttons that lets you set the view mode (see  :ref:`Using the Viewer <using_the_viewer>`  ).

At the bottom of the work area another customizable set of buttons is available. 

The frame bar and the playback buttons let you set the current frame and move through animation frames. The set frame rate is visualized, and in case the playback is activated, the actual frame rate is displayed on its left. 

The other buttons are relevant only using the Edit tool ( |Toonz71_061| ) to animate objects and when previewing the animation in the viewer (see 

:ref:`Animating Objects <animating_objects>`  and 

:ref:`Previewing the Animation <previewing_the_animation>`  ).



.. note:: If the bottom bar is too short to display all the options, it can be scrolled by using arrow buttons available at its ends.

.. note:: In case a frame range is defined by playback markers, the playback buttons refer to the defined range only (see  :ref:`Using the Playback Markers <using_the_playback_markers>`  ).

.. tip:: **To navigate the work area:**

    Do one of the following:

    - Use the Zoom tool ( |Toonz71_062| ): to zoom in, click and drag up; to zoom out, click and drag down. The point where you click is the center of the zooming action.



    - Use the zoom shortcut keys (by default + and - keys) to zoom in and zoom out at specific steps (e.g. 50%, 100%, 200%, etc.).

    - Use the mouse wheel to zoom in and zoom out.

    - Middle-click and drag or use the Hand tool ( |Toonz71_063| ) to scroll in any direction.

    - Use the Rotate tool ( |Toonz71_064| ) to rotate the work area: an horizon line is displayed to let you understand the amount of rotation; the center of rotation is the absolute center of the work area.

    - Use the reset view shortcut (by default the 0 key) or right-click in the viewer and select Reset View from the menu that opens, to display the viewer at its actual size, centered on the absolute center with no rotation applied.

    - Right-click and choose Fit to Window to automatically zoom the viewer so that it fits the camera box.

.. tip:: **To play the scene contents back:**

    Do one of the following:

    - Use the play button.

    - Drag the frame bar cursor.

.. tip:: **To set the current frame:**

    Do one of the following:

    - Use the playback buttons.

    - Drag the frame bar cursor.

    - Type in the frame bar field the number of the frame you want to view.

.. tip:: **To set the playback frame rate:**

    Do one of the following:

    - Enter a value in the FPS field.

    - Use the frame rate slider.

.. _adjusting_the_work_area_visualization:

Adjusting the Work Area Visualization
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
The way the work area visualizes the scene content can be adjusted according to the task to perform.

The full screen mode can be entered to maximize the work area to the monitor screen, hiding any interface window border. This is available only on Windows platform.

Vector drawings, that can slow down the visualization performance when used in large amounts in a scene, can be visualized as raster drawings, faster to visualize, still preserving their vector nature.

.. note:: If the current level is vector-based, it is displayed as it is, to allow any drawing and editing operation you may perform.

Raster drawings and images that usually are displayed in the work area according to their DPI value, can be displayed at their actual pixel size, that is to say that one pixel from the image is displayed as one pixel of the screen monitor, to better examine them.

.. note:: Visualizing an image at its actual pixel size is different from zooming in because zooming always takes into account the image DPI information.

.. tip:: **Windows only - to enter/exit the work area full screen mode:**

    Right-click the work area and choose Full Screen Mode/Exit Full Screen Mode from the menu that opens.

.. tip:: **To activate or deactivate the raster visualization for vector drawings:**

    Activate or deactivate the View > Visualize Vector As Raster check.

.. tip:: **To display raster drawings and images at their actual pixel size:**

    1. In the xsheet select the level to which the drawing or image belongs so that it becomes the current level.

    2. Select the drawing or image in the level strip in order to display it alone.

    3. Use the Actual Pixel Size shortcut (by default the N key) or right-click the work area and choose Actual Pixel Size from the menu that opens.

.. _customizing_the_work_area:

Customizing the Work Area
~~~~~~~~~~~~~~~~~~~~~~~~~
The work area can be customized according to your needs: the background colors visible in the work area and inside the camera box can be changed; a field guide and a safe area can be displayed for reference; the table and camera box can be hidden; custom guides can be added to help you aligning objects or composing the elements of the scene for a particular frame. The View>Inks Only check allows to hide the painted areas of the levels facilitating the drawing process.

The set of buttons and information available in the bottom bar of the work area can be customized as well, so that only the elements you requires are visible.

.. tip:: **To change the work area background color:**

    1. Open the Xsheet > Scene Settings dialog.

    2. Define the Viewer BG Color by doing one of the following:

    - Set the Red, Green and Blue values.

    - Click the color thumbnail and use the Style Editor to edit it (see  :ref:`Plain Colors <plain_colors>`  ).

.. tip:: **To change the camera box background color:**

    1. Open the Xsheet > Scene Settings dialog.

    2. Define the Camera BG Color by doing one of the following:

    - Set the Red, Green, Blue and Alpha values.

    - Click the color thumbnail and use the Style Editor to edit it (see  :ref:`Plain Colors <plain_colors>`  ).

.. tip:: **To show or hide the table:**

    Choose View > Table to show or hide the table.

.. tip:: **To show or hide the camera box:**

    Choose View > Camera Box to show or hide the camera box.

.. note:: The camera box visualization also triggers the safe area visualization (see below).

.. tip:: **To show or hide the camera background color:**

    Choose View > Camera BG Color to show or hide the camera box background color.

.. tip:: **To show or hide the field guide:**

    Choose View > Field Guide to show or hide the field guide.

.. tip:: **To define the displayed field guide:**

    1. Open the Xsheet > Scene Settings dialog.

    2. Define the Field Guide Size and A/R. The Size is the number of fields the field guide is wide (1 field is equal to 1 inch), and the A/R is the ratio between the field guide width and height.

.. tip:: **To show or hide the safe area:**

    Choose View > Safe Area to show or hide the safe area.

.. note:: The safe area is not visible if the camera box is hidden (see above).

.. tip:: **To define the displayed safe area:**

    1. Open the Xsheet > Scene Settings dialog.

    2. Define the Safe Area Box 1 and Box 2 by using values that represent percentages of the current camera size. 

.. tip:: **To add a custom guide:**

    Click in the ruler: a click in the horizontal ruler will create a vertical guide, a click in the vertical ruler will create an horizontal guide. 

.. tip:: **To move a custom guide:**

    Drag its marker in the ruler.

.. tip:: **To delete a custom guide:**

    Drag its marker outside of the viewer, in the opposite direction of the guide itself.

.. tip:: **To show or hide guides:**

    Choose View > Guides to show or hide the guides.

.. tip:: **To show or hide rulers where guide markers are located:**

    Choose View > Rulers to show or hide the rulers.

.. note:: When the work area is rotated, guides are rotated as well, but rulers and guide markers preserve their position and orientation. However the position of a guide can still be controlled by markers, even if visually they don’t match anymore.

.. tip:: **To customize the set of buttons in the bottom bar of the work area:**

    Click the option button ( |Toonz71_065| ) on the far left of the bottom area, and select the elements to show, or deselect those to hide, in the menu that opens. 



.. _drawing_tools:

Drawing Tools
'''''''''''''
You can draw by using the Brush( |Toonz71_066| ) and 

Geometric (

 |Toonz71_067| ) tools. For both tools you can set the thickness of the line you are going to draw: values range from 0 to 100 for Toonz vector levels, and from 1 to 100 for Toonz and standard raster levels.



.. note:: For Toonz and standard raster levels it is possible to set a the Brush tool size higher than 100 by typing the value in the Size text boxes.

.. note:: The Min and Max Thickness can be modified by pressing Shift or Ctrl and dragging the mouse without clicking. Press Ctrl to modify the Min thickness and Shift for the Max.

With the Brush tool ( |Toonz71_068| ), you can take full advantage of the pressure sensitivity if you are using a pressure sensitive tablet. The more you press on the tablet, the thicker the line you draw. 



With the Geometric tool ( |Toonz71_069| ), the thickness value is constantly applied to the whole shape you draw. 



When creating vector drawings the thickness can also be set to 0 (zero): in this case vector lines will only exist as a wireframe even if you zoom in or zoom out, and they will be not visible when the animation is rendered.

.. note:: For vector drawings, line thickness can be changed and calibrated afterwards by using other tools (see  :ref:`Editing Drawings <editing_drawings>`  ).

.. _drawing_with_the_brush_tool:

Drawing with the Brush Tool
~~~~~~~~~~~~~~~~~~~~~~~~~~~
The Brush tool( |Toonz71_070| ) allows you to draw freehand lines with the current style. 



When using a pressure sensitive tablet, and the Pressure Sensitivity option is activated, varying the pressure of the pen on the tablet will allow you to create variable-thickness lines that will make your drawings more expressive. 

When using the Brush tool ( |Toonz71_071| ) on Toonz and standard raster drawings, the cursor displays the exact pixel area that will be affected by the brush: the inner jagged circle representing the minimum brush thickness, and the outer one, the maximum.



In the tool options bar you can set the following:

- Thickness Min and Max sets the size of the brush; the size will vary between the two values if you're using a pressure sensitive tablet. If the two values are the same, your lines will have a constant thickness. When using a mouse to draw, the maximum thickness value will be used.

- Accuracy sets how ed the generated line is compared to what you draw with the mouse or on the tablet: a high value will generate lines that completely preserves the movement you perform (even a trembling hand); a low value will simplify the line. This is available for vector drawings only.

- Hardness sets the amount of antialiasing along the line border. This is available for Toonz and standard raster drawings only.

- Opacity Min and Max sets the opacity of the brush; the opacity will vary between the two values if you're using a pressure sensitive tablet. Overlapping areas are not considered while drawing a single line, but only when different lines are overlapping. This is available for raster drawings only.

- Break Sharp Angles automatically breaks the drawn vector into sections if very sharp angles are drawn: in this way drawn shapes may result simpler and easier to fill. This is available for vector drawings only.

- Selective allows the drawing operation without affecting already drawn lines. This is available for Toonz raster drawings only.

- Pencil Mode draws lines without antialiasing, that is with jagged edges. This is available for Toonz raster drawings only.

- Pressure Sensitivity detects, in case you are using a graphic tablet, the pressure of the pen on the tablet allowing the creation of variable-thickness lines.

- A brush preset can be chosen in the option menu on the right. You can add or remove a preset clicking the + and - buttons. A presets list is created for each level type and each added preset will be available for next use.

- The cap option sets the shape of the ends of the vector you are going to draw. Options are butt for squared ends, round for semicircular ends, and projecting for squared ends extending beyond the end of the line according to the vector thickness. This is available for vector drawings only.

- The join option sets the shape of the straight corners along the vector you are going to draw. Options are miter for pointed corners, round for rounded corners, bevel for squared corner. This is available for vector drawings only.

- Miter sets the maximum length of a miter join, that is computed multiplying the miter value by the stroke thickness. If the length exceeds the maximum value, the miter join is turned into a bevel join. This is available for vector drawings only, and only if the join option is set to miter.

.. note:: If the tool options bar is too short to display all the tool options, it can be scrolled by using arrow buttons available at its ends.

.. tip:: **To add a new brush preset:**

    1. Click the + button on the right of the presets list.

.. tip:: **To remove a new brush preset:**

    1. Click the - button on the right of the presets list.

.. _drawing_with_the_geometric_tool:

Drawing with the Geometric Tool
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
The Geometric tool( |Toonz71_072| ) allows you to draw rectangles, circles, ellipses, regular polygons, polylines and arcs. 



In the tool options bar you can set the following:

- Thickness sets the size of the brush used to draw the geometric shapes.

- Hardness sets the amount of antialiasing along the shape border. This is available for Toonz and standard raster drawings only.

- The shape can be chosen in the option menu. In case you want to draw a polygon, the Polygon Sides lets you set the number of sides.

- Auto Group automatically defines any drawn closed shape (i.e. rectangles, circles, ellipses, polygons and closed polylines) as a group, thus creating a new layer that is placed in front of the other drawing vectors, without intersecting them (see  :ref:`Grouping and Ungrouping Vectors <grouping_and_ungrouping_vectors>`  ). This is available for Toonz vector drawings only.

- Auto Fill automatically paints the area defined by any drawn closed shape (i.e. rectangles, circles, ellipses, polygons and closed polylines) with the same style used for drawing. This is available for Toonz vector drawings only.

- Selective allows the drawing operation without affecting already drawn lines. This is available for Toonz raster drawings only.

- Pencil Mode draws geometric shapes without antialiasing, that is with jagged edges. This is available for Toonz raster drawings only.

.. note:: If the tool options bar is too short to display all the tool options, it can be scrolled by using arrow buttons available at its ends.

While rectangles and ellipses are defined by a (bounding) box, circles and polygons are defined by a center and radius; polylines can be used to create open or closed shapes by defining a series of lines; arcs let you set the end points of a curve, and then the bend.

.. tip:: **To draw a rectangle or an ellipse:**

    Click to define the upper left corner, drag, and release to define the bottom right corner. If you press the Shift key while dragging, the shape will be regular, i.e. a square or a circle; if you press the Alt key, shapes will be drawn starting from their center.

.. tip:: **To draw a circle:**

    Click to define the center, drag and release to define the radius.

.. tip:: **To draw a polygon:**

    1. Set the number of sides in the Polygon Sides field.

    2. Click to define the center, drag and release to define the radius of a circle bounding the polygon.

.. tip:: **To draw a polyline:**

    1. Do one of the following:

    - Click to define the first point as a corner point.

    - Click and drag to define the first point as a control point; while dragging you can set the control point handles.

    2. Do one of the following:

    - Click to define the end point of the line as a corner point. If you press the Shift key, you will draw a vertical, horizontal or 45° line.

    - Click and drag to define the end point of the line as a control point; while dragging you can set the control point handles.

    3. Do one of the following:

    - Click or click and drag again to define the end point of another line connected to the end point of the previous line.

    - Double click to define the last point of an open shape. 

    - Click or click and drag again on the first point you defined to draw a closed shape.

.. note:: Press the Ctrl key to add a linear point after a Nonlinear one.

.. note:: Press the ESC key to to cancel the creation of the polyline.

.. tip:: **To draw an arc:**

    1. Click to define the first end point.

    2. Click to define the second endpoint.

    3. Drag to set the bend, and click to draw the arc.

.. _adding_text:

Adding Text
~~~~~~~~~~~
Text can be added by using the Type tool ( |Toonz71_073| ). In the tool options bar you can set the following:



    - The Font to be used, taken from a list based on the Operating System default fonts folder. 

    - The Style for the chosen font. 

    - The font Size, that can be chosen among a set of options. 

.. note:: Written text can be resized by using the Selection tool( |Toonz71_074| ) (see  :ref:`Editing Drawings <editing_drawings>`  ).

    - The Vertical Orientation option lets you place the text vertically, one letter under another, instead of horizontally.

The current palette style is applied to the text you type. The palette style can be changed while typing text, thus you can have characters having different styles in the same text editing session (see  :ref:`Editing Styles <editing_styles>`  ).

.. note:: For vector drawings, as soon as the text is committed, it is converted into vector outlines, and can no longer be edited as text.

.. tip:: **To add text:**

    1. Select the Type tool() and click in the work area where you want to start writing. 

    2. Choose options for the size, font and orientation. These options can be changed as long as you are in text editing mode.

    3. Change the current style in the palette if you want to use more than one style in the same text editing session.

    4. Click inside the text editing area to change the text insertion point.

    5. Click outside the text editing area, or select a different tool, to commit the text.

.. _using_the_eraser:

Using the Eraser
~~~~~~~~~~~~~~~~
The Eraser tool ( |Toonz71_076| ) allows you to partially erase lines, both in vector and raster drawings. 



In the tool options bar you can set the following:

- Size sets the eraser size.

- Hardness sets the amount of antialiasing along the eraser border. This is available for Toonz and standard raster drawings only.

- Opacity set the opacity of the eraser; passing twice on an area is not considered while performing a single erasing operation, but only when performing different erasing operations. This is available for raster drawings only.

- Type has the options Normal, to use the standard eraser; Rectangular, to perform the erasing inside the box you define; Freehand, to perform the erasing inside the area you outline by clicking and dragging; and Polyline, to perform the erasing inside the area you outline by defining a series of lines. In vector drawings, a vector is erased only if it is fully included in the area you define.

- Mode has the options Areas, to erase only areas, Lines, to erase only the drawing outline, and Lines & Areas, to perform both the operations. This is available only for raster drawings.

- Selective allows you to erase only lines or areas made with the current style. This is available only for Toonz raster and vector drawings.

- Invert performs the erasing on the outside of the area defined with the Rectangular, Freehand or Polyline options. In vector drawings, a vector is erased only if it is fully outside of the area you define.

- Frame Range allows you to perform Rectangular, Freehand and Polyline erasing on a range of frames, by defining an area in the first and then in the last frame of the range.

- Pencil Mode erases lines without antialiasing, that is with jagged edges. This is available for Toonz raster drawings only.

.. note:: If the tool options bar is too short to display all the tool options, it can be scrolled by using arrow buttons available at its ends.

.. note:: The Eraser tool ( |Toonz71_077| ) can be automatically selected by using the eraser of the tablet pen.



.. _converting_raster_drawings_to_vectors:

Converting Raster Drawings to Vectors
'''''''''''''''''''''''''''''''''''''
Scanned drawings and raster ones, i.e. drawings not based on vectors, can be converted into Toonz vector-based drawings.

Two main conversion modes are available: centerline and outline. The choice between the two modes depends on which conversion best fits your needs.




In centerline mode a single vector with a variable thickness is generated for each line in the drawing. This means that the converted drawing can be edited like vector-based drawings made directly in Toonz, for example you can change the bend of a vector with the Pinch tool ( |Toonz71_079| ) or with the Control Point Editor tool and the thickness with the Pump tool (

 |Toonz71_080| ).








In the outline mode two vectors are generated to define each line in the drawing, and areas filled with different colors are separated by a vector. This means that, for example, to change the bend of a line you have to change the bend of the two vectors defining it, and to change the thickness you have to model one or both vectors defining it. The thickness of all the vectors is set to 0, so that they won’t be visible in the final render.

.. note:: Parameters that are not considered necessary by the user can be hidden using the option button  |Toonz71_082|  at the bottom right of the Convert To vector Pop Up.



In the Outline mode the following settings are available:

- Accuracy sets how much the vector will follow the shape of the original drawing lines. High values create more precise vectors but makes them more complex.

- Despeckling removes small spots or marks from the converted images. Its value expresses the size in pixels of the side of the maximum area that has to be removed. 

- Preserve Painted Areas, when activated, includes all the colors in the converted level. 

- Adherence sets how much smooth curves bend toward full corners.

- Angle sets the angular threshold below which full corners are inserted in the image

- Curve Radius sets the measure of a curve's radius below which it is replaced by a smooth corner

- Max Colors defines the maximum number of colors that are considered in the raster image and used in the vector one. The value has to be set taking care of the real number of colors used in the raster image. High values increase the time needed for the conversion. This is relevant for raster levels only.

- Transparent Color defines the color that has to be set as the transparent background of the resulting vector level. This is relevant for raster levels only.

- Tone Threshold sets the value of the darkest pixels to be taken into account to detect lines to be converted to vectors; for low values only the darkest pixels are considered thus resulting in thinner lines; for high values lighter pixels are considered too, thus resulting in thicker lines. This is relevant for Toonz raster levels only.

In the Centerline mode the following settings are available:

- Threshold sets the value of the darkest pixels to be taken into account to detect lines to be converted to vectors; for low values only the darkest pixels are considered thus resulting in thinner vectors; for high values lighter pixels are considered too, thus resulting in thicker lines. For Toonz raster levels (TLV files) the process examines only pixels belonging to the lines; for full-color images, pixels of the whole image.

- Accuracy sets how much the vector will follow the shape of the original drawing lines. High values create more precise vectors but makes them more complex.

- Despeckling ignores during the conversion small areas generated by the image noise; the higher the value, the larger the areas ignored.

- Max Thickness sets the maximum vector thickness; if this value is low very thick lines will be converted in two centerline vectors defining the line outline; if this value is high, they will be converted in a single centerline vector.

- Thickness Calibration start and end calibrates the vector thickness defined according to the Threshold value; a low value will reduce the vector thickness preserving its integrity. A different value inserted in the Start / End field determines an animation of the thickness along the length of the level.

- Preserve Painted Areas, when activated, preserves all painted areas in Toonz raster levels (TLV files) and all the areas painted with colors different from the line color in full-color images.

- Add Border adds a vector along the image border in order to detect also areas bleeding off the image edge.

- Enhanced Ink recognition, when activated, allows to vectorize Full color images (such as TGA, TIF, PNG etc...) without antialiasing along the lines. An Heuristic is used to recognize lines and painted areas creating a PLI level where the lines are seen as ink and the painted areas as paint.

- It is possible to select the images or the level frames that have to be converted directly in the xsheet.

When a conversion is performed a new level is created according to the selection you made, and exposed in the xsheet in the column next to that containing the source level: the new file has the same name of the starting one but has a PLI extension, and a “v” suffix, and is saved in the +drawings default folder. 

.. note:: Toonz vector levels (PLI files) created with Toonz Harlequin 7.0 are not compatible with previous versions of the software.

.. note:: In case a PLI level with the same name already exists, the name of the new file will be followed by a progressive number.

.. tip:: **To convert raster drawings into vectors:**

    1. Select the images or the level frames to convert in the xsheet.

    2. Choose Level > Convert to Vectors.

    3. In the dialog set parameters for the conversion.

    4. Click the Convert button.

.. _checking_the_convert_to_vectors_process:

Checking the Convert to Vectors Process
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
At the bottom of the Convert-to-Vectors settings window a preview area is available to display the drawing selected in the xsheet as it will be after the conversion according to the defined settings. At the same time it allows you to compare the final result with the original raster drawing that is displayed on the left side, and to highlight the vector structure by clicking the Centerlines Check button ( |Toonz71_083| ).



You can activate or deactivate it, resize it or navigate its content.

If you change any parameter in the Convert-to-Vector settings, the previewed drawing automatically updates to display how the changes affect the result.

.. tip:: **To activate the preview area:**

    1. In the xsheet select the drawing you want to preview. 

    2. Click the Preview button ( |Toonz71_084| ) in the bottom bar of the Convert-to-Vector settings window.

.. tip:: **To deactivate the preview area:**

    Click the Preview button ( |Toonz71_085| ) in the bottom bar of the Convert-to-Vector settings window.



.. tip:: **To resize the preview area:**

    Do any of the following:

    - Click and drag the horizontal separator.

    - Click and drag the separator toward the window border to hide the preview area.

    - Click and drag the separator collapsed to the window border toward the window center to display again the preview area.

.. tip:: **To navigate the preview area:**

    Do one of the following:

    - Use the mouse wheel, or the zoom shortcut keys (by default + and - keys) to zoom in and zoom out.

    - Middle-click and drag to scroll in any direction.

    - Use the reset view shortcut (by default the 0 key) to display preview at its actual size

.. tip:: **To activate and deactivate the Centerlines Check:**

    Click the Centerlines Check button ( |Toonz71_086| ) in the bottom bar of the Convert-to-Vector window.



.. _saving_and_loading_convert_to_vector_settings:

Saving and Loading Convert To Vector Settings
'''''''''''''''''''''''''''''''''''''''''''''
Convert To Vector setting can be saved as tnzsettings files in order to have different settings for each level and to be loaded back and used in a different scene. 

Loaded Convert To Vector settings can also become the default settings for the scene or for the project (see  :ref:`Scene Settings and Project Default Settings <scene_settings_and_project_default_settings>`  ). 

.. tip:: **To save the Convert To Vector settings:**

    1. Click the Save Settings button () in the bottom bar of the Convert To Vector window.

    2. In the browser that opens choose for the tnzsettings file a location and a name, and click the Save button.

.. tip:: **To load saved Convert To Vector settings:**

    1. Click the Load Settings button () in the bottom bar of the Convert To Vector window.

    2. In the browser that opens retrieve the tnzsettings file you want to load, and click the Load button.

.. tip:: **To reset the Convert To Vector settings to the scene default:**

    Click the Reset Settings button ( |Toonz71_089| ) in the bottom bar of the Convert To Vector settings window.





.. _changing_the_canvas_size:

Changing the Canvas Size
------------------------
It is possible to change the size of Toonz and standard raster levels, in order to increase or decrease the area around the images of a level.

The new size can be set in any unit supported by Toonz, by using absolute or relative values. If the canvas is enlarged, some white transparent area is added; if the canvas is reduced, some cropping is applied to the level images.

.. tip:: **To change the canvas size:**

    1. Select the Toonz or the standard raster level you want to modify in the xsheet.

    2. Choose Level > Canvas Size: the Canvas Size dialog opens.

    3. In the dialog set the unit to express the new size of the canvas, and set the Width and Height of the new canvas; activate the Relative option to define the new size by specifying only the size the canvas has to increase or decrease.

    4. Use the Anchor diagram to decide the position of the current canvas in the new one: the arrows are a reference to see how the new size will increase or decrease the current canvas size.

    5. Click the OK button.

.. note:: In case the new canvas size is smaller than the current one, a confirmation dialog will open, asking you whether you want to crop the canvas.

.. _editing_drawings:

Editing Drawings
----------------
Toonz raster and vector drawings, and raster images, can be manipulated in Toonz.

To edit a drawing, for example to copy a part of it, you have first to select it in the xsheet or in the level strip. When selected in the xsheet, the work area displays the whole scene contents at the current frame, when selected in the level strip, the work area displays the selected frame of the current animation level only, to let you work more easily on it.

Drawings can be also selected directly in the work area: this allows you to work on the different drawings visible at a certain frame with no need to retrieve them in the xsheet or in the level strip.

.. note:: All the editing performed on drawings is not saved until you save the related level, or scene (see  :ref:`Saving Levels <saving_levels>`  ).

.. tip:: **To select the drawing to edit:**

    Do one of the following:

    - Select it in the xsheet or level strip.

    - Right-click in the work area the drawing you want to edit and in the menu that opens choose the Select command related to the column containing the drawing you want to edit.

.. note:: The right-click menu first lists all the columns containing overlapping drawings, then the columns and objects that are hierarchically linked to the clicked one.

.. _using_the_selection_tool:

Using the Selection Tool
''''''''''''''''''''''''
The Selection tool ( |Toonz71_090| ) allows you to edit, move, rotate, scale and distort a selection in a drawing. 



In the tool options bar you can set the following:

- Type has the options Rectangular, to select the area of the box you define by clicking and dragging; Freehand, to select the area you outline by clicking and dragging; and Polyline, to select the area you outline by defining a series of lines. In vector drawings, a vector is selected only if it is fully included in the area you define.

- Mode has the options Standard, to select vectors; Selected Frames, to edit all the lines of Selected Frames at once; Whole Level, to transform all of the drawings of the current animation level; Same Style, to select at once all of the vectors painted with the same style in the current drawing; Same Style on Selected Frames, to select at once all of the vectors painted with the same style in the Selected Frames of the current animation level; Same Style on Whole Level, to select at once all of the vectors painted with the same style in all the drawings of the current animation level; Boundary Strokes, to select all the bounderies stroke of the current drawing; Boundary Strokes on Selected Frames, to select all the bounderies stroke of the Selected Frame; Boundary Strokes on Whole Level, to select all the bounderies stroke of the Whole Level.This is available for Toonz vector drawings only.

- Preserve Thickness will preserve the original thickness of the drawing vectors while performing resizing operations. This is available for Toonz vector drawings only.

- Scale H and V set the horizontal and vertical scaling of the current selection; activating the Link options will maintain the proportions of the selection.

- Rotation sets the rotation of the current selection.

- Position N/S and E/W set a vertical and horizontal offset for the selection.

- Thickness sets the thickness of the selected vectors. In case the selected vectors have a variable thickness, or different thickness values, the highest value is displayed, and any change will affect the other values accordingly. This is available for Toonz vector drawings only.

- The cap option sets the shape of the ends of the selected vectors. Options are butt for squared ends, round for semicircular ends, and projecting for squared ends extending beyond the end of the line according to the vector thickness. This is available for vector drawings only.




    - The join option sets the shape of the straight corners along the selected vectors. Options are miter for pointed corners, round for rounded corners, bevel for squared corner. This is available for vector drawings only.




    - Miter sets the maximum length of a miter join, that is computed multiplying the miter value by the stroke thickness. If the length exceeds the maximum value, the miter join is turned into a bevel join. This is available for vector drawings only, and only if the join option is set to miter.

    - The Modify Savebox check box allows you to resize the Savebox of a drawing. The drawing part that, because of the editing, falls outside of the savebox will be erased. This is available for Toonz raster drawings only.

.. note:: The Savebox size can be set automatically to the minimum size activating the Preferences> Drawing> Minimize Savebox after Editing Option.

    - When the No Antialias option is activated the antialiasing is not applied when the selection is deformed or rotated. This is available on Raster and Toonz raster drawings only.

.. note:: If the tool options bar is too short to display all the tool options, it can be scrolled by using arrow buttons available at its ends.

When a selection is made, it is displayed with a bounding box with handles that allows you to perform the following transformations:

    - Click and drag any corner handle to scale the selection freely; by pressing the Shift key while dragging the scaling will be uniform; by pressing the Alt key the scaling will be applied from the center.

    - Click and drag any side handle to scale the selection in one direction; by pressing the Alt key the scaling will be applied symmetrically from the center.

    - Click and drag outside any corner handle to rotate the selection.

    - Click and drag the center handle to change the center of rotation, and the center used when Alt-scaling.

    - Ctrl-click (PC) or Cmd-click (Mac) any corner handle to distort the selection, or any side handle to shear it.

.. note:: Ctrl-click (PC) or Cmd-click (Mac) operations are not allowed in Whole Level mode (see above).

    - Click the double arrow-head at the bottom right corner of the selection and drag up to increase the thickness of selected lines, down to decrease it. This is available for Toonz vector drawings only.

    - Click and drag the inside of the raster selection, or any selected vector of a vector selection, to move it; by pressing the Shift key while dragging, the movement will be constrained on the horizontal or vertical direction. The Arrow keys can be used as well to move the selection one pixel right, left, up or down; if they are used while pressing the Shift key, the movement size will be ten pixels.

    - Click outside the selection to apply the transformation.

.. note:: As you roll over the handles, the cursor changes shape to indicate you the operations you may perform. 

Selections can also be cut, copied, pasted and deleted by using the relevant command in the Edit menu. Cut, or copy, and paste also works from one drawing to another, or to a new one. This allows you to copy or move a section of a drawing to another drawing, or split a drawing into several drawings.

When a Toonz drawing, or a section of a drawing, is pasted to another one, the colors of the pasted drawing are added to the palette of the target one, unless the same colors are already available in the palette.

.. note:: The vector selection can also be used to change the style of selected vectors by choosing it in the palette, or by creating a new style. See  :ref:`Editing Styles <editing_styles>`  . 

.. tip:: **To edit the drawing savebox:**

    1. Activate the Modify Savebox option to visualize the savebox around the drawing. 

    2. Use the handles to resize it.

    3. Switch Off the Modify Savebox check box to confirm the changes.

.. tip:: **To select and transform an area in a Toonz raster drawing or in a raster image:**

    1. Select the area by doing one of the following:

    - Set the type to Rectangular and click and drag to define the box whose area you want to select.

    - Set the type to Freehand and click and drag to outline the area you want to select.

    - Set the type to Polyline and click to outline the area you want to select by defining a series of lines.

    2. Do one of the following to make geometric transformations:

    - Operate the handles available along the bounding box.

    - Edit the scale, rotation and position values available in the tool options bar.




.. tip:: **To select and transform vectors in a Toonz vector drawing:**

    1. Select the vectors by doing one of the following:

    - Click a vector to select it.

    - Shift-click to add a vector to or remove it from the current selection.

    - Set the type to Rectangular and click and drag right to define a box and select all the vectors that are completely included in the box; click and drag left to select all the vectors that are partially included in the box.

    - Set the type to Freehand and click and drag to outline an area and select all the vectors that are completely included in the area.

    - Set the type to Polyline and click to outline an area by defining a series of lines and select all the vectors that are completely included in the area.

    - Set the mode to Same Style and click to select automatically all the vectors painted with the same style used for the vector you select in the current drawing, or Shift-click to add them to or remove them from the selection.

.. note:: When clicking a vector belonging to a group, the whole group is selected (see  :ref:`Grouping and Ungrouping Vectors <grouping_and_ungrouping_vectors>`  ). 

    2. Do one of the following to make geometric transformations:

    - Operate the handles available along the bounding box.

    - Edit the scale, rotation, position and thickness values available in the tool options bar.




.. tip:: **To select and transform all the drawings of a Toonz vector level:**

    1. Do one of the following:

    - Set the mode to Whole Level to automatically select all the vectors in all of the drawings of the current animation level. 

    - Set the mode to Same Style on Whole Level and click to select at once all of the vectors painted with the same style used for the vector you select in all of the drawings of the current animation level, or Shift-click to add them to or remove them from the selection.

    2. Do one of the following to make geometric transformations affecting all of the level drawings:

    - Operate the handles available along the bounding box.

    - Edit the scale, rotation, position and thickness values available in the tool options bar.

.. note:: When working on the whole level the bounding box displayed in the current level drawing is double-lined.

.. tip:: **To paste a selection in another existing drawing:**

    1. Make a selection in the current drawing.

    2. Copy/cut it.

    3. Select the other drawing in the level strip or in the .

    4. Paste the copied/cut selection.

.. note:: Selections from Toonz raster and vector levels can be pasted in any other type of drawing, automatically converting to raster or vector the pasted selection; selections from standard raster levels can be pasted in other standard raster drawings only.

.. tip:: **To paste a selection in a new drawing:**

    1. Make a selection in the current drawing.

    2. Copy/cut it.

    3. Select an empty frame in the level strip or an empty cell in the .

    4. Paste the copied/cut selection.

.. tip:: **To merge several drawings into one drawing:**

    1. Select the area you want to merge and copy/cut it.

    2. Select the drawing you want to paste the selection to.

    3. Paste the copied/cut selection.

.. note:: Several raster animation levels can also be merged at once by using the related command (see  :ref:`Merging Animation Levels <merging_animation_levels>`  ).

.. tip:: **To split a drawing into several drawings:**

    1. Select the area you want to use as a new drawing and copy/cut it.

    2. Select an empty cell in the .

    3. Paste the copied/cut selection: automatically a new drawing will be created.

.. _grouping_and_ungrouping_vectors:

Grouping and Ungrouping Vectors
'''''''''''''''''''''''''''''''
All the vectors of a drawing lie on the same layer, therefore drawing areas are outlined by segments defined by vector intersections. This means that if you draw two intersecting squares, automatically three areas are defined: one belonging only to the first square, one to the second one, and another defined by the intersection.




To organize vectors in layers you can use the grouping features, that creates a new layer containing only the vectors you select.

In the case of two intersecting squares, if you want the two squares to be overlapping instead of intersecting, you can create a group containing the vectors of the first square, and another those of the second square, thus defining two layers whose order can be arranged.

It is possible to create as many group as you want in any drawing; groups can be made of one vector only as well, for instance a circle, or a line.




When drawing with the Geometric tool ( |Toonz71_097| ) closed shapes (i.e. rectangles, circles, ellipses, polygons and closed polylines) can be defined automatically as a group by activating the Auto Group option (see 

:ref:`Drawing with the Geometric Tool <drawing_with_the_geometric_tool>`  ). 



When your vector selection includes one or several groups, the new group will include them as well, preserving them and their original layering position in case the group is released. 

.. note:: It is not possible to define a group if the selection includes only some strokes belonging to a group.

When a group is released, if no other group is defined in the same drawing, all the vectors will lie on the same layer; if other groups are defined, the vectors of the released group will lie on a layer placed behind, in front of, or between the other groups, according to the original group layering position.

It is possible to enter groups to isolate them visually from the rest of the drawing and better understand which vectors are inside and which outside the group. In this way it is also easier to work on the drawing, for instance to fill an area or to change the color of some vectors. 

As the Selection tool ( |Toonz71_098| ) considers the group as a whole, if you want to select a vector belonging to a group, first you have to enter the group, and then select the vector.



.. note:: As groups define layers, when using the Fill tool ( |Toonz71_099| ), only areas defined by vectors within the same group can be filled.



.. tip:: **To define a group:**

    1. Use the Selection tool () to select the vectors you want to be in a group.

    2. Do one of the following:

    - Choose Edit > Group.

    - Right-click on the selection and choose Group from the menu that opens.

.. tip:: **To release a group:**

    1. Select the group you want to release.

    2. Do one of the following:

    - Choose Edit > Ungroup.

    - Right-click on the selection and choose Ungroup from the menu that opens.

.. tip:: **To enter a group:**

    Do one of the following:

    - Select the group, then choose Edit > Enter Group.

    - Right-click the group and choose Enter Group from the menu that opens.

    - Double-click the group.

.. tip:: **To exit a group:**

    Do one of the following:

    - Choose Edit > Exit Group.

    - Right-click the group and choose Exit Group from the menu that opens.

    - Double-click outside the group.

.. tip:: **To select a group:**

    Choose the Selection tool ( |Toonz71_101| ) and do any of the following:



    - Click any vector belonging to the group.

    - Click and drag to select at least one vector belonging to the group.

    - Set the type to Rectangular and click and drag to define a box and select at least one vector belonging to the group.

    - Set the type to Freehand and click and drag to outline an area and select at least one vector belonging to the group.

    - Set the type to Polyline and click to outline an area by defining a series of lines and select at least one vector belonging to the group.

.. tip:: **To select a vector in a group:**

    1. Enter the group.

    2. Click the vector to select it.

.. _setting_stroke_and_group_layering_order:

Setting Stroke and Group Layering Order
'''''''''''''''''''''''''''''''''''''''
For each drawing, vectors and groups layering order can be changed by setting what has to lie in front of, and what behind.




.. tip:: **To bring the selection to front:**

    Do one of the following:

    - Choose Edit > Bring to Front.

    - Right-click on the selection and choose Bring to Front from the menu that opens.

.. tip:: **To bring the selection one layer forward:**

    Do one of the following:

    - Choose Edit > Bring Forward.

    - Right-click on the selection and choose Bring Forward from the menu that opens.

.. tip:: **To send the selection back:**

    Do one of the following:

    - Choose Edit > Send Back.

    - Right-click on the selection and choose Send Back from the menu that opens.

.. tip:: **To send the selection one layer backward:**

    Do one of the following:

    - Choose Edit > Send Backward.

    - Right-click on the selection and choose Send Backward from the menu that opens.

.. _editing_vector_drawings:

Editing Vector Drawings
'''''''''''''''''''''''
Vector drawings can be edited in some additional ways by using the set of tools. This allows you for example to better calibrate the bend of a vector, or to change its thickness.

All these transformations can be also achieved on already painted drawings, because the fill styles used to paint will automatically follow the shape of the areas you modify, working like “liquid” color flooding an area defined by an outline.

.. _editing_vector_control_points:

Editing Vector Control Points
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
To modify a vector by editing its control points you can use the Control Point Editor tool ( |Toonz71_103| ). 



Control points have handles whose length and direction define the bend of the vector. With this tool you can select a vector and modify the control point handles, or the bend of a curve defined by control points, and move, add or delete control points.

Control point handles may be linked, that is to say they share the same direction, or not, creating a cusp in the vector; they can also be collapsed in the control point in order to turn it in a corner point. In case only one handle is collapsed, the point will be corner on one side and smooth on the other. When a section of the vector is defined by two corner points, it will be a straight line.

The option Auto Select Drawing is available to automatically select any vector of any drawing visible in the work area.




.. tip:: **To select a vector:**

    Click it.

.. tip:: **To edit the bend of a vector:**

    Do any of the following:

    - Click and drag the ends of the control point handles.

    - Click and drag the curve defined by the control points to edit it.

    - Shift-click and drag the curve defined by the control point to edit it by keeping the control points position fixed.

.. tip:: **To unlink the control point handles:**

    Alt-click one of the handle ends and drag.

.. tip:: **To link the control point handles:**

    Alt-click one of the handle ends and drag: the other handle snaps to the direction of the one you are dragging.

.. tip:: **To add a control point:**

    Ctrl-click (Pc) or Cmd-click (Mac) the vector where you want to add a control point.

.. tip:: **To select control points:**

    Do one of the following:

    - Click a control point to select it.

    - Ctrl-click (Pc) or Cmd-click (Mac) a control point to add it to the selection.

    - Click and drag to select all of the control points that are included in the selection area. 

.. tip:: **To move the selection:**

    Do one of the following:

    - Click any selected control point and drag.

    - Use the Arrow keys to move the selection one pixel right, left, up or down.

.. tip:: **To delete the selection:**

    Choose Edit > Delete.

.. tip:: **To turn a control point into a corner point:**

    Do one of the following:

    - Alt-click the control point.

    - Move the handle ends to the control point, in order to collapse them.

    - Right-click the control point and choose Set Linear Control Point from the menu that opens.

.. tip:: **To retrieve handles from a corner point:**

    Do one of the following:

    - Alt-click the corner point.

    - Right-click the control point and choose Set Non-linear Control Point from the menu that opens.

.. _changing_the_bend_of_vectors:

Changing the Bend of Vectors
~~~~~~~~~~~~~~~~~~~~~~~~~~~~
To modify a bend of a vector in a more intuitive way you can use the Pinch tool ( |Toonz71_105| ). You can use it anywhere you want on the vector in order to modify the bend in any direction. 



When the tool is selected, a segment of the center line of the closest vector is highlighted: the segment shows the length of the vector that will be affected by the pinching. 

The length of the segment depends on the corner points that the tool automatically detects along the vector according to the Corner value. It can also be manually set by activating the Manual option thus using the Size value to set the affected length.

When the manual mode is activated a handle is displayed along the highlighted vector to control interactively the length of the segment that will be affected by the tool. The handle has a double circle and a square at its ends, that allows you to do the following:

- The double circle lets you move the handle along the segment;

- The square lets you increase the length of the segment affected by the tool by clicking and dragging right, or decrease it by clicking and dragging left.

In both automatic and manual modes different types of editing can be performed when clicking and moving the cursor:

- Click and drag to change the bend of the highlighted segment.

- Shift-click and drag to edit the highlighted segment by adding a cusp.

- Ctrl-click (Pc) or Cmd-click (Mac) and drag to edit the highlighted segment by adding a corner.

.. tip:: **To modify the bend of a vector:**

    1. Change the length of the segment affected by the tool by setting the Corner value in the tool options bar.

    2. Click, Shift-click, or Ctrl-click (Pc) or Cmd-click (Mac) and drag to modify the bend of the highlighted segment.




.. tip:: **To modify the bend of a vector in manual mode:**

    1. Activate the Manual option in the tool options bar.

    2. Change the length of the segment affected by the tool by doing one of the following:

    - Set the Size value in the tool options bar.

    - Click and drag the small square at one end of the handle displayed along the highlighted vector.

    3. Click, Shift-click, or Ctrl-click (PC) or Cmd-click (Mac) and drag to modify the bend of the highlighted segment.

.. tip:: **To eliminate a corner point from a segment:**

    1. Click and drag the point until the smooth segment is formed again.

    2. Click and drag to correct the bend of the newly smoothed segment.

.. _using_other_modifier_tools:

Using Other Modifier Tools
~~~~~~~~~~~~~~~~~~~~~~~~~~
To modify the thickness of a vector you can use the Pump tool ( |Toonz71_107| ). You can use it anywhere you want on the vector to increase or decrease the thickness locally. When the tool is selected, a segment of the closest vector is highlighted: the segment shows the length of the vector that will be affected by the tool. To modify this length you can change the Size value in the tool options bar.



.. note:: It is possible to modify the thickness of a vector, a vector selection, or vectors in all of the level drawings, by using the Selection tool ( |Toonz71_108| ) and its related options (see 

:ref:`Using the Selection Tool <using_the_selection_tool>`  ).



To distort more than one vector at once, you can use the Magnet tool ( |Toonz71_109| ). The tool affects all vectors included in a circular area and allows you to distort them in the direction of your dragging. Highlighted segments will show the vectors that will be affected. To modify the action range of the tool, represented by a circle, you can change the tool size in the tool options bar.



To bend a part of a drawing, for example a character’s arm, you can use the Bender tool ( |Toonz71_110| ). The tool allows you to define a line and then bend all the vectors intersected by the segment. While bending you can see the affected vectors assuming their position after the transformation. The bending can be performed in both clockwise and counterclockwise direction; once you start dragging you cannot change the bend direction.



.. note:: If you move the cursor far from the bending center, you will be able to set with more precision the amount of bend you want to apply to the vectors.

To smooth a vector, you can use the Iron tool ( |Toonz71_111| )


. When used again and again on a vector, it increasingly flatten the bends of the vector. When the tool is selected, the cursor snaps to the closest vector to indicate where you are going to operate. 



.. tip:: **To modify the thickness of a vector:**

    1. Select the Pump tool ().

    2. Set the Size value in the tool options bar.

    3. Click the point of the vector where you want to modify the thickness and drag up to increase the thickness, or down to decrease the thickness. 




.. tip:: **To distort several vectors at once:**

    1. Select the Magnet tool ().

    2. Click in the viewer: all the vectors included in the circle will be affected by the tool. 

    3. Drag to distort the vectors in the direction of your dragging. 

.. tip:: **To bend one or several vectors:**

    1. Select the Bender tool ().

    2. Click on one side of the vectors you want to bend to set the center of the bend.

    3. Click on the opposite side of the vectors: all vectors intersected by the defined line will be affected by the bending. 

    4. Drag in the direction you want to bend vectors. 

.. tip:: **To smooth a vector:**

    1. Select the Iron tool ().

    2. Click and drag along the vector you want to smooth. By dragging over and over you increasingly flatten the vector.

.. _joining_and_splitting:

Joining and Splitting
~~~~~~~~~~~~~~~~~~~~~
To join the ends of two different vectors, you can use the Tape tool( |Toonz71_117| ). This way it will be possible to handle them as a single vector, for instance for modifying their bend, or thickness, as a whole. 



When the tool is used, the pointer snaps to the closest detected vector endpoint in order to make the operation easier.

.. note:: The Tape tool ( |Toonz71_118| ) can also be used to close gaps along the drawing outline for painting purposes (see 

:ref:`Closing Gaps in Drawing Outline <closing_gaps_in_drawing_outline>`  ).



To do the contrary, that is to say splitting a vector in two sections, you can use the Cutter tool ( |Toonz71_119| ). 



.. tip:: **To join two open ends of one or two vectors:**

    1. Select the Tape tool (), and activate the Join Vectors option; activate also the Smooth option if you want a joining with no corners.

    2. Do one of the following: 

    - Set the type to Normal and the mode to Endpoint to Endpoint, click a vector endpoint and drag to a different endpoint; the pointer snaps to the closest detected vector endpoint.

    - Set the type to Rectangular, and click and drag to define a box including the endpoints you want to connect; the endpoints will be automatically joined according to the set distance value. 

.. note:: If the vectors you are going to join have different styles, the style of this first vector you click will be assigned to the second one after joining.

.. tip:: **To split a vector:**

    1. Select the Cutter tool (): the pointer snaps to the closest vector indicating, with a small highlighted segment, the point where you are going to split the vector.

    2. Click to split the vector in the highlighted point.

.. _cleaning_up_vector_intersections:

Cleaning up Vector Intersections
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Vector intersections may be a weak point in drawings to be painted, because if a gap occurs, drawing areas cannot be painted properly.

The best solution for this kind of issue is to overlap the final section of vectors, in order to define clear intersections, then automatically remove the sections that overflow. 

.. tip:: **To cleanup vector intersections:**

    1. Use the Selection tool () to select the vectors whose intersections you want to cleanup.

    2. Do one of the following:

    - Choose Edit > Remove Vector Overflow.

    - Right-click the selection and choose Remove Vector Overflow from the menu that opens.

.. _animation_techniques:

Animation Techniques
--------------------
Besides drawing frame by frame, one image at a time, until you achieve the animation you want, some other techniques are easier to achieve thanks to Toonz features.

Whatever the technique is, you can control your work and how smooth the animation is by using the onion skin, that allows you to view more than one image in the viewer at the same time as reference.

.. _modelling_a_vector_drawing:

Modelling a Vector Drawing
''''''''''''''''''''''''''
Instead of animating a level by starting every time from a blank frame, you can duplicate a vector drawing and make subsequent modifications. You can do it even if the drawings are painted, because the styles used to paint will automatically follow the shape of the areas you modify (see  :ref:`Editing Drawings <editing_drawings>`  ).

The sequence of the animation level drawings can be easily controlled in the level strip.

You can use both the Edit > Duplicate Drawing command and the standard Copy and Paste commands to make a copy of a drawing that you can later modify to create slight movements.

When you use the Duplicate Drawing command, the selected drawing is duplicated in the following frame. If the following frame already contains a drawing, it is shifted down in order to insert the duplicated drawing in the sequence.

When you use the Copy and Paste commands, you can also decide the frame of the level strip where you want to paste the drawing.

Once finished, you can make a copy of the modified drawing, and modify it in its turn. You can go on duplicating and modifying drawings until you complete the animation level.

.. tip:: **To create an animation level by modelling vector drawings:**

    1. In the , select a drawing of the vector animation level you want to edit.

    2. In the level strip, select the drawing you want to duplicate.

    3. Copy the selected drawing in the following frame by doing one of the following:

    - Choose Cells > Duplicate Drawing.

    - Choose Edit > Copy, then select the following frame and choose Paste.

    4. Select the new drawing in the level strip.

    5. Use modifier tools to modify the drawing.

    6. Go on duplicating and modifying drawings until you complete the animation level.

.. _using_the_in-betweener_with_vector_drawings:

Using the In-betweener with Vector Drawings
'''''''''''''''''''''''''''''''''''''''''''
An animation technique reserved to vector animation levels is the use of the in-betweener in the level strip. The in-betweener creates in-between drawings once you have selected a starting drawing and an ending one.

When more than two frames are selected in the level strip, a vertical strip is displayed on the right of the pane. By clicking on it all frames between the first and the last selected frame will be overwritten by images interpolating the first and the last image. 

The interpolated drawings are created by taking into account the number of the vectors, and the vectors direction. This means that the result will depend on the way drawings were made. For example if the first image is a single shape drawn clockwise, and the last is another shape, you will get different results depending on the way it was drawn, clockwise or counterclockwise.

 |Toonz71_123| 

To obtain the best results with complex drawings, copy the drawing you want to interpolate from, and paste it in another frame of the level strip. Modify the pasted drawing without adding and deleting vectors, but only distorting and moving existing vectors (see  :ref:`Editing Drawings <editing_drawings>`  ). Select the whole range and then perform the interpolation.

The interpolation speed can be controlled in the dialog opening when performing in-betweening. Options are the following:

- Linear, for a constant interpolation. 

- Ease In, for an interpolation starting slowly, then getting faster. 

- Ease Out, for an interpolation starting quickly, then getting slower. 

- Ease In Out, for an interpolation starting slowly, getting faster, then getting slower again.

If you want the interpolation to last more or less frames, you can insert frames, or cut them, and use the in-betweener again.

.. tip:: **To create in-between drawings:**

    1. Select the level where you want to perform interpolation.

    2. In the level strip select the frame range from the drawing you want to interpolate from, to the one you want to interpolate to. If you want the interpolation to last more frames, make room for more drawings with the Edit > Insert command.

    3. Click the vertical strip displayed on the right of the frame range selection.

    4. Select the in-between mode among Linear, Ease In, Ease Out, Ease In Out, and click the In-between button.

.. tip:: **To optimize the in-betweening process:**

    1. Create and paint the drawing you want to interpolate from.

    2. Do one of the following:

    - Copy and paste it in another frame of the level strip, considering the number of in-between drawings you want to achieve.

    - Duplicate it and insert as many empty frames as the number of in-between drawings you want to achieve.

    3. Modify the pasted, or duplicated, drawing using the modifier tools, to create the final drawing of the interpolation.

    4. Select the frame range from the drawing you want to interpolate from, to the one you want to interpolate to.

    5. Click the vertical strip displayed on the right of the frame range selection.

.. _rotoscoping:

Rotoscoping
'''''''''''
Rotoscoping consists of tracing drawings taking a live clip as reference. 




As you can import clips and frame sequences in a scene, you can simply load them, and create an animation level by drawing in the work area, while the frames of the clips are visible underneath. See  :ref:`Using the File Browser <using_the_file_browser>`  . 

The way to obtain best results is not trying to reproduce with fidelity the clip, but to use its frames just as a reference to better understand the movement or the transformation of the clip’s subject. In this way you can take advantage, for example, of a natural movement represented in the clip, without renouncing an expressive drawing style.

.. tip:: **To perform rotoscoping:**

    1. Load a QuickTime or Avi clip, or a sequence of frames, in the . The clip will be placed in a column of the .

    2. In the  select a cell in a column on the right of the column containing the clip you loaded. The image of the clip placed at the same frame of the cell you selected will be visible in the work area while you are drawing.

    3. Create a new animation level and use tools to trace the first drawing in the work area.

    4. Move to next frames, and trace the next drawings.

.. _cloning_levels:

Cloning Levels
''''''''''''''
Sometimes it may be useful to create a clone of a level in order to edit it without affecting the original one. For example you may want to create a new animation level starting from the drawings of another level, in order to have two sequences similar but not identical.

The Clone command allows you to create a copy of the selected cells, preserving the numbering order and assigning a name to the clone. The _clone suffix appended to the name of the level is the default.

The cloned level will contain only drawings exposed in selected cells, even if the original level is made of more drawings; they will be automatically exposed in the column on the right of the selection, shifting the following columns.

The new level will be available in the scene cast as a new element; it will be saved in the +drawings or +extras default folder according to the format of the original file as soon as you save it with the save command, or you save the scene.

The cell selection can also spread over several columns: in this case the same number of new columns will be inserted to make room for the cloning result. If more than one level is selected, the same number of new levels will be created and it is not possible to assign a name to the cloned levels.

.. tip:: **To clone levels:**

    1. Select the cells you want to clone.

    2. Do one of the following:

    - Choose Cells > Clone.

    - Right-click in the selection and choose Clone from the menu that opens.

    3. Enter a name for the Cone Level and press OK to confirm.

.. _using_onion_skin:

Using Onion Skin
----------------
If you want to view more than one level drawing at the same time in the viewer as reference when you create drawings, or you want to check the animation, you can activate the onion skin mode. 

The onion skin is available both in the  and in the level strip according to where the cursor showing the current frame is displayed, as the onion skin can be activated starting from the cursor and managed in the frame number column. 




When a frame of the level strip is selected, the onion skin refers to the current level only, referring to the sequence of the full animation level as it was created.

When a cell of the  is selected, the onion skin refers to the current level according to how the drawing sequence is edited in the scene, including movements and transformations performed thanks to the object animation (see  :ref:`Animating Objects <animating_objects>`  ), while the rest of the scene related to the current frame will be visible as is. If you want you can also extend the onion skin to the whole content of the , to allow references to all the animated or moving elements in the scene as well.

The relative onion skin mode displays frames in relation to the position of the current frame. For instance you can activate the frame previous to the current one, and every time you change the current frame, the previous frame will be displayed in onion skin mode. 

The fixed onion skin mode displays the selected frame independently from the current frame. For instance you can activate frame 5, and every time you change the current frame, frame 5 will be displayed in onion skin mode.

The way images are displayed in onion skin mode can be customized in the Preferences dialog: it is possible to define the Paper Thickness, to set a color correction for previous frames and one for following frames, and to display Toonz levels with lines only.

.. tip:: **To activate frames in relative onion skin mode:**

    1. Click and drag the small squared markers available on the left of the current frame cursor. If you drag up you will display previous images, if you drag down you will display following images. 

    2. Once you have activated the relative onion skin, clicking the marker related to each frame lets you decide which frame to hide or show. Click and drag automatically hides or shows a series of frame.

.. tip:: **To activate or deactivate frames in fixed onion skin mode:**

    Do one of the following:

    - In the , click the squared markers appearing in ghost mode on the left of the frame column. Click and drag automatically activates or deactivates a series of frames. 

    - In the level strip, click in the white area on the top left of the strip frames. Click and drag automatically activates or deactivates a series of frames. 

.. tip:: **To deactivate or activate again the onion skin mode:**

    Do one of the following:

    - Click in the area on the left of the current frame cursor, where two squares are visible. Click again in the same area to display again the previous onion skin configuration.

    - Right-click in the viewer, or in the frame column of the  and level strip, and choose Deactivate Onion Skin or Activate Onion Skin in the menu that opens.

.. note:: The first time you click in the area on the left of the current frame cursor you will activate a default onion skin mode, showing the previous three frames in relative onion skin mode.

.. tip:: **To extend the onion skin to the whole  content:**

    1. Activate the onion skin in .

    2. Right-click in the viewer, or in the frame column of the , and choose Extend Onion Skin to Scene from the menu that opens.

.. tip:: **To limit the onion skin to the current level:**

    Right-click in the viewer, or in the frame column of the , and choose Limit Onion Skin to Level from the menu that opens.

.. tip:: **To customize the way images are displayed in onion skin mode:**

    1. Choose File > Preferences > Onion Skin.

    2. Do any of the following:

    - Set a value for the Paper Thickness; the lower the value, the more transparent the drawings displayed in onion skin mode.

    - Use the Previous Frames Correction to set a color for displaying previous frames.

    - Use the Following Frames Correction to set a color for displaying following frames.

    - Activate the Display Lines Only option to display Toonz levels with lines only.

.. _using_the_shift_and_trace:

Using the Shift and Trace
-------------------------
The shift and trace function can help you in the creation of animated levels as you were drawing on paper with the light table; in fact it allows you to use the previous and the next drawing as reference when you insert an inbetween or a break down. 

It possible to temporary move and rotate the drawings you want to use as reference to fit the position where you want to draw the inbetween one. It is also possible to automatically set the position of the reference drawings creating and editing a path of action line.

To better check the new drawing and the animation you can toggle the shift and trace visualization on the viewer.

.. tip:: **To enter the shift and trace view:**

    1. Position the frame cursor on the frame where you want to draw the inbetweening drawing.

    2. Enable View > Shift and Trace: the previous and next drawing will be visualized.

.. tip:: **To edit the position of the reference drawings:**

    1. Position the frame cursor where you want to draw the inbetween drawing and sketch the path of action line beteween your reference points.

    2. Activate View > Edit Shift.

    3. Click on the drawing you want to reposition: the related bounding box will be displayed.

    4. Do any of the following:

    - Click and drag anywhere to move the reference drawing.

    - Click and drag any corner handle to rotate the reference drawing.

    - Click and drag the center handle to change the center of rotation.

    5. Repeat the same steps on the second reference drawing.

.. tip:: **To automatically edit the position of the reference drawings:**

    1. Position the frame cursor where you want to draw the inbetween drawing and sketch the path of action line beteween your reference points.

    2. Activate View > Edit Shift.

    3. Ctrl-click and drag to create a path from the reference point in the first drawing to the reference point in the second one. The starting and the ending points will be overlapped at the center of the path.

    4. Click and drag the handle along the path to change the shape of the path: the reference drawings will move according to the handle position and rotate according to the path shape modification.

    5. If needed use the bounding box handles to fix the rotation of the reference drawing. 

.. note:: Clicking and dragging one of the reference drawings will remove the path of action line.

.. tip:: **To toggle the shift:**

    Activate View > No Shift to toggle the visualization of the reference drawings in their original position.

.. tip:: **To reset the position of the reference drawings:**

    Choose the View > Reset Shift command.

.. tip:: **To create an inbetween drawing using the shift and trace:**

    1. Create the first key drawing.

    2. Create the second key drawings.

    3. Select the cell where you want to create the inbetween drawing.

    4. Activate View > Shift and Trace.

    5. Sketch the path of action line beteween your reference points.

    6. Activate View > Edit Shift and edit the position of the reference drawings.

    7. Create the inbetween drawing.

.. |Toonz71_061| image:: /_static/Toonz71/Toonz71_061.gif
.. |Toonz71_062| image:: /_static/Toonz71/Toonz71_062.gif
.. |Toonz71_063| image:: /_static/Toonz71/Toonz71_063.gif
.. |Toonz71_064| image:: /_static/Toonz71/Toonz71_064.gif
.. |Toonz71_065| image:: /_static/Toonz71/Toonz71_065.gif
.. |Toonz71_066| image:: /_static/Toonz71/Toonz71_066.gif
.. |Toonz71_067| image:: /_static/Toonz71/Toonz71_067.gif
.. |Toonz71_068| image:: /_static/Toonz71/Toonz71_068.gif
.. |Toonz71_069| image:: /_static/Toonz71/Toonz71_069.gif
.. |Toonz71_070| image:: /_static/Toonz71/Toonz71_070.gif
.. |Toonz71_071| image:: /_static/Toonz71/Toonz71_071.gif
.. |Toonz71_072| image:: /_static/Toonz71/Toonz71_072.gif
.. |Toonz71_073| image:: /_static/Toonz71/Toonz71_073.gif
.. |Toonz71_074| image:: /_static/Toonz71/Toonz71_074.gif
.. |Toonz71_076| image:: /_static/Toonz71/Toonz71_076.gif
.. |Toonz71_077| image:: /_static/Toonz71/Toonz71_077.gif
.. |Toonz71_079| image:: /_static/Toonz71/Toonz71_079.gif
.. |Toonz71_080| image:: /_static/Toonz71/Toonz71_080.gif
.. |Toonz71_082| image:: /_static/Toonz71/Toonz71_082.gif
.. |Toonz71_083| image:: /_static/Toonz71/Toonz71_083.gif
.. |Toonz71_084| image:: /_static/Toonz71/Toonz71_084.gif
.. |Toonz71_085| image:: /_static/Toonz71/Toonz71_085.gif
.. |Toonz71_086| image:: /_static/Toonz71/Toonz71_086.gif
.. |Toonz71_089| image:: /_static/Toonz71/Toonz71_089.gif
.. |Toonz71_090| image:: /_static/Toonz71/Toonz71_090.gif
.. |Toonz71_097| image:: /_static/Toonz71/Toonz71_097.gif
.. |Toonz71_098| image:: /_static/Toonz71/Toonz71_098.gif
.. |Toonz71_099| image:: /_static/Toonz71/Toonz71_099.gif
.. |Toonz71_101| image:: /_static/Toonz71/Toonz71_101.gif
.. |Toonz71_103| image:: /_static/Toonz71/Toonz71_103.gif
.. |Toonz71_105| image:: /_static/Toonz71/Toonz71_105.gif
.. |Toonz71_107| image:: /_static/Toonz71/Toonz71_107.gif
.. |Toonz71_108| image:: /_static/Toonz71/Toonz71_108.gif
.. |Toonz71_109| image:: /_static/Toonz71/Toonz71_109.gif
.. |Toonz71_110| image:: /_static/Toonz71/Toonz71_110.gif
.. |Toonz71_111| image:: /_static/Toonz71/Toonz71_111.gif
.. |Toonz71_117| image:: /_static/Toonz71/Toonz71_117.gif
.. |Toonz71_118| image:: /_static/Toonz71/Toonz71_118.gif
.. |Toonz71_119| image:: /_static/Toonz71/Toonz71_119.gif
.. |Toonz71_123| image:: /_static/Toonz71/Toonz71_123.gif
