# 📱 React Native বাংলা চিটশিট (বেসিক + অ্যাডভান্স)

> **React Native** — JavaScript/TypeScript দিয়ে iOS, Android এবং Web অ্যাপ একসাথে তৈরি করার ফ্রেমওয়ার্ক।

---

## 1. 🚀 সেটআপ (Expo CLI / React Native CLI)
**Expo CLI** → নতুনদের জন্য সহজ, অনেক বিল্ট-ইন API।  
**React Native CLI** → কাস্টম নেটিভ মডিউল দরকার হলে বেস্ট।

```bash
npm install -g expo-cli
expo init MyApp
cd MyApp
npm start
```

---

## 2. 🧩 Core Components
| Component | কাজ |
|-----------|------|
| **View** | UI layout container |
| **Text** | টেক্সট দেখায় |
| **Image** | ছবি দেখায় |
| **ScrollView** | স্ক্রলযোগ্য কন্টেইনার |
| **FlatList** | বড় ডাটা রেন্ডারের জন্য |
| **TouchableOpacity** | টাচ ইফেক্ট সহ বাটন |

---

## 3. 🎨 Styling
```jsx
const styles = {
  container: {
    flex: 1,
    alignItems: 'center',
    justifyContent: 'center',
  },
};
```
- CamelCase ব্যবহার করতে হবে।
- ইউনিট → dp (Density-independent Pixels)।

---

## 4. 📏 Flexbox Layout
```jsx
<View style={{ flex: 1, flexDirection: 'row', justifyContent: 'center', alignItems: 'center' }} />
```
- **flexDirection:** row / column  
- **justifyContent:** main axis alignment  
- **alignItems:** cross axis alignment  

---

## 5. 📦 Props & State
```jsx
const Greeting = ({ name }) => <Text>Hello, {name}</Text>;
```
```jsx
const [count, setCount] = useState(0);
```

---

## 6. 🛠 Event Handling
```jsx
<Button title="Press Me" onPress={() => alert('Clicked')} />
```

---

## 7. 📃 Lists
**FlatList** / **SectionList** → Lazy loading সহ।

---

## 8. 🧭 Navigation
- `@react-navigation/native`
- `@react-navigation/native-stack`

---

## 9. 🌐 Networking
**fetch / axios**
```jsx
axios.get('/api/data').then(res => setData(res.data));
```

---

## 10. 📱 Platform Specific
```jsx
if (Platform.OS === 'ios') { ... }
```

---

## 11. 🎭 Animations
- `Animated`
- `react-native-reanimated`
- `moti`

---

## 12. 🪝 Hooks
`useState`, `useEffect`, `useRef`, `useCallback`, `useMemo`

---

## 13. 📦 Third-Party Libraries
- axios
- react-query / tanstack-query
- Zustand / Redux Toolkit

---

## 14. 🔍 Debugging
- Flipper
- React Native Debugger

---

## 15. 🛠 Commands
```bash
npm start
npm run android
npm run ios
```

---

## 16. 📝 TypeScript
Type Safety → কম বাগ।

---

## 17. 🧪 Testing
- Jest
- React Native Testing Library
- Detox (E2E Testing)

---

## 18. ♿ Accessibility
`accessible`, `accessibilityLabel`

---

## 19. 🔑 Permissions
- `PermissionsAndroid`
- `react-native-permissions`

---

## 20. 📲 Device APIs
- Geolocation
- Camera Roll
- Clipboard
- Push Notifications

---

## 21. 💾 Offline Storage
- AsyncStorage
- MMKV (Fast key-value storage)
- SQLite / WatermelonDB / RealmDB

---

## 22. ⚡ Performance Optimization
- `React.memo`
- `useCallback`
- Avoid inline functions
- Remove unnecessary re-renders
- VirtualizedList optimization
- Lazy load heavy screens

---

## 23. 🌍 Internationalization (i18n)
`react-native-localize` + `i18n-js`

---

## 24. 🚧 Error Handling
- Error Boundaries
- try-catch in async calls
- Sentry / Bugsnag for crash reporting

---

## 25. 🏗 Architecture Best Practices
```
src/
 ├─ components/
 ├─ screens/
 ├─ navigation/
 ├─ hooks/
 ├─ services/
 ├─ store/
 ├─ utils/
```
- Use feature-based folder structure  
- Keep UI + Logic separate  
- API calls in services layer  

---

## 26. 🔐 Security in React Native
- Never store sensitive data in AsyncStorage → use `react-native-keychain`
- Use HTTPS always
- Secure API keys via backend
- Enable Proguard (Android)
- iOS App Transport Security

---

## 27. 📦 State Management (Advanced)
- Redux Toolkit
- Zustand
- Recoil
- MobX

---

## 28. 📡 Realtime Features
- WebSockets (`socket.io-client`)
- Firebase Realtime Database
- Pusher

---

## 29. 🚀 Deployment
**Android (APK / AAB)**  
```bash
expo build:android
```
**iOS (IPA)**  
```bash
expo build:ios
```

---

## 30. 🛡 Offline-First Apps
- Cache API responses with react-query
- Store data locally with WatermelonDB

---

## 31. 🏎 Advanced Performance Tools
- Hermes Engine (JS engine for faster startup)
- Code Push for OTA updates
- Bundle splitting

---

## 32. 🖥 React Web vs React Native Quick Compare

| Feature | React Web | React Native |
|---------|-----------|--------------|
| UI | HTML Tags | RN Core Components |
| Styling | CSS | StyleSheet / JS Object |
| Routing | react-router | React Navigation |
| Deployment | Web Server | App Store / Play Store |
| Animations | CSS / Framer Motion | Animated API / Reanimated |
| Device API | Limited | Full Native Access |
