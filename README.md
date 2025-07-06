Bagi Anda yang menerapkan cache untuk meningkatkan kinerja WordPress, baik itu cache di tingkat aplikasi menggunakan plugin, page cache di tingkat server seperti Varnish, Nginx FastCGI, maupun cache di tingkat proxy seperti Cloudflare, berikut adalah daftar URI dan cookies yang sebaiknya tidak dicache.
## WordPress
**URI**
```
/wp-admin/
/wp-json/
/wp-login.php
/xmlrpc.php
(\?|&)preview=
wp-.*.php
index.php
```
**Cookies**
```
wordpress_
wordpress_no_cache
wordpress_logged_in_
wordpress_test_cookie
wordpress_[a-f0-9]+
wp-postpass
wp-settings-
comment_author_
comment_author_url_
comment_author_email_
```
**Bacaan lebih lanjut:**
https://developer.wordpress.org/advanced-administration/wordpress/cookies/

## WooCommerce
**URI**
```
/cart/
/addons/
/wc-api
/checkout/
/my-account/
```
**Cookies**
```
woocommerce_
woocommerce_cart_hash
wp_woocommerce_session_
woocommerce_items_in_cart
woocommerce_recently_viewed
store_notice[notice id]
```
**Bacaan lebih lanjut:**
https://developer.woo.com/docs/how-to-configure-caching-plugins-for-woocommerce/

## Easy Digital Download
**URI**
```
/edd-sl/
/edd-api
/checkout/
/purchase-confirmation/
```
**Cookies**
```
edd_cart
edd_purchase
edd_cart_fees
edd_saved_cart
edd_cart_token
edd_items_in_cart
edd_cart_messages
edd_resume_payment
cart_discounts
preset_discount
```
**Bacaan lebih lanjut:**
- https://easydigitaldownloads.com/docs/configure-cache/
- https://easydigitaldownloads.com/docs/cloudflare/

## Lainnya
**URI**
```
/feed/
robots.txt
sitemap.xml
sitemap(_index)?.xml
ao_noptirocket
ao_speedup_cachebuster
removed_item
```
**Cookies**
```
bookly
ec_
ecwid
jetpack
wpsc_
xf_
yith_wcwl_session_
yith_wrvp_
```
