# Custom 404 Error Page Configuration

## Objective

Replace Apache's default 404 Not Found page with a custom branded error page.

## Error Page Location

Server Path:

/var/www/html/error_404.html

Repository Path:

error-pages/error_404.html

## Apache Configuration

Directive added in httpd.conf:

ErrorDocument 404 /error_404.html

## Verification

Test URL:

https://dhruvmishra.co.in/test

Expected Result:

Custom error page is displayed instead of Apache's default 404 page.

## Benefits

* Improved user experience
* Professional appearance
* Website branding consistency
* Easy navigation back to homepage

## Files Added

* error-pages/error_404.html
* error-pages/error-pages.md

## Apache Command Used

Reload configuration:

sudo systemctl reload httpd

Verify service:

sudo systemctl status httpd

