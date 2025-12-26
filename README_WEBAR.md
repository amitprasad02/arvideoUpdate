# WebAR Camera Troubleshooting Guide

## Common Camera Issues and Solutions

### "Cannot access camera" Error

This error typically occurs due to browser permissions, security settings, or device compatibility issues.

### Quick Fixes

1. **Check Browser Permissions**
   - Click the camera icon in your browser's address bar
   - Allow camera access for this site
   - Reload the page

2. **Use HTTPS**
   - Camera access requires a secure connection (HTTPS)
   - If testing locally, use `localhost` or `127.0.0.1`
   - For remote testing, use HTTPS or tools like ngrok

3. **Try Different Browsers**
   - **Recommended:** Chrome on Android, Safari on iOS
   - **Desktop:** Latest Chrome, Firefox, or Edge
   - **Avoid:** In-app browsers (Facebook, Instagram, etc.)

4. **Check Device Camera**
   - Ensure your camera is working in other apps
   - Close other applications using the camera
   - Try switching between front/back cameras

### Browser-Specific Solutions

#### Chrome
- Go to Settings > Privacy and Security > Site Settings > Camera
- Ensure the site is allowed to use camera
- Clear browser cache and cookies

#### Safari (iOS)
- Settings > Safari > Camera > Allow
- Ensure iOS is updated to latest version
- Try refreshing the page

#### Firefox
- Click the shield icon in address bar
- Allow camera permissions
- Check about:config for media.navigator.enabled

### Mobile Device Issues

#### Android
- Check if Chrome has camera permissions in Android Settings
- Ensure you're not in an in-app browser
- Try opening the link in Chrome directly

#### iOS
- Use Safari browser (recommended)
- Check iOS Settings > Safari > Camera permissions
- Ensure iOS version supports WebRTC

### Advanced Troubleshooting

1. **Check Console Errors**
   - Open browser developer tools (F12)
   - Look for camera-related errors in console
   - Share error messages for further help

2. **Test Camera Access**
   - Visit https://webrtc.github.io/samples/src/content/getusermedia/gum/
   - If this doesn't work, the issue is with your browser/device setup

3. **Network Issues**
   - Ensure stable internet connection
   - Try different network (mobile data vs WiFi)
   - Check if corporate firewall blocks camera access

### Still Having Issues?

If none of these solutions work:

1. Copy the diagnostic information from the app
2. Note your browser version and device type
3. Check the browser console for error messages
4. Try the camera test link mentioned above

### Supported Configurations

- **Mobile:** Chrome on Android 7+, Safari on iOS 11+
- **Desktop:** Chrome 60+, Firefox 55+, Safari 11+, Edge 79+
- **Requirements:** HTTPS or localhost, camera permissions granted

### Security Notes

- Camera access requires user permission
- Only works on secure contexts (HTTPS/localhost)
- Some corporate networks may block camera access
- In-app browsers often restrict camera functionality