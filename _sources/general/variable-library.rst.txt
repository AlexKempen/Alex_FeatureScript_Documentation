Variable library
================
The Variable library feature makes it possible to create and use global variables in Onshape by storing variables on cube parts. Variables may also have associated descriptions which can be viewed via a custom table.

The Variable library FeatureScript can be found here: `Variable library suite document <https://cad.onshape.com/documents/d33530b06909083111cf1770/w/5be0429e68b3332e158a3559/e/e4e782e0fe48a9227b9440aa>`_

Steps for using variable libraries
----------------------------------
#. Create a Variable library feature in a part studio.
#. Set the Variable library useage behavior to **Use**.
#. Click **Select Part Studio...**, then navigate to another part studio containing one or more library variable cubes and select them.
#. The variables attatched to those parts are automatically added to the part studio.
#. |confirm-feature|

Steps for creating variable libraries manually
----------------------------------------------
#. Create a Variable Library feature in a part studio.
#. Set the Variable library usage behavior to **Create**.
#. Set the library creation type to **Manual**.
#. Add one or more variables. A library cube part is created containing each added variable.
#. If desired, choose **Add descriptions**, then add descriptions to each variable in **Variables**.

.. seealso:: 
    :ref:`variable-descriptions` for more information.

#. |confirm-feature|

Steps for creating variable libraries from existing variables
-------------------------------------------------------------

.. note::
    It isn't currently possible to add custom variable descriptions when creating variable libraries this way.

#. Create a Variable library feature in a part studio with one or more existing variables.
#. Set the Variable library usage behavior to **Create**.
#. Set the library creation type to **Automatic**.
#. Specify a **Library name**.
#. A library cube part is created containing all ofthe variables currently visible to the variable library feature.
#. |confirm-feature|

.. image:: variableLibraryAutoUI.png
    :width: 40%
    :align: center

Steps for creating variable libraries from CSV files
----------------------------------------------------

#. Open the Variable Library Template, make a copy, and then edit it as desired.

The Variable Library Template can be found here:
`Variable Library Template <https://docs.google.com/spreadsheets/d/1k5xZ5Lqxz4xRqVlRQ4j5USSUi_MWBjeumz-F2teNtok/edit#gid=0>`_

#. Download the template file as a .csv (Comma Seperated Values) file, then upload it into Onshape.
#. #. Create a Variable library feature in a part studio in the same document as your uploaded CSV file.
#. Set the Variable library usage behavior to **Create**.
#. Set the library creation type to **Import**.
#. Select the **CSV file** you uploaded to Onshape.
#. If your CSV file has a top-level header row, select **Skip first row**.
#. The variable library feature should add one or more variable library cube parts to the part studio.
#. |confirm-feature|

.. _variable-descriptions:

Variable descriptions
---------------------

Descriptions can be added to manually created variables and to variables imported from CSV files. These descriptions can then be seen later on using a custom table.

To add and use the variable library custom table, you will need to first add it to your custom table tab.

#. Open the **Custom tables** panel by clicking on the corresponding button on the far right side of your screen.
#. Choose **Add custom table**, then copy and paste the following link into the search bar:

    `https://cad.onshape.com/documents/d33530b06909083111cf1770/w/5be0429e68b3332e158a3559/e/2ac1b130ef1d31461f8fca54 <https://cad.onshape.com/documents/d33530b06909083111cf1770/w/5be0429e68b3332e158a3559/e/2ac1b130ef1d31461f8fca54>`_

#. Open the resulting document and click **Library variables** to add it to your custom tables.
#. If your part studio has one or more variables from a library variable feature, they are displayed in a table format.
