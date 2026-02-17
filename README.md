# ANDROID DEVELOPMENT - EXAM QUICK NOTES (THANGLISH)

---

## 2 MARK QUESTIONS

### 1. Broadcast Receiver enna?

**Definition:** Background la nadakura events-a listen panni respond panra component.

**Key Points:**
- SMS receive aachu, battery low aachu - indha maari system events-ku response panrum
- Background la run aagum
- Intent-a receive pannikum
- Example: Phone boot aanadhum automatic-a app start pannalam

**Simple Example:**
```java
public class MyReceiver extends BroadcastReceiver {
    public void onReceive(Context context, Intent intent) {
        Toast.makeText(context, "Event happened!", Toast.LENGTH_SHORT).show();
    }
}
```

---

### 2. Gradle enna Android development la?

**Definition:** Build automation tool - apk file create panna use panra tool.

**Key Points:**
- Dependencies manage panrum (library add pannuradhu)
- Code-a compile panni APK file-a create panrum
- Two types: Project level & App level
- build.gradle file la irukum

**Example:**
```gradle
dependencies {
    implementation 'androidx.appcompat:appcompat:1.6.1'
}
```

---

### 3. Mobile Application Development enna?

**Definition:** Mobile devices (smartphone, tablet) ku software/apps develop panradhu.

**Key Points:**
- Native apps: Android (Java/Kotlin), iOS (Swift)
- Cross-platform apps: Flutter, React Native
- Features: Touch interface, sensors, camera, GPS use pannalam
- Platforms: Android, iOS, Windows Phone

---

### 4. Android SDK enna?

**Definition:** Software Development Kit - Android apps develop panna venum resources ellam irukkura package.

**Key Points:**
- Tools, libraries, API ellamae idhu la irukum
- Different Android versions ku support
- Emulator, debugger, build tools included
- API level versions: 21, 28, 33, etc.

---

### 5. Event Handling in Android UI

**Definition:** User actions (click, touch, swipe) ku respond panra process.

**Key Points:**
- **Listener** use panni events-a capture pannurom
- Common events: onClick, onTouch, onLongClick
- Two methods: XML la or Java code la

**Example:**
```java
button.setOnClickListener(new View.OnClickListener() {
    public void onClick(View v) {
        // Click aacha button ku action
    }
});
```

---

### 6. CheckBox enna?

**Definition:** True/False (checked/unchecked) select panna use panra UI widget.

**Key Points:**
- Multiple options select pannalam
- Boolean value return panrum (true/false)
- OnCheckedChangeListener use pannurom

**XML:**
```xml
<CheckBox
    android:id="@+id/checkbox"
    android:text="Agree Terms"
    android:layout_width="wrap_content"
    android:layout_height="wrap_content" />
```

---

### 7. Spinner enna?

**Definition:** Dropdown list - multiple options la onnu select panna use panra widget.

**Key Points:**
- Drop-down menu maari work aagum
- Array or ArrayList la items store pannurom
- Adapter use panni data set pannurom

**XML:**
```xml
<Spinner
    android:id="@+id/spinner"
    android:layout_width="match_parent"
    android:layout_height="wrap_content" />
```

---

### 8. Event Handling in Android (detailed)

**Definition:** User interactions-a detect panni action execute panradhu.

**Types:**
1. **Click Events** - button press
2. **Touch Events** - screen touch
3. **Key Events** - hardware button press
4. **Focus Events** - field select aachu

**Listeners:**
- OnClickListener
- OnTouchListener
- OnLongClickListener

---

### 9. Fragment enna?

**Definition:** Activity kulla reusable UI portion - mini activity maari.

**Key Points:**
- Own lifecycle irukum
- Multiple fragments-a oru activity la use pannalam
- Tablets la side-by-side UI ku best
- FragmentManager use panni manage pannurom

**Example:**
```java
public class MyFragment extends Fragment {
    public View onCreateView(LayoutInflater inflater, ViewGroup container, Bundle savedInstanceState) {
        return inflater.inflate(R.layout.fragment_layout, container, false);
    }
}
```

---

### 10. onCreate() Method Purpose

**Definition:** Activity life la first-a call aagura method - initialization nadakkura place.

**Key Points:**
- Layout set pannurom (setContentView)
- Variables initialize pannurom
- UI components find pannurom (findViewById)
- Only once call aagum

**Example:**
```java
protected void onCreate(Bundle savedInstanceState) {
    super.onCreate(savedInstanceState);
    setContentView(R.layout.activity_main);
    // Initialization code
}
```

---

### 11. Android vs iOS - 2 Differences

| Feature | Android | iOS |
|---------|---------|-----|
| **Language** | Java, Kotlin | Swift, Objective-C |
| **Customization** | Romba customizable | Limited customization |

---

### 12. Android Runtime (ART) enna?

**Definition:** Android apps-a execute panra environment.

**Key Points:**
- APK file-a machine code-a convert panrum
- AOT (Ahead-of-Time) compilation use panrum
- Battery life & performance improve aagum
- Dalvik-ku replacement (old version)

---

### 13. Android Emulator enna?

**Definition:** Computer la Android phone maari run aagura virtual device.

**Key Points:**
- Testing ku use panrom
- Different Android versions test pannalam
- Different screen sizes try pannalam
- Real device illama testing possible

---

### 14. Activity enna Android la?

**Definition:** Screen with UI - user interact panna base component.

**Key Points:**
- Each screen = One activity
- Lifecycle methods irukum (onCreate, onStart, etc.)
- Intent use panni switch pannurom
- MainActivity - app start aagumbodhu first activity

---

### 15. XML Layout enna Android la?

**Definition:** UI design panna use panra markup language file.

**Key Points:**
- UI elements (Button, TextView, etc.) define pannurom
- res/layout folder la store aagum
- Java/Kotlin code la reference pannurom
- Design & logic separate-a irukum

**Example:**
```xml
<LinearLayout>
    <TextView android:text="Hello" />
    <Button android:text="Click" />
</LinearLayout>
```

---

### 16. Layout Managers - 2 Examples

1. **LinearLayout** - Vertical or horizontal-a arrange pannum
2. **RelativeLayout** - Relative position la arrange pannum

---

### 17. Linear Layout enna?

**Definition:** Components-a oru line la (vertical/horizontal) arrange panra layout.

**Key Points:**
- **Orientation:** vertical or horizontal
- Simple & straightforward
- Weight property use panni space distribute pannalam

**XML:**
```xml
<LinearLayout
    android:orientation="vertical"
    android:layout_width="match_parent"
    android:layout_height="match_parent">
    <Button android:text="Button 1" />
    <Button android:text="Button 2" />
</LinearLayout>
```

---

### 18. Relative Layout Position UI Components

**Definition:** Components-a mathavanga ku relative-a position set panradhu.

**Key Points:**
- **Relative to parent:** centerInParent, alignParentTop
- **Relative to sibling:** toRightOf, below, above
- Flexible positioning
- Complex UI ku best

**Example:**
```xml
<RelativeLayout>
    <Button android:id="@+id/btn1"
        android:layout_alignParentTop="true" />
    <Button android:id="@+id/btn2"
        android:layout_below="@id/btn1" />
</RelativeLayout>
```

---

### 19. Implicit Intent Example Use Case

**Definition:** Specific component specify pannama action request panradhu.

**Example Use Cases:**
- **Browser open panradhu:**
```java
Intent intent = new Intent(Intent.ACTION_VIEW, Uri.parse("https://google.com"));
startActivity(intent);
```
- **Phone call panradhu:**
```java
Intent intent = new Intent(Intent.ACTION_DIAL, Uri.parse("tel:1234567890"));
startActivity(intent);
```

---

### 20. Intent enna?

**Definition:** Components ku idaila message pass panna or action trigger panna use panra object.

**Key Points:**
- **Explicit Intent:** Specific component-a start pannum
- **Implicit Intent:** Action request pannum (OS decide pannum component-a)
- Activities, Services, Broadcast Receivers ku data pass pannalam

**Example:**
```java
// Explicit Intent
Intent intent = new Intent(this, SecondActivity.class);
startActivity(intent);
```

---

## 13 MARK QUESTIONS

---

### 1. Android Platform Architecture

**Layers (Bottom to Top):**

#### **1. Linux Kernel (Base Layer)**
- Hardware ku interface
- Memory, process, security manage panrum
- Device drivers (camera, WiFi, Bluetooth)

#### **2. Hardware Abstraction Layer (HAL)**
- Hardware functions-a standard API-a convert panrum
- Manufacturer-specific code-a abstract panrum

#### **3. Native C/C++ Libraries**
- **SQLite:** Database
- **OpenGL ES:** Graphics
- **WebKit:** Browser engine
- **Media Framework:** Audio/Video

#### **4. Android Runtime (ART)**
- Apps-a execute panrum
- .dex files-a run panrum
- Garbage collection

#### **5. Java API Framework**
- **Activity Manager:** Activities manage panrum
- **Window Manager:** Windows handle panrum
- **Content Providers:** Data sharing
- **View System:** UI components
- **Package Manager:** Apps install/uninstall

#### **6. System Apps (Top Layer)**
- Pre-installed apps (Phone, Contacts, Browser)
- User apps indha layer la run aagum

**Diagram:**
```
┌─────────────────────────────────────┐
│      SYSTEM APPS & USER APPS        │
├─────────────────────────────────────┤
│      JAVA API FRAMEWORK             │
│ (Activity Mgr, View System, etc.)   │
├─────────────────────────────────────┤
│   ANDROID RUNTIME (ART) + LIBRARIES │
│   (SQLite, OpenGL, Media)           │
├─────────────────────────────────────┤
│   HARDWARE ABSTRACTION LAYER (HAL)  │
├─────────────────────────────────────┤
│         LINUX KERNEL                │
│   (Drivers, Memory, Security)       │
└─────────────────────────────────────┘
```

**Key Points:**
- Layered architecture - oru layer failure aacha marhadhu work aagum
- Open source - customization easy
- Security - permissions, sandboxing

---

### 2. Android Project Structure (Android Studio)

**Main Folders & Files:**

#### **1. app/ (Main Application Module)**
- **manifests/**
  - **AndroidManifest.xml:** App permissions, components declare pannurom
  
- **java/**
  - **com.example.app:** Java/Kotlin source code files
  
- **res/ (Resources)**
  - **layout/:** XML layout files (activity_main.xml)
  - **drawable/:** Images, icons
  - **values/:** strings.xml, colors.xml, styles.xml
  - **mipmap/:** App icons (different resolutions)

- **build.gradle (App-level):**
  - Dependencies, SDK versions

#### **2. Gradle Scripts**
- **build.gradle (Project-level):** Project-wide settings
- **settings.gradle:** Project modules list
- **gradle.properties:** Build configuration

#### **3. Important Files**

**AndroidManifest.xml Example:**
```xml
<manifest>
    <application android:icon="@mipmap/ic_launcher">
        <activity android:name=".MainActivity">
            <intent-filter>
                <action android:name="android.intent.action.MAIN" />
                <category android:name="android.intent.category.LAUNCHER" />
            </intent-filter>
        </activity>
    </application>
    <uses-permission android:name="android.permission.INTERNET" />
</manifest>
```

**strings.xml (values folder):**
```xml
<resources>
    <string name="app_name">MyApp</string>
    <string name="welcome">Welcome</string>
</resources>
```

**Structure Summary:**
```
MyProject/
├── app/
│   ├── manifests/
│   │   └── AndroidManifest.xml
│   ├── java/
│   │   └── MainActivity.java
│   ├── res/
│   │   ├── layout/
│   │   ├── drawable/
│   │   ├── values/
│   │   └── mipmap/
│   └── build.gradle
└── build.gradle (project)
```

---

### 3. Common UI Widgets in Android

#### **1. Button**
**Purpose:** User click pannuradhu ku

**XML:**
```xml
<Button
    android:id="@+id/btnSubmit"
    android:text="Submit"
    android:layout_width="wrap_content"
    android:layout_height="wrap_content" />
```

**Java:**
```java
Button btn = findViewById(R.id.btnSubmit);
btn.setOnClickListener(v -> Toast.makeText(this, "Clicked", Toast.LENGTH_SHORT).show());
```

---

#### **2. TextView**
**Purpose:** Text display panna use panrom

**XML:**
```xml
<TextView
    android:id="@+id/tvTitle"
    android:text="Welcome"
    android:textSize="20sp"
    android:textColor="#000000"
    android:layout_width="wrap_content"
    android:layout_height="wrap_content" />
```

**Java:**
```java
TextView tv = findViewById(R.id.tvTitle);
tv.setText("Hello Android");
```

---

#### **3. EditText**
**Purpose:** User input type panna

**XML:**
```xml
<EditText
    android:id="@+id/etName"
    android:hint="Enter name"
    android:inputType="textPersonName"
    android:layout_width="match_parent"
    android:layout_height="wrap_content" />
```

**Java:**
```java
EditText et = findViewById(R.id.etName);
String name = et.getText().toString();
```

---

#### **4. ImageView**
**Purpose:** Images display panna

**XML:**
```xml
<ImageView
    android:id="@+id/imgLogo"
    android:src="@drawable/logo"
    android:scaleType="centerCrop"
    android:layout_width="100dp"
    android:layout_height="100dp" />
```

**Java:**
```java
ImageView img = findViewById(R.id.imgLogo);
img.setImageResource(R.drawable.logo);
```

---

#### **5. CheckBox**
**Purpose:** Multiple options select panna

**XML:**
```xml
<CheckBox
    android:id="@+id/cbAgree"
    android:text="I agree to terms"
    android:layout_width="wrap_content"
    android:layout_height="wrap_content" />
```

**Java:**
```java
CheckBox cb = findViewById(R.id.cbAgree);
boolean isChecked = cb.isChecked();
```

---

#### **6. Spinner (Dropdown)**
**Purpose:** List la irundhu onnu select panna

**XML:**
```xml
<Spinner
    android:id="@+id/spinnerCountry"
    android:layout_width="match_parent"
    android:layout_height="wrap_content" />
```

**Java:**
```java
Spinner spinner = findViewById(R.id.spinnerCountry);
String[] countries = {"India", "USA", "UK"};
ArrayAdapter<String> adapter = new ArrayAdapter<>(this, android.R.layout.simple_spinner_item, countries);
spinner.setAdapter(adapter);
```

---

### 4. Input Validation Techniques in Android

**Purpose:** User wrong data enter pannama prevent panradhu

#### **Validation Types:**

**1. Empty Field Check**
```java
EditText etName = findViewById(R.id.etName);
String name = etName.getText().toString();

if (name.isEmpty()) {
    etName.setError("Name is required");
    return;
}
```

**2. Email Validation**
```java
String email = etEmail.getText().toString();

if (!Patterns.EMAIL_ADDRESS.matcher(email).matches()) {
    etEmail.setError("Invalid email");
    return;
}
```

**3. Password Length Check**
```java
String password = etPassword.getText().toString();

if (password.length() < 6) {
    etPassword.setError("Password must be 6+ characters");
    return;
}
```

**4. Phone Number Validation**
```java
String phone = etPhone.getText().toString();

if (phone.length() != 10) {
    etPhone.setError("Enter 10 digit number");
    return;
}
```

**5. Number Range Check**
```java
int age = Integer.parseInt(etAge.getText().toString());

if (age < 18 || age > 100) {
    etAge.setError("Age must be 18-100");
    return;
}
```

**Complete Example:**
```java
public void validateForm() {
    String name = etName.getText().toString();
    String email = etEmail.getText().toString();
    String phone = etPhone.getText().toString();
    
    // Name validation
    if (name.isEmpty()) {
        etName.setError("Required");
        return;
    }
    
    // Email validation
    if (!Patterns.EMAIL_ADDRESS.matcher(email).matches()) {
        etEmail.setError("Invalid email");
        return;
    }
    
    // Phone validation
    if (phone.length() != 10) {
        etPhone.setError("10 digits required");
        return;
    }
    
    // Ellam correct-a irundhaa
    Toast.makeText(this, "Form submitted!", Toast.LENGTH_SHORT).show();
}
```

---

### 5. Android Activity Lifecycle

**Definition:** Activity create aagi destroy aagura varaikum nadakkura stages.

#### **Lifecycle Methods (Order):**

**1. onCreate()**
- Activity create aagumbohu first call
- Layout set pannurom
- Initialization

**2. onStart()**
- Activity visible aagiduchu
- User paakka start pannuvanga

**3. onResume()**
- Activity foreground la active
- User interact panna ready

**4. onPause()**
- Another activity focus get panniduchu
- Background la poiruchu
- Data save pannurom

**5. onStop()**
- Activity completely hidden
- Screen la theriyaadhu

**6. onRestart()**
- Stop state la irundhaa again start aagum

**7. onDestroy()**
- Activity complete-a destroy
- Memory release
- Cleanup

#### **Lifecycle Diagram:**
```
        onCreate()
             ↓
        onStart()
             ↓
        onResume() ←──────┐
             ↓             │
    [ACTIVITY RUNNING]    │
             ↓             │
        onPause()          │
             ↓             │
        onStop()           │
             ↓             │
     onRestart() ──────────┘
             ↓
        onDestroy()
             ↓
        [DESTROYED]
```

#### **Use Cases:**

**onCreate():** Database initialize, views find panradhu
```java
protected void onCreate(Bundle savedInstanceState) {
    super.onCreate(savedInstanceState);
    setContentView(R.layout.activity_main);
    // Setup code
}
```

**onPause():** Data save panradhu, music pause panradhu
```java
protected void onPause() {
    super.onPause();
    // Save data, pause music
}
```

**onResume():** Music restart, refresh data
```java
protected void onResume() {
    super.onResume();
    // Resume music, refresh UI
}
```

**onDestroy():** Resources release, network connections close
```java
protected void onDestroy() {
    super.onDestroy();
    // Cleanup code
}
```

**States:**
- **Running:** User interact panranga
- **Paused:** Partially visible (dialog top la irukkum)
- **Stopped:** Completely hidden
- **Destroyed:** Memory la illa

---

### 6. Core Android Components

#### **1. ACTIVITIES**

**Definition:** UI screen - user interact panra component

**Real-time Example:**
- **Login Screen** = LoginActivity
- **Home Screen** = MainActivity
- **Profile Screen** = ProfileActivity

**Code:**
```java
public class MainActivity extends AppCompatActivity {
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
    }
}
```

**Use Case:** WhatsApp la each screen (Chat list, Chat window, Settings) = separate activities

---

#### **2. SERVICES**

**Definition:** Background la long-running operations panna component (UI illa)

**Real-time Examples:**
- **Music Player:** Background la music play aagum
- **File Download:** Download nadakkum, vera screen ku poiyum continue aagum
- **Location Tracking:** Background la GPS track panrum

**Code:**
```java
public class MusicService extends Service {
    public int onStartCommand(Intent intent, int flags, int startId) {
        // Play music
        return START_STICKY;
    }
    
    public IBinder onBind(Intent intent) {
        return null;
    }
}
```

**Start Service:**
```java
Intent intent = new Intent(this, MusicService.class);
startService(intent);
```

**Use Case:** YouTube la video play aagitu home button press pannalum audio continue aagum

---

#### **3. BROADCAST RECEIVERS**

**Definition:** System events or custom broadcasts-a receive panni respond panra component

**Real-time Examples:**
- **Battery Low Warning:** Battery 15% ku keela ponaa notification
- **SMS Received:** Message vandhaa read panradhu
- **Network Change:** WiFi ON/OFF aacha detect panradhu
- **Boot Completed:** Phone restart aanadhum app auto-start

**Code:**
```java
public class BatteryReceiver extends BroadcastReceiver {
    public void onReceive(Context context, Intent intent) {
        int level = intent.getIntExtra(BatteryManager.EXTRA_LEVEL, -1);
        Toast.makeText(context, "Battery: " + level + "%", Toast.LENGTH_SHORT).show();
    }
}
```

**Register in Manifest:**
```xml
<receiver android:name=".BatteryReceiver">
    <intent-filter>
        <action android:name="android.intent.action.BATTERY_LOW" />
    </intent-filter>
</receiver>
```

**Use Case:** Alarm apps - BOOT_COMPLETED broadcast receive panni alarms-a again set pannuradhu

---

#### **4. CONTENT PROVIDERS**

**Definition:** Apps ku idaila data share panna use panra component (Database la irukura data share panradhu)

**Real-time Examples:**
- **Contacts:** Phone la irukura contacts-a vera apps read pannalam
- **Gallery:** Photos-a Instagram, WhatsApp access pannalam
- **Calendar:** Calendar events-a apps share pannuradhu

**Code:**
```java
public class MyContentProvider extends ContentProvider {
    public Cursor query(Uri uri, String[] projection, String selection, String[] selectionArgs, String sortOrder) {
        // Return data from database
        return cursor;
    }
    
    public Uri insert(Uri uri, ContentValues values) {
        // Insert data
        return uri;
    }
}
```

**Access Content Provider:**
```java
// Contacts read panradhu
Cursor cursor = getContentResolver().query(
    ContactsContract.Contacts.CONTENT_URI,
    null, null, null, null
);
```

**Use Case:** WhatsApp la photo attach panna Gallery la irukura photos access panrum - adhu Content Provider through

---

## COMPONENT SUMMARY TABLE

| Component | Purpose | UI Irukuma? | Example |
|-----------|---------|-------------|---------|
| **Activity** | Screen with UI | Yes | Login page, Home screen |
| **Service** | Background tasks | No | Music player, Download |
| **Broadcast Receiver** | System events listen | No | Battery alert, SMS receive |
| **Content Provider** | Data sharing | No | Contacts, Gallery access |

---

## QUICK REVISION POINTS

**Remember:**
- **Activity** = Screen (UI irukum)
- **Service** = Background worker (UI illa)
- **Broadcast Receiver** = Event listener (notifications)
- **Content Provider** = Data sharing gate (apps ku idaila)

**Intent:**
- Components-a connect panna messenger
- Explicit = Specific target
- Implicit = System decide pannum

**Lifecycle:**
- onCreate → onStart → onResume → onPause → onStop → onDestroy
- onResume la interact pannalam
- onPause la data save pannanum

**Layouts:**
- LinearLayout = Line la (vertical/horizontal)
- RelativeLayout = Relative position
- ConstraintLayout = Flexible (new & best)

---

## TIPS FOR EXAM

1. **Diagrams:** Architecture & Lifecycle diagram draw panna marks kidaikum
2. **Code:** Short-a, clear-a ezhudhunga - syntax perfect-a irukanum
3. **Examples:** Real-world examples sollum (WhatsApp, YouTube)
4. **Keywords:** Bold-a highlight pannunga important terms
5. **Structure:** Points-a clear-a ezhudhunga

**All the best! 🎓**
