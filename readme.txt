=== Password bcrypt ===
Contributors: szepe.viktor
Tags: password, hash, bcrypt
Requires at least: 4.4
Tested up to: 4.5.2
Stable tag: 1.0.2
License: GPLv2 or later
License URI: http://www.gnu.org/licenses/gpl-2.0.html

Replaces wp_hash_password and wp_check_password with PHP 5.5's password_hash and password_verify.

== Description ==

wp-password-bcrypt is a WordPress plugin to replace WP's outdated and insecure
MD5-based password hashing with the modern and secure [bcrypt](https://en.wikipedia.org/wiki/Bcrypt).

It is written by [roots.io people](https://roots.io/plugins/bcrypt-password/).

This plugin requires PHP >= 5.5.0 which introduced the built-in
[`password_hash`](http://php.net/manual/en/function.password-hash.php) and
[`password_verify`](http://php.net/manual/en/function.password-verify.php) functions.

See [Improving WordPress Password Security](https://roots.io/improving-wordpress-password-security/)
for more background on this plugin and the password hashing issue.

== Installation ==

1. Upload the plugin files to the `/wp-content/plugins/password-bcrypt` directory, or install the plugin through the WordPress plugins screen directly.
1. Activate the plugin through the 'Plugins' screen in WordPress

== Frequently Asked Questions ==

= Manual installation as a must-use plugin =

If you don't use Composer, you can manually copy `wp-password-bcrypt.php` into your `mu-plugins` folder.

We **do not** recommend using this as a normal (non-MU) plugin. It makes it too easy to disable or remove the plugin.

== Changelog ==

= 1.0.3 =
* Check for another password plugin.

= 1.0.2 =
* Added license file, excuse me.

= 1.0.1 =
* This is the WordPress-stlye version of the original [roots wp-password-bcrypt](https://github.com/roots/wp-password-bcrypt) plugin
