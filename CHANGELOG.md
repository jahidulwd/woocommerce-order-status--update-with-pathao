## 2.2.3 — Location preload reliability fix

- Fixed nested Pathao API response parsing for city, zone, and area preload requests.
- Added validation for empty or unexpected API responses and surfaced actionable error messages in the preload progress UI.
- Corrected bulk zone and area grouping to use Pathao `zone_id`, `zone_name`, `area_id`, and `area_name` fields where provided.

# Changelog

## 2.2.2 — Author credit and admin UI refinement

- Updated the WordPress plugin author to Jahidul Islam.
- Retained explicit original plugin and Pathao API integration credit to Pathao in the documentation.
- Fixed the Refresh merchant info icon/label alignment using an inline-flex button layout.
- Added a spinning refresh icon while merchant information is loading.


## 2.2.0 — WooCommerce Auto Order Status Sync enhancement

- Added webhook-driven WooCommerce order status synchronization.
- Pathao Delivered → WooCommerce Completed.
- Pathao Returned/Return, Partial Delivery, Delivery Failed, Pickup Cancelled, and On Hold → WooCommerce On hold by default.
- Other courier states, including Picked and In Transit, do not change the WooCommerce order status by default.
- Saves Pathao status, delivery fee, and consignment ID via the WooCommerce order object.
- Adds an order note when an automatic WooCommerce status change is made.
- Added the `ptc_wc_order_status_map` filter for developer customization.
- Enhancement and documentation credit: Jahidul Islam. Original plugin credit remains with Pathao.

## Compatibility and testing note

PHP syntax checks passed for the modified plugin PHP files. The webhook-to-status workflow still needs to be tested on a staging WooCommerce site using a real Pathao webhook and matching webhook secret before production use.
