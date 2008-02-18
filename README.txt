/**
 * unique_field: Unique field module for Drupal
 * by Joe Turgeon (http://arithmetric.com)
 * version 02/18/2008
 * licensed under the GPL version 2
 */

unique_field provides a way to require that node titles or CCK fields are
given unique values.

This module adds additional options to the content type administration page
for specifying which fields must be unique. The administrator may specify
whether each field must be unique or whether the fields in combination must
be unique.

It has been tested with the integer and text fields from CCK-5.x-1.6-1,
the date field from Date 5.x-1.8, the name fields from cck_fullname-5.x-1.5,
and the e-mail field from email-5.x-1.x.

This does not work well with the 'decimal' field in the CCK 5.x releases, 
due to a problem with the floating point datatype used. (However, this is
fixed in the CCK 6.x release: http://drupal.org/node/109246)

Please send comments and suggestions to Joe: arithmetric at gmail.com

