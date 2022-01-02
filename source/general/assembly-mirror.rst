Assembly mirror
===============

Assembly mirror facilitates assembly behavior by adding mate connectors to parts 
which allow instances of those parts to be quickly placed in mirrored positions in assemblies. 

Steps for creating mirrored parts
---------------------------------

  #. Create an Assembly mirror feature by selecting it from your :term:`FeatureScript dropdown`.
  #. Specify your desired result behavior (**Part center** or **Origin**).

    .. seealso::
        :ref:`result-behavior` for more information.

  #. Specify one or more **Entities** to find mirrors for by clicking on parts or surfaces in the :term:`graphics window<Graphics window>` or :term:`parts list<Parts list>`.
  #. Select a **Mirror plane** to mirror about by clicking on construction planes or faces in the :term:`graphics window<Graphics window>` or :term:`feature tree<Feature tree>`.
  #. The Assembly mirror feature will automatically try each possible transform type (**Linear**, **Z axis**, **Y axis**, **X axis**, and **Mirror**) for each part and select the one that matches a part to its mirror image.

    If a valid transform is found, the transform type of the part will be updated with the valid transform, a mirror image of the part will be shown in blue in the :term:`graphics window<Graphics window>`, and a mate connector which can be used to assemble the part in the location of its mirror image will be created.

    Otherwise, the transform type of the part will be changed to **Mirror**, and a mirror copy of the part will be created.

    .. warning::
        The Assembly mirror feature can only set transform types automatically for parts. For other types of entities, like surfaces and edges, the transform type will always default to **Mirror** and will need to be updated manually.

    .. tip::
        The transform type will only be computed automatically when a feature is first selected. If you make changes to the part later on, you might need to update the transform type manually.

Steps for assembling mirrored parts
-----------------------------------

Steps for creating mirrored parts using preselections
-----------------------------------------------------
#. Before creating an Assembly mirror feature:

    * Pre-select a **Mirror plane** and one or more **Entities** to mirror by either:

        * Selecting entities directly from the feature tree or parts list
        * Selecting geometry (edges, faces, or vertices) in the :term:`graphics window<Graphics window>` which touch the entities you'd like to use


#. Create an Assembly mirror feature by selecting it from your :term:`FeatureScript dropdown`.
#. The **Entities** and **Mirror plane** parameters are filled in automatically according to your preselections.
#. Add and modify additional parameters as needed.

.. tip::
    Several native Onshape features also support preselections. For example, the Onshape construction plane feature will automatically switch to
    line-angle mode if you click a plane and a line before choosing the construction plane feature in your toolbar.



Transform types
---------------

There are five possible transform types:
* **Linear**

A direct linear shift across the mirror plane.

* **Z axis**

A linear shift plus a 180 degree rotation about the world z-axis.

* **Y axis**

A linear shift plus a 180 degree rotation about the world y-axis.

* **X axis**

A linear shift plus a 180 degree rotation about the world x-axis.

* **Mirror**

A standard mirror operation.

.. _result-behavior:

Result behavior
---------------
Assembly mirror offers two options for locating mirrored parts; **Part center** and **Origin**.

* **Part center**: Mate connectors are created such that mirrors are aligned when their center mate connectors are fastened together.
* **Origin**: Mate connectors are located relative to the world origin, so mirrors are aligned when their mate connector is fastened to the part studio origin. To assist with this, care should be taken that the assembly origin matches the part studio origin.

Copy part names
---------------

.. warning::
    Manually changing any property on a part which has been set by a FeatureScript, like color, material, or name, will shadow the FeatureScript applied 
    property until all properties on the part are reset.

.. tip::
    Part names are saved automatically when a part is first selected. If you change the original part name later, you can re-select the part
    in the Assembly mirror feature so the mirrored version of that part will also reflect the new name.