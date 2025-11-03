====================
Comments and chatter
====================

Odoo Spreadsheet offers two ways to communicate with other users who have access to the same
spreadsheet, namely by using:

- :ref:`comments <spreadsheet/collaboration/comments>`
- the spreadsheet's :ref:`chatter thread <spreadsheet/collaboration/chatter>`

.. _spreadsheet/collaboration/comments:

Use comments in a spreadsheet
=============================

Comments, which are added to individual spreadsheet cells, are useful for discussing specific
elements of a spreadsheet. Other collaborators can be notified by typing `@` followed by their
name.

.. important::
   Only the spreadsheet's owner or users with :guilabel:`Editor` rights can use comments in a
   spreadsheet; both roles can perform the same actions. Comments are not visible to users with
   :guilabel:`Viewer` rights.

.. _spreadsheet/collaboration/comments-add-react:

Add or react to comments
------------------------

To add or react to a comment:

#. If the comment is:

   - the first comment being added to the cell, right-click the cell then click :icon:`os-comments`
     :guilabel:`Insert comment` or click :menuselection:`Insert -->` :icon:`os-comments`
     :menuselection:`Insert comment` from the menu bar.
   - a reaction to an existing comment thread on a cell, click on the relevant cell or on the
     comment thread to open the thread.

#. Type a comment in the text box.

   .. tip::
      Type `@` to tag users, or add emojis or GIFs by clicking :icon:`oi-smile-add` :guilabel:`Add a
      Reaction`.

#. Click :guilabel:`Send` or press `Ctrl` + `Enter`.

Click anywhere else in the spreadsheet to close the comment thread.

.. tip::
   To react to an individual comment with only an emoji, hover over the comment, click the
   :icon:`oi-smile-add` :guilabel:`(Add a Reaction)` icon, then select the desired emoji.

.. _spreadsheet/collaboration/comments-view:

View comments
-------------

When a comment has been added to a cell, a small yellow triangle appears in the top right corner of
the cell.

To view a comment thread on a single cell hover over the cell; click the cell or the comment
thread to open the thread to be able to add a comment.

To view all comments on a spreadsheet, click :menuselection:`View -->` :icon:`os-comments`
:menuselection:`All comments` from the menu bar. Alternatively, after opening a comment thread,
click :guilabel:`Open all comments`.

The :guilabel:`Comments` panel opens on the right side of the spreadsheet. By default, comment
threads for :guilabel:`All sheets` of the spreadsheet are shown, grouped by sheet. To see only the
comment threads for the current sheet, select :guilabel:`This sheet` in the :guilabel:`Filter
comments` field.

Click on a comment thread in the :guilabel:`Comments` panel to open it.

.. _spreadsheet/collaboration/comments-edit-delete:

Edit or delete comments
-----------------------

.. note::
   A spreadsheet's owner or users with :guilabel:`Editor` rights can edit or delete any comment.

To edit a comment:

#. Hover over the comment then click the :icon:`fa-ellipsis-v` :guilabel:`(ellipsis)` icon.
#. Click :icon:`fa-pencil` :guilabel:`Edit`.
#. Make the desired changes then click :guilabel:`Save` or press `Enter`. To abort the edit, click
   :guilabel:`Cancel` or press `Escape`.

.. tip::
   A comment that has been modified has *(edited)* added to the end of the text.

To delete a comment:

#. Hover over the comment then click the :icon:`fa-ellipsis-v` :guilabel:`(ellipsis)` icon.
#. Click :icon:`fa-trash` :guilabel:`Delete`.
#. Click :guilabel:`Confirm` to confirm the deletion.

.. _spreadsheet/collaboration/comments-resolve:

Resolve comment threads
-----------------------

To resolve a comment thread:

#. Access the :guilabel:`Comments` panel by clicking :menuselection:`View -->` :icon:`os-comments`
   :menuselection:`All comments` from the menu bar. Alternatively, with a comment thread open, click
   :guilabel:`Open all comments`.
#. Click the :icon:`fa-ellipsis-v` :guilabel:`(ellipsis)` icon for the relevant comment thread then
   click :guilabel:`Resolve this thread`.

Once resolved, the comment thread is no longer accessible directly on the spreadsheet, but remains
visible in the :guilabel:`Comments` panel; resolved threads are identified by a :icon:`fa-check`
:guilabel:`(check)` icon.

To reopen a resolved comment thread, from the :guilabel:`Comments` panel, click the
:icon:`fa-ellipsis-v` :guilabel:`(ellipsis)` icon for the relevant comment thread then click
:guilabel:`Re-open this thread`.

.. _spreadsheet/collaboration/chatter:

Use a spreadsheet's chatter thread
==================================

Whereas :ref:`comments <spreadsheet/collaboration/comments>` on specific spreadsheet cells are
suited for discussions about specific elements of a spreadsheet, a spreadsheet’s :doc:`chatter
thread <../../discuss/chatter>` allows for a more general discussion.

To access the chatter thread of a spreadsheet:

#. With the **Documents** app open, navigate to the folder or section where the spreadsheet is
   saved.
#. Select the :icon:`oi-view-list` :guilabel:`(List)` view in the upper-right corner.
#. Select the relevant spreadsheet, then click the :icon:`fa-info-circle` :guilabel:`(Info & tags)`
   button in the upper-right corner next to the view selector. Alternatively, with the spreadsheet
   selected, click the :icon:`fa-cog` :guilabel:`Action` button then select :icon:`fa-info-circle`
   :guilabel:`(Info & tags)`.

The spreadsheet’s chatter thread opens on the right of the screen, below the spreadsheet's
:ref:`details panel <documents/details-panel>`.
