Edge derive
===========

.. image:: edgeDerive.png
    :width: 80%
    :align: center

Edge derive makes it possible to quickly derive length-specific parts into a part studio. Mate connectors attatched to derived parts are automatically converted into selectable points, and various positioning options are also avaialable by default.

The Edge derive FeatureScript can be found here: `Edge derive document <https://cad.onshape.com/documents/ad42d9d1532c5ea87446b1e8/w/2ed67f49f3f015638cdeb398/e/05f19623ee55474ef77cab5e>`_

Steps for deriving entities
---------------------------

#. Create a Edge derive feature by selecting it from your :term:`FeatureScript dropdown`.
#. Specify **Entities to import**.
#. Select one or more edges to derive parts along.
#. For each selected edge, a set of manipulators are automatically created in the graphics window which enable positioning.

.. image:: edgeDeriveManip.png
    :width: 60%
    :align: center

#. Choose whether to **Move** parts relative to their reference edges.
#. Choose whether to **Delete planes and sketches** from **Entities to import**.
#. |confirm-feature|

.. image:: edgeDeriveUI.png
        :width: 40%
        :align: center

Steps for setting up parts to be derived with edge derive
--------------------------------------------------------------

#. Create a new part studio.
#. In the **Configuration panel** on the right side of the screen, add a **Confirguation variable** named "length" (lowercase 'l').
#. Use the configuration to drive the length of your part.
#. If desired, add one or more mate connectors with their z-axis facing upwards to the middle of the part. When the part is derived using Edge derive, these mate connectors will be converted into selectable points.
#. Add additional configurations and modifications to the part studio as desired.

.. image:: edgeDerivePart.png
        :width: 60%
        :align: center

.. note:: 
    A sample part studio can also be found here:
    `Edge derive example part studio <https://cad.onshape.com/documents/567e587532cc61cedf4afcd4/w/d46a937c79b679f60c070ec7/e/a2ce9f9fc6c3ab079d1d8d1a?configuration=length%3D0.254%2Bmeter&renderMode=0&uiState=61f7620f427777032afbb25e>`_