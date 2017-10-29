=== WooCommerce Cancel Abandonned Order ===
Contributors: rvola
Donate link: https://www.paypal.me/rvola
Tags: woocommerce, cancel, order, pending, on hold, gateway
Requires PHP: 5.3
Requires at least: 4.0
Tested up to: 4.9
Stable tag: 1.0.0
License: GPLv3
License URI: https://www.gnu.org/licenses/gpl-3.0.html

Cancel "on hold" orders after a certain number of days

== Description ==

**WooCommerce Cancel Abandonned Order** allows you to add a small option that will take care of dealing with "abandoned" commands.

If you have check or transfer type orders for example, you will be able to set a maximum number of days to receive the payment.

WooCommerce Cancel Abandoned Order, will take care of checking this and change the status of the order to "Cancel" if you have not received payment on time.

[**GitHub**](https://github.com/rvola/woocommerce-cancel-abandonned-order) | [**Donate**](https://www.paypal.me/rvola)

== Installation ==

This section describes how to install the plugin and get it working.

1. Upload the plugin files to the `/wp-content/plugins/woocommerce-cancel-abandonned-order` directory, or install the plugin through the WordPress plugins screen directly.
1. Activate the plugin through the 'Plugins' screen in WordPress
1. By default you can control the orders on the payment gateways: Check and BACS. Go to the options of the payment pages on WooCommerce.
1. *To add another payment gateway, simply use the `woo_cao-gateways` filters*

== Requirement ==

* PHP minimal: **5.3**
* WordPress minimal: **4.0**
* WooCommerce minimal : **2.2.0**

== Hooks ==
* `woo_cao-gateways`/ Adds a payment gateway for the control.
* `woo_cao-default_days` / Default value of the number of days for order processing.

== Frequently Asked Questions ==

= What does the plugin do? =

Depending on the options on the payment gateway options page *(enabled or disabled, maximum number of days)*, the plugin will fetch every day at midnight, the "on hold" commands with the payment gateway type *(default Check, BACS)* and if the maximum number of days indicated and exceeded, the system will take care to update the status of the order.

= I want to make suggestions =
We’re glad you want to help us improve **WooCommerce Cancel Abandonned Order**!
The GIT repository is available here [https://github.com/rvola/woocommerce-cancel-abandonned-order](https://github.com/rvola/woocommerce-cancel-abandonned-order)

== Changelog ==

= 1.0.0 / 2017-10-29 =
* Launch