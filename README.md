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
wp_lang
comment_author_
comment_author_url_
comment_author_email_
```
**Bacaan lebih lanjut:** https://developer.wordpress.org/advanced-administration/wordpress/cookies/

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
_wc_session_
```
**Bacaan lebih lanjut:** https://developer.woocommerce.com/docs/best-practices/performance/configuring-caching-plugins/

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
edd_cart_fees
edd_cart_messages
edd_cart_token
edd_items_in_cart
edd_purchase
edd_resume_payment
edd_saved_cart
edd_session_*
preset_discount
cart_discounts
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
