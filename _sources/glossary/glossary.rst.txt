.. This document creates a term glossary

Glossary
========

.. glossary::
    Graphics window
        The graphics window refers to the model window, where parts, sketches, and other entities can be seen and interacted with.

        .. image:: /images/graphicsWindow.png
            :width: 50%
            :align: center

    Editing logic
        Editing logic is a feature of some FeatureScripts which enables certain parameters to update dynamically as a user is creating or making changes to a feature.
        For example, creating an extrude which hits another part will result in the boolean operation of the extrude feature being set to **Add**, and the other part being added to the **Merge scope**.
    
    Feature
        A feature is a modeling tool which exists in part studios. Features are listed in the Feature list on the left side of your screen, and can represent an
        instance of a custom FeatureScript feature or a native Onshape feature (like the Onshape extrude feature).

    Feature dialog
        The term feature dialog refers to the menu that is shown when creating or editing a feature.

    Feature tree
        The list of features in a part studio which can be found on the left side of your screen.

    Parts list
        The list of all parts in a part studio. The parts list exists in the bottom left of your screen, underneath the feature tree.

    FeatureScript dropdown
        Your FeatureScript fropdown is a section of your part studio toolbar which is reserved for custom features you've added there.

    Manipulators
        Manipulators are a feature of some FeatureScripts which enable users to modify the behavior of features via selectable arrows and points in the graphics window.

    Preselections
        Preselections are a feature of some FeatureScripts which allow certain entities to be selected before a feature is created.
        For example, a plane and a line can be selected before creating a Construction plane feature to change the plane creation mode to **Line angle** automatically.