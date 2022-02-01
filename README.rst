=================================
Welcome to NS-REL-IMPORTS's docs!
=================================


Simple rel import generator module
==================================

Generates Realitive info with a camel to snake conversion of class name.

.... code-block:: python

    >>> obj_str = 'awt.uno.XInterface'
    >>> ns = 'dyn.awt.grid'
    >>> rel = RelInfo.get_rel_import(in_str =obj_str, ns=ns)
    >>> print(f"from {rel.frm} import {rel.imp}")
    from ....awt.uno.x_interface import XInterface

