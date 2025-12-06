Enviro Inventory Android App (API-ready)
---------------------------------------
This Android Studio project is configured to call your API at:
http://192.168.1.103/public/api/

Steps to build APK:
1. Open this project in Android Studio.
2. Let Gradle sync and download dependencies.
3. Connect an Android device (USB debugging) or use emulator.
4. Build -> Build Bundle(s) / APK(s) -> Build APK(s).
5. Install the generated APK on device and run.

Notes:
- API endpoints used:
    http://192.168.1.103/public/api/scan.php?barcode=CODE
    http://192.168.1.103/public/api/add_stock.php (POST barcode, qty)
    http://192.168.1.103/public/api/remove_stock.php (POST barcode, qty)
- Ensure your API is reachable from the Android device (same LAN).
- If your API requires authentication, update ApiClient.kt accordingly.
