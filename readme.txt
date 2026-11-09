=== Pathao Courier Plugin For WordPress Woocommerce ===
Contributors: jahidul-islam
Tags: courier, pathao, pathao courier, pathao courier plugin, pathao plugin, pathao woocommerce, pathao woocommerce plugin, pathao wordpress, pathao wordpress plugin, pathao wordpress woocommerce
Requires at least: 6.0
Tested up to: 6.4
Requires PHP: 7.0
Stable tag: 2.2.3
License: GPLv3
License URI: https://www.gnu.org/licenses/gpl-3.0.html

== Description ==
Pathao Courier Plugin For WordPress Woocommerce is a WordPress plugin which is designed to enhance your website's functionality by providing courier service features.
Whether you need seamless package tracking or a user-friendly way to manage deliveries, our plugin has you covered.

== Features ==
- Easy to implement
- Sync orders to the Pathao Merchant Panel
- Webhook Implementations
- Realtime order status updates
- Bulk Order Creation
- WooCommerce Auto Order Status Sync: Delivered -> Completed; Returned, Partial Delivery, Delivery Failed, Pickup Cancelled -> On hold.
- Saves Pathao status, delivery fee, and consignment ID to the WooCommerce order.
- Adds an order note when an automatic WooCommerce status change occurs.
- Customizable status mapping via ptc_wc_order_status_map filter.

== Screenshots ==
1. Installation
2. Settings
3. Add Client ID and Client Secret from Pathao Courier Merchant Panel
4. Save Settings
5. Place Order
6. Go woocommerce orders
7. Click Send with Pathao
8. Add Receiver Name, Receiver Phone Number, Receiver Address, Receiver City and others necessary information
9. Click Send with Pathao Courier
10. Preload City, Zone & Area (Settings)
11. Bulk Order Modal Preload Prompt
12. Bulk Order Modal Grid View

== Enhancement Credits ==
Original plugin by Pathao. WooCommerce Auto Order Status Sync enhancement and documentation by Jahidul Islam (https://bd.linkedin.com/in/jahidulwd).

== Changelog ==
= 2.2.3 =
* Fixed Pathao city, zone, and area preload response parsing across WordPress AJAX and Pathao API response wrappers.
* Added explicit API/preload error messages instead of leaving progress at 0%.
* Improved zone and area field mapping using Pathao zone_id/zone_name and area_id/area_name fields.
= 2.2.2 =
* Updated plugin author credit to Jahidul Islam with LinkedIn author profile; retained original plugin credit to Pathao.
* Fixed Refresh merchant info button icon alignment and added a loading spin state.

= 2.2.0 =
* Added automatic WooCommerce order status synchronization from Pathao webhooks.
* Delivered maps to Completed. Returned, Partial Delivery, Delivery Failed, Pickup Cancelled, and On Hold map to On hold by default.
* Saves courier metadata through the WooCommerce order object and adds an order note for automatic status changes.
* Added ptc_wc_order_status_map developer filter and documentation.
