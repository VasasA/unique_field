/**
 * unique_field: Unique field module for Drupal
 *
 * By Joe Turgeon [http://arithmetric.com]
 * Version 2008/10/24
 * Licensed under the GPL version 2
 */

The unique field module provides a way to require that node titles or 
CCK fields are given unique values.

Without this module, Drupal and CCK do not prevent multiple nodes from 
having the same title or the same value in a given field.

For example, if you have a custom content type with a Date field and there 
should only be one node per date, you could use this module to prevent a 
node from being saved with a date already used in another node.

This module adds additional options to the content type administration page
for specifying which fields must be unique. The administrator may specify
whether each field must be unique or whether the fields in combination must
be unique. Also, the administrator can choose whether the fields must be 
unique among all other nodes or only among nodes from the given node's 
content type.

Alternatively, you can select the 'single node' scope, which allows you 
to require that the specified fields are each unique on that node. For 
example, if a node has multiple, separate user reference fields, this 
setting will require that no user is selected more than once on one node.

This module has been tested with the integer, text, node and user reference 
fields from CCK-5.x-1.9, the date field from Date 5.x-1.8, the name fields 
from cck_fullname-5.x-1.5, and the e-mail field from email-5.x-1.x.

This does not work well with the 'decimal' field in the CCK 5.x releases, 
due to a problem with the floating point datatype used. (However, this is
fixed in the CCK 6.x release: http://drupal.org/node/109246)

Thanks to fago and his excellent auto_nodetitle module.

This module's development has been sponsored by:
-- Sundays Energy [http://sundaysenergy.com]
-- Icelink Design [http://icelinkdesign.net]

Please send comments and suggestions to Joe Turgeon (detour) at
arithmetric @ gmail.com

