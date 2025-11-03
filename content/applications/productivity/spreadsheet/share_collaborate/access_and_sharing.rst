==================
Access and sharing
==================

In principle, the rights to access Odoo spreadsheets are handled like :ref:`any other file in the
Documents app <documents/access-rights>`. :ref:`Roles and permissions
<spreadsheet/collaboration/roles-permissions>` are either inherited from the folder a spreadsheet is
saved in or controlled at the level of the spreadsheet itself.

However, there are important differences to consider between :ref:`spreadsheets that contain only
static data <spreadsheet/collaboration/static-spreadsheet>` and :ref:`spreadsheets that contain
dynamic Odoo data <spreadsheet/collaboration/dynamic-spreadsheet>`, in terms of both access and data
visibility.

.. tip::

   - Access to a folder or spreadsheet can be managed by its owner or any user with
     :guilabel:`Editor` rights.
   - A user with :guilabel:`Viewer` rights cannot share a spreadsheet with a specific user
     directly, but can copy a link to the spreadsheet.
   - Any user with access to a spreadsheet can download it as an `.xlsx` file by clicking
     :menuselection:`File -->` :icon:`os-download` :menuselection:`Download`  from the menu bar. If
     the spreadsheet contained dynamic data, the values are frozen at the moment of download.

.. _spreadsheet/collaboration/roles-permissions:

Roles and permissions
=====================

Permissions are managed using the following roles:

.. list-table::
   :header-rows: 1
   :stub-columns: 1
   :widths: 5 5 5 5 5 5 5 5 5

   * - Role
     - View
     - Edit
     - Delete
     - Download .xlsx
     - Share
     - Manage roles
     - Use comments
     - Use chatter
   * - Owner
     - :icon:`fa-check`
     - :icon:`fa-check`
     - :icon:`fa-check`
     - :icon:`fa-check`
     - :icon:`fa-check` with specific people or via link
     - :icon:`fa-check` including changing owner
     - :icon:`fa-check`
     - :icon:`fa-check`
   * - Editor
     - :icon:`fa-check`
     - :icon:`fa-check`
     - :icon:`fa-check`
     - :icon:`fa-check`
     - :icon:`fa-check` with specific people or via link
     - :icon:`fa-check` but cannot change owner
     - :icon:`fa-check`
     - :icon:`fa-check`
   * - Viewer
     - :icon:`fa-check`
     - :icon:`oi-close`
     - :icon:`oi-close`
     - :icon:`fa-check`
     - :icon:`fa-check` only via link
     - :icon:`oi-close`
     - :icon:`oi-close`
     - :icon:`fa-check`

.. _spreadsheet/collaboration/static-spreadsheet:

Share a static spreadsheet
==========================

Spreadsheets containing only static data can be shared internally or externally by the owner of the
spreadsheet or any user with :guilabel:`Editor` rights.

To do so, click :icon:`fa-share-alt` :guilabel:`Share` in the upper-right corner above the
spreadsheet, then :ref:`configure access as appropriate <documents/access-rights>`.

.. _spreadsheet/collaboration/dynamic-spreadsheet:

Share a dynamic spreadsheet
===========================

A spreadsheet is considered a *dynamic spreadsheet* if it contains any of the following:

- formulas that retrieve live data from an Odoo database, e.g., in a :doc:`list or pivot table that
  has been inserted into the spreadsheet <../insert>`
- a linked :ref:`data source <spreadsheet/insert/data-sources>`, even if the corresponding list or
  pivot table has been deleted from the spreadsheet
- links to Odoo menu items

Internal sharing
----------------

Spreadsheets containing dynamic Odoo data can be shared *with internal users only* by the owner of
the spreadsheet or any user with :guilabel:`Editor` rights.

However, having access to a spreadsheet does not necessarily mean an internal user *sees* all the
data in the original spreadsheet. The visibility of dynamic Odoo data is based on an internal user’s
access rights to the model from which the data has been retrieved, and takes into account any record
rules that may restrict access.

.. important::
   Permissions to view data are taken into account when an internal user opens a spreadsheet, with
   the spreadsheet only being populated with data the user is authorized to see.

  .. example::
     A sales manager creates a spreadsheet that includes sales data for all the salespeople in their
     team. Users with the permission `Sales / User: Own Documents Only` only see data related to
     their own sales.

To share a spreadsheet containing dynamic Odoo data, click :icon:`fa-share-alt` :guilabel:`Share` in
the upper-right corner above the spreadsheet, then :ref:`configure access as appropriate
<documents/access-rights>`.

External sharing
----------------

Spreadsheets containing dynamic Odoo data *cannot be accessed by external users*.

.. note::
   If an external user attempts to access a dynamic spreadsheet via a link, an error message is
   shown.

If a spreadsheet containing Odoo data needs to be shared with an external user, the owner of the
spreadsheet or a user with :guilabel:`Editor` rights can create a frozen, read-only version. In this
version, all Odoo formulas are converted to their value at the moment the frozen version is created,
and any links to Odoo menus are removed.

To create a frozen version of a spreadsheet that contains dynamic Odoo data, click
:icon:`fa-share-alt` :guilabel:`Freeze and share` in the upper-right corner above the spreadsheet,
then :ref:`configure access as appropriate <documents/access-rights>`.

.. tip::
   It is also possible to download a frozen version of a spreadsheet that contains Odoo data as an
   `.xlsx` file by clicking :menuselection:`File -->` :icon:`os-download` :menuselection:`Download`
   from the menu bar. The values of any dynamic data are frozen at the moment of download.
