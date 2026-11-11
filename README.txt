AFRAH MAKKAH SALES BRIEF - UPLOAD PACKAGE
=========================================

FILES (upload all three into one folder, e.g. /afrah-makkah/)
  index.html       The full page. Everything is built in: images, fonts, map, scripts.
  share-image.jpg  Preview picture used when the link is shared on WhatsApp, X, LinkedIn etc.
  favicon.png      Small Madain icon shown in the browser tab.

STEPS
1. Upload the folder to your web server or hosting (cPanel File Manager, FTP/SFTP,
   Netlify, Vercel, Cloudflare Pages, S3, etc.). It is a plain static page:
   no database, PHP, Node or build step needed.
2. Make sure the site runs on HTTPS (needed for the live map to load reliably).
3. Open index.html in a text editor and replace YOUR-DOMAIN in these two lines with
   your real address, e.g. https://madain.sa/afrah-makkah/ :
     <meta property="og:image" content="https://YOUR-DOMAIN/afrah-makkah/share-image.jpg"/>
     <meta property="og:url"   content="https://YOUR-DOMAIN/afrah-makkah/"/>
   (Share previews only work with full https addresses.)
4. Visit https://your-domain/afrah-makkah/ and check: both languages, the gallery,
   the price list filters, the payment plan, and the map.

RECOMMENDED SERVER SETTINGS (optional, for speed)
- The page is about 5.6 MB because all images are embedded. Turn on gzip or Brotli
  compression for .html files (most hosts have it on by default).
- Apache (.htaccess):
    AddOutputFilterByType DEFLATE text/html
    <FilesMatch "\.(jpg|png)$">Header set Cache-Control "max-age=604800"</FilesMatch>
- Nginx:
    gzip on; gzip_types text/html;

EXTERNAL SERVICES THE PAGE CALLS
- Map tiles: Esri World Street Map (server.arcgisonline.com). No key needed.
  Check Esri's terms of use for public/commercial websites; if you want to stay
  fully within free terms, ask and I can switch it to a static map only,
  or to Google Maps (needs your Google Maps API key).
- If the map service ever fails, a built-in map picture shows instead.
- "Register interest" buttons link to https://www.takwine.com.sa/registerinterest
- "Open in Google Maps" links to https://maps.app.goo.gl/2R6Mc5xjt9G9jLJv6
No cookies, tracking or analytics are included. Add your own (e.g. Google Analytics)
before </head> if you want visitor stats.

BEFORE GOING PUBLIC
- The Wafi off-plan sales licence number is not shown yet (pending). Confirm you are
  allowed to advertise publicly before the licence is issued.
- Unit availability: only T2-R-B and T2-R-C are marked Sold. Update before launch.
- Prices follow the price list provided on 11 Nov 2026.
