User & Development Guide
==========================

Usage in Editor
---------------

1. Open any text area using the TinyMCE editor in Moodle.
2. Select the text or paragraph you want to justify.
3. Click the **Justify** button on the toolbar.

Development & AMD Compilation
-----------------------------

When modifying files inside `amd/src/`:

1. Bump the version in `version.php`.
2. Compile AMD modules with Grunt at Moodle's root:

   .. code-block:: bash

      npx grunt amd --root=lib/editor/tiny/plugins/justify

3. Purge caches via CLI:

   .. code-block:: bash

      php admin/cli/purge_caches.php
