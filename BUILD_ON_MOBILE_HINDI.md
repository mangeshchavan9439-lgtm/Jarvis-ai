# मोबाइल से Jarvis APK बनाना (GitHub Actions)

1. इस ZIP को फोन में डाउनलोड करके Extract करें।
2. Chrome में https://github.com खोलें और अपने अकाउंट में Sign in करें (नया अकाउंट हो तो बनाएं)।
3. `+` > `New repository` चुनें। नाम `Jarvis` रखें, `Public` या `Private` चुनें, फिर `Create repository` दबाएं।
4. खाली repository में `uploading an existing file` चुनें।
5. Extract किए हुए `Jarvis_Full_OPPO_Android16` फ़ोल्डर के **अंदर की सभी फ़ाइलें और फ़ोल्डर** अपलोड करें। `.github` फ़ोल्डर भी ज़रूर शामिल करें। फ़ोल्डर को ZIP के रूप में अपलोड न करें।
6. नीचे `Commit changes` दबाएं।
7. Repository में `Actions` टैब खोलें। `Build Jarvis APK` workflow चुनें और `Run workflow` दबाएं (अगर build अपने-आप शुरू न हुआ हो)।
8. Build पूरा होने पर हरा check दिखेगा। Run खोलें, नीचे `Artifacts` में `Jarvis-debug-apk` डाउनलोड करें।
9. ZIP को Extract करें। `app-debug.apk` खोलकर Install करें। Android पूछे तो Chrome/Files को इस स्रोत से ऐप install करने की अनुमति दें।

नोट:
- यह cloud build है; फोन से ही काम होगा, लेकिन APK GitHub के सर्वर पर बनेगा।
- Debug APK Android के debug key से अपने-आप signed होता है। Play Store release के लिए अलग release signing की ज़रूरत होती है।
- GitHub अकाउंट ज़रूरी है। API key/AI endpoint सेट करना वैकल्पिक है।
