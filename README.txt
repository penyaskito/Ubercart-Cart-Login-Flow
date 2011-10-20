Background
==========
Ubercart (http://drupal.org/project/ubercart) is an ecommerce solution based on Drupal.

The default Ubercart cart behavior is merging the anonymous cart and the existing user cart 
once the user logs in.

This can be confusing for users because their cart could have some products added long ago, 
and when they log in, the old existing cart and the new anonymous cart are merged.

Description
==========
This module provides different behaviors, depending on the source of the user when logs in:

* If the users log in while at the checkout page, the old existing cart is discarded, 
and the new cart that has been created while the user is anonymous will be checked out.

* If the users log in other cases, we discard the anonymous cart and recover the previously 
existing cart that was associated with this user.

Dependencies
============

* Ubercart: uc_cart must be enabled.

Installation
============
Download the module and enable it. The installation takes care of setting the weight of 
the module to a lower value than uc_cart has, but if you manually edit the weights, 
please take this into account.

Attribution
===========
Development sponsored by Emergya
