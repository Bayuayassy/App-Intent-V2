# App-Intent-V2

Nama &nbsp; &nbsp;: Bayu Maulana Ayassy<br>
NIM&nbsp; &nbsp; &nbsp; : 312210166<br>
Kelas&ensp; &nbsp; : TI.22.A.1<br>
Dosen &nbsp; : Donny Maulana, S.Kom., M.M.S.I.<br><br>
*Aplikasi intent versi kedua, dengan perubahan tombol text menjadi ICON*

## 1. Menu Utama 
Pertama yang harus kita lakukan adalah mengganti tampilan menu utamanya dengan code yang baru agar ikon tombol berubah menjadi gambar, caranya adalah :

Jika awal pembuatan project kita memilih template Empty Views Activity, maka pada layout otomatis terbuat file `activity_main.xml` dan pada java akan ada `MainActivity.java`. Maka langsung saja kita buka `activity_main.xml`, dan buat code seperti berikut ini:

```
<?xml version="1.0" encoding="utf-8"?>
<RelativeLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">


    <RelativeLayout
        android:layout_width="500dp"
        android:layout_height="match_parent"
        android:background="@drawable/bg6">

    </RelativeLayout>

    <LinearLayout
        android:layout_width="match_parent"
        android:layout_height="match_parent"
        android:layout_marginLeft="16dp"
        android:layout_marginTop="100dp"
        android:layout_marginRight="16dp"
        android:orientation="vertical">

        <TextView
            android:id="@+id/textView"
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            android:fontFamily="serif"
            android:text="Menu Program"
            android:textAlignment="center"
            android:textColor="@color/black"
            android:textSize="34sp"
            android:textStyle="bold" />

        <LinearLayout
            android:layout_width="match_parent"
            android:layout_height="150dp"
            android:layout_margin="5dp"
            android:orientation="horizontal">

            <androidx.cardview.widget.CardView
                android:id="@+id/cdMenu1"
                android:layout_width="match_parent"
                android:layout_height="match_parent"
                android:layout_margin="10dp"
                android:layout_weight="1"
                app:cardCornerRadius="20dp"
                app:cardElevation="7dp">

                <LinearLayout
                    android:layout_width="match_parent"
                    android:layout_height="match_parent"
                    android:orientation="vertical">

                    <ImageView
                        android:id="@+id/imageView0"
                        android:layout_width="match_parent"
                        android:layout_height="wrap_content"
                        android:layout_margin="16dp"
                        android:layout_weight="1"
                        app:srcCompat="@drawable/worldwide" />

                    <TextView
                        android:id="@+id/textView0"
                        android:layout_width="match_parent"
                        android:layout_height="wrap_content"
                        android:fontFamily="serif"
                        android:text="Hello World"
                        android:textAlignment="center"
                        android:textSize="18dp"
                        android:textStyle="bold" />
                </LinearLayout>
            </androidx.cardview.widget.CardView>

            <androidx.cardview.widget.CardView
                android:id="@+id/cdMenu2"
                android:layout_width="match_parent"
                android:layout_height="match_parent"
                android:layout_margin="10dp"
                android:layout_weight="1"
                app:cardCornerRadius="20dp"
                app:cardElevation="7dp">

                <LinearLayout
                    android:layout_width="match_parent"
                    android:layout_height="match_parent"
                    android:orientation="vertical">

                    <ImageView
                        android:id="@+id/imageView1"
                        android:layout_width="match_parent"
                        android:layout_height="wrap_content"
                        android:layout_margin="16dp"
                        android:layout_weight="1"
                        app:srcCompat="@drawable/mathematics_symbols" />

                    <TextView
                        android:id="@+id/textView1"
                        android:layout_width="match_parent"
                        android:layout_height="wrap_content"
                        android:fontFamily="serif"
                        android:text="Fibonacci"
                        android:textAlignment="center"
                        android:textSize="18dp"
                        android:textStyle="bold" />
                </LinearLayout>
            </androidx.cardview.widget.CardView>
        </LinearLayout>

        <LinearLayout
            android:layout_width="match_parent"
            android:layout_height="150dp"
            android:layout_margin="5dp"
            android:orientation="horizontal">

            <androidx.cardview.widget.CardView
                android:id="@+id/cdMenu3"
                android:layout_width="match_parent"
                android:layout_height="match_parent"
                android:layout_margin="10dp"
                android:layout_weight="1"
                app:cardCornerRadius="20dp"
                app:cardElevation="7dp">

                <LinearLayout
                    android:layout_width="match_parent"
                    android:layout_height="match_parent"
                    android:orientation="vertical">

                    <ImageView
                        android:id="@+id/imageView2"
                        android:layout_width="match_parent"
                        android:layout_height="wrap_content"
                        android:layout_margin="16dp"
                        android:layout_weight="1"
                        app:srcCompat="@drawable/clapperboard" />

                    <TextView
                        android:id="@+id/textView2"
                        android:layout_width="match_parent"
                        android:layout_height="wrap_content"
                        android:fontFamily="serif"
                        android:text="Scroll Movie"
                        android:textAlignment="center"
                        android:textSize="18dp"
                        android:textStyle="bold" />
                </LinearLayout>
            </androidx.cardview.widget.CardView>

            <androidx.cardview.widget.CardView
                android:id="@+id/cdMenu4"
                android:layout_width="match_parent"
                android:layout_height="match_parent"
                android:layout_margin="10dp"
                android:layout_weight="1"
                app:cardCornerRadius="20dp"
                app:cardElevation="7dp">

                <LinearLayout
                    android:layout_width="match_parent"
                    android:layout_height="match_parent"
                    android:orientation="vertical">

                    <ImageView
                        android:id="@+id/imageView3"
                        android:layout_width="match_parent"
                        android:layout_height="wrap_content"
                        android:layout_margin="16dp"
                        android:layout_weight="1"
                        app:srcCompat="@drawable/alarm__1_" />

                    <TextView
                        android:id="@+id/textView3"
                        android:layout_width="match_parent"
                        android:layout_height="wrap_content"
                        android:fontFamily="serif"
                        android:text="Alarm"
                        android:textAlignment="center"
                        android:textSize="18dp"
                        android:textStyle="bold" />
                </LinearLayout>
            </androidx.cardview.widget.CardView>
        </LinearLayout>

        <LinearLayout
            android:layout_width="match_parent"
            android:layout_height="150dp"
            android:layout_margin="5dp"
            android:orientation="horizontal">

            <androidx.cardview.widget.CardView
                android:id="@+id/cdMenu5"
                android:layout_width="match_parent"
                android:layout_height="match_parent"
                android:layout_margin="10dp"
                android:layout_weight="1"
                app:cardCornerRadius="20dp"
                app:cardElevation="7dp">

                <LinearLayout
                    android:layout_width="match_parent"
                    android:layout_height="match_parent"
                    android:orientation="vertical">

                    <ImageView
                        android:id="@+id/imageView4"
                        android:layout_width="match_parent"
                        android:layout_height="wrap_content"
                        android:layout_margin="16dp"
                        android:layout_weight="1"
                        app:srcCompat="@drawable/messaging" />

                    <TextView
                        android:id="@+id/textView4"
                        android:layout_width="match_parent"
                        android:layout_height="wrap_content"
                        android:fontFamily="serif"
                        android:text="Two Activity"
                        android:textAlignment="center"
                        android:textSize="18dp"
                        android:textStyle="bold" />
                </LinearLayout>
            </androidx.cardview.widget.CardView>

            <androidx.cardview.widget.CardView
                android:id="@+id/cdMenu6"
                android:layout_width="match_parent"
                android:layout_height="match_parent"
                android:layout_margin="10dp"
                android:layout_weight="1"
                app:cardCornerRadius="20dp"
                app:cardElevation="7dp">

                <LinearLayout
                    android:layout_width="match_parent"
                    android:layout_height="match_parent"
                    android:orientation="vertical">

                    <ImageView
                        android:id="@+id/imageView5"
                        android:layout_width="match_parent"
                        android:layout_height="wrap_content"
                        android:layout_margin="16dp"
                        android:layout_weight="1"
                        app:srcCompat="@drawable/gps" />

                    <TextView
                        android:id="@+id/textView5"
                        android:layout_width="match_parent"
                        android:layout_height="wrap_content"
                        android:fontFamily="serif"
                        android:text="Maps"
                        android:textAlignment="center"
                        android:textSize="18dp"
                        android:textStyle="bold" />
                </LinearLayout>
            </androidx.cardview.widget.CardView>

        </LinearLayout>
    </LinearLayout>

</RelativeLayout>
```

> - Maka tampilan menu utama akan seperti ini :

![Gambar WhatsApp 2023-12-02 pukul 14 30 46_2b70bc2b](https://github.com/Bayuayassy/App-Intent-V2/assets/115678251/89c4f780-f366-49c7-b3ee-7794af517a44)


> - Setelah itu kita buka `MainActivity.java` untuk menambahkan code intent untuk masing-masing tombol :
```
package com.intent_app;

import android.content.Intent;
import android.net.Uri;
import android.os.Bundle;
import android.view.View;
import androidx.appcompat.app.AppCompatActivity;

public class MainActivity extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);

        findViewById(R.id.cdMenu4).setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View v) {

                setAlarm();
            }
        });

        findViewById(R.id.cdMenu1).setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View v) {
                // Ketika tombolSatu ditekan, pindah ke HelloActivity
                Intent helloworld = new Intent(MainActivity.this, HelloActivity.class);
                startActivity(helloworld);
            }
        });

        findViewById(R.id.cdMenu2).setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View v) {
                // Ketika tombolDua ditekan, lakukan aksi yang diinginkan
                // Misalnya, pindah ke aktivitas lain atau jalankan fungsi khusus
                Intent toast = new Intent(MainActivity.this, CountActivity.class);
                startActivity(toast);
            }
        });

        findViewById(R.id.cdMenu3).setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View v) {
                // Ketika tombolDua ditekan, lakukan aksi yang diinginkan
                // Misalnya, pindah ke aktivitas lain atau jalankan fungsi khusus
                Intent sianida = new Intent(MainActivity.this, SianidaActivity.class);
                startActivity(sianida);
            }
        });

        findViewById(R.id.cdMenu5).setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View v) {
                // Ketika tombolDua ditekan, lakukan aksi yang diinginkan
                // Misalnya, pindah ke aktivitas lain atau jalankan fungsi khusus
                Intent twoactivity = new Intent(MainActivity.this, TwoActivity.class);
                startActivity(twoactivity);
            }
        });

        findViewById(R.id.cdMenu6).setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View v) {
                // Example location: Jakarta, Indonesia
                Uri geoLocation = Uri.parse("geo:-6.2088,106.8456");
                openMaps(geoLocation);
            }
        });
    }

    private void setAlarm() {
        Intent alarmIntent = new Intent(android.provider.AlarmClock.ACTION_SET_ALARM);
        // Add extra details for the alarm, e.g., alarm time, label, etc.
        // alarmIntent.putExtra(...
        startActivity(alarmIntent);
    }
    private void openMaps(Uri geoLocation) {
        Intent maps = new Intent(Intent.ACTION_VIEW);
        maps.setData(geoLocation);
        if (maps.resolveActivity(getPackageManager()) != null) {
            startActivity(maps);
        }
    }


}
```

> Button *HelloWorld, Count, Sianida dan TwoActivity* menggunakan Explicit Intent, dan untuk project *SetAlarm* beserta *Maps* menggunakan Implicit Intent.

> Menu halaman utama dan tombol-tombol aplikasi sudah berhasil dibuat. Maka selanjutnya yang kita lakukan adalah menambahkan coding pada `AndroidManifest.xml` agar aplikasi dapat berjalan.

## 3. AndroidManifest.xml
Didalam AndroidManifest.xml ini kita tambahkan semua .java dari semua project kita sebelumnya. Berikut nama .java dari berbagai project yang telah saya buat:<br>
- a. Project Hello World = HelloActivity.java
- b. Project Count = CountActivity.java
- c. Project Sianida = SianidaActivity.java
- d. Project TwoActivity = TwoactActivity.java dan Twoact2Activity.java
- e. Project Set Alarm = MainActivity.java (karena implicit intent, jadi code untuk set alarm dibuat langsung disini)
```
<?xml version="1.0" encoding="utf-8"?>
<manifest xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:tools="http://schemas.android.com/tools">

    <uses-permission
        android:name="com.android.alarm.permission.SET_ALARM" />
    <application
        android:allowBackup="true"
        android:dataExtractionRules="@xml/data_extraction_rules"
        android:fullBackupContent="@xml/backup_rules"
        android:icon="@drawable/backgroundlauncer"
        android:label="@string/app_name"
        android:roundIcon="@drawable/backgroundlauncer"
        android:supportsRtl="true"
        android:theme="@style/Base.Theme.IntentApp"
        tools:targetApi="31">

        <activity
            android:name=".MainActivity"
            android:exported="true">
            <intent-filter>
                <action android:name="android.intent.action.SET_ALARM" />
                <category android:name="android.intent.category.DEFAULT" />
            </intent-filter>
        </activity>

        <activity
            android:name=".HelloActivity"
            android:exported="true" />

        <activity
            android:name=".TwoactActivity"
            android:exported="true" />

        <activity
            android:name=".Twoact2Activity"
            android:exported="true" />

        <activity
            android:name=".CountActivity"
            android:exported="true" />

        <activity
            android:name=".SianidaActivity"
            android:exported="true" />

        <activity
            android:name=".SplashScreen"
            android:exported="true"
            android:theme="@style/SplashScreen">
            <intent-filter>
                <action android:name="android.intent.action.MAIN" />
                <category android:name="android.intent.category.LAUNCHER" />
            </intent-filter>
        </activity>
    </application>

</manifest>
```
## 4. Hasil RUN
Berikut video hasil RUN, dari aplkasi yang sudah saya buat ini :<br>

https://github.com/Bayuayassy/App-Intent-V2/assets/115678251/300b94c0-48f5-47e1-901f-72fd17f76552

# Code Semua Project
## Strings, Colors, Dimens
- Strings
  > Berisi semua string dari project
  ```
  <resources>
    <string name="app_name">IntentApp</string>
    <string name="project_hello">Project Hello World</string>
    <string name="project_count">Project Count</string>
    <string name="project_sianida">Project Sianida</string>
    <string name="project_twoactivity">Project TwoActivity</string>
    <string name="project_set_alarm">Project Set Alarm</string>

    <string name="hello_text">>_Hello World!</string>

    <string name="button_label_toast">Desk</string>
    <string name="button_label_count">Count</string>
    <string name="count_initial_value">0</string>
    <string name="toast_message">Project Count</string>

    <string name="button_main">Send</string>
    <string name="text_header_reply">Message Received</string>
    <string name="editText_main">Enter Your Message Here</string>
    <string name="text_header">Reply Received</string>
    <string name="button_second">Reply</string>
    <string name="editText_second">Enter Your Reply Here</string>

    <string name="article_title">Kasus Sianida</string>
    <string name="article_subtitle">ICE COLD!</string>

    <string name="article_teks">Kasus kopi sianida berawal dari pertemuan Jessica Wongso, Mirna, dan Hanie Boon Juwita di Kafe Olivier Grand Indonesia (GI) pada 6 Januari 2016. Jessica datang lebih dahulu         dan memesan tempat dilayani resepsionis Cindy yang menawarkan meja nomor 54.</string>
</resources>

  ```

- Colors
  > Berisi semua colors dari project
  ```

  <?xml version="1.0" encoding="utf-8"?>
<resources>
    <color name="black">#FF000000</color>
    <color name="white">#FFFFFFFF</color>
    <color name="grey">#323232</color>
    <color name="blue">#0004FF</color>
    <color name="green">#08BD02</color>
    <color name="colorPrimary">#3F51B5</color>
    <color name="colorPrimaryDark">#303F9F</color>
    <color name="colorAccent">#FF4081</color>
</resources>

  ```
- Dimens
  > Berisi code dimen untuk project sianida
  ```
  <?xml version="1.0" encoding="utf-8"?>
  <resources>
    <dimen name="padding_regular">10dp</dimen>
    <dimen name="line_spacing">5sp</dimen>
  </resources>
  ```
  
## A. Project Hello World
- **activity_hello.xml**
  ```
  <?xml version="1.0" encoding="utf-8"?>
  <androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".HelloActivity">

    <ImageView
        android:id="@+id/background"
        android:layout_width="match_parent"
        android:layout_height="match_parent"
        android:background="@drawable/bg_hello"
        android:adjustViewBounds="true"
        android:scaleType="centerCrop"/>

    <TextView
        android:id="@+id/Texthello"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:fontFamily="courier"
        android:gravity="center"
        android:text="@string/hello_text"
        android:textColor="@color/green"
        android:textSize="11pt"
        android:textStyle="bold"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        tools:ignore="TextSizeCheck" />

  </androidx.constraintlayout.widget.ConstraintLayout>
  ```
- **HelloActivity.java**
  ```
  package com.example.tugassembilan;

  import android.os.Bundle;
  import androidx.appcompat.app.AppCompatActivity;

  public class HelloActivity extends AppCompatActivity {

  @Override
  protected void onCreate(Bundle savedInstanceState) {
      super.onCreate(savedInstanceState);
      setContentView(R.layout.activity_hello);
      }
  }
  ```
## B. Project Count
- **activity_count.xml**
  ```
  <?xml version="1.0" encoding="utf-8"?>
  <androidx.constraintlayout.widget.ConstraintLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".CountActivity">

    <ImageView
        android:id="@+id/background"
        android:layout_width="match_parent"
        android:layout_height="match_parent"
        android:background="@drawable/bg_count"
        android:adjustViewBounds="true"
        android:scaleType="centerCrop" />

    <Button
        android:id="@+id/button_toast"
        android:layout_width="0dp"
        android:layout_height="wrap_content"
        android:layout_marginEnd="8dp"
        android:layout_marginStart="8dp"
        android:layout_marginTop="8dp"
        android:background="@color/colorPrimary"
        android:onClick="showToast"
        android:text="@string/button_label_toast"
        android:textColor="@android:color/white"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        tools:ignore="UsingOnClickInXml"/>

    <Button
        android:id="@+id/button_count"
        android:layout_width="0dp"
        android:layout_height="wrap_content"
        android:layout_marginEnd="8dp"
        android:layout_marginStart="8dp"
        android:layout_marginBottom="8dp"
        android:background="@color/colorPrimary"
        android:onClick="countUp"
        android:text="@string/button_label_count"
        android:textColor="@android:color/white"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintBottom_toBottomOf="parent"
        tools:ignore="UsingOnClickInXml" />

    <TextView
        android:id="@+id/show_count"
        android:layout_width="0dp"
        android:layout_height="wrap_content"
        android:layout_marginStart="8dp"
        android:layout_marginEnd="8dp"
        android:text="@string/count_initial_value"
        android:textAlignment="center"
        android:textColor="@color/colorPrimary"
        android:textSize="160sp"
        android:textStyle="bold"
        app:layout_constraintBottom_toTopOf="@+id/button_count"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toBottomOf="@+id/button_toast"
        tools:ignore="RtlCompat" />

  </androidx.constraintlayout.widget.ConstraintLayout>
  ```
- **CountActivity.java**
  ```
  package com.example.tugassembilan;

  import android.annotation.SuppressLint;
  import android.os.Bundle;
  import android.view.View;
  import android.widget.TextView;
  import android.widget.Toast;

  import androidx.appcompat.app.AppCompatActivity;

  public class CountActivity extends AppCompatActivity {
  private int nCount = 0;

  private TextView nShowCount;

  @SuppressLint("MissingInflatedId")
  @Override
  protected void onCreate(Bundle savedInstanceState) {
      super.onCreate(savedInstanceState);
      setContentView(R.layout.activity_count);
      nShowCount = findViewById(R.id.show_count);
      }

      public void showToast(View view){
      Toast toast = Toast.makeText(this, "Menghitung Bilangan",
          Toast.LENGTH_SHORT);
          toast.show();
      }

      @SuppressLint("SetTextI18n")
      public void countUp(View view){
          nCount++;
      if (nShowCount != null)
          nShowCount.setText(Integer.toString(nCount));
      }
  }
  ```

## C. Project Sianida
- **activity_sianida.xml**
  ```
  <?xml version="1.0" encoding="utf-8"?>
  <RelativeLayout xmlns:android="http://schemas.android.com/apk/res/android"
      android:layout_width="match_parent"
      android:layout_height="match_parent"
      xmlns:tools="http://schemas.android.com/tools"
      tools:context=".SianidaActivity">

      <TextView
          android:id="@+id/article_heading"
          android:layout_width="match_parent"
          android:layout_height="wrap_content"
          android:background="@color/colorPrimary"
          android:padding="@dimen/padding_regular"
          android:text="@string/article_title"
          android:textAppearance="@android:style/TextAppearance.DeviceDefault.Large"
          android:textColor="@android:color/white"
          android:textStyle="bold" />

        <ScrollView
          android:layout_width="wrap_content"
          android:layout_height="wrap_content"
          android:layout_below="@id/article_heading">

          <LinearLayout
              android:layout_width="match_parent"
              android:layout_height="wrap_content"
              android:orientation="vertical">

              <TextView
                  android:id="@+id/article_subheading"
                  android:layout_width="match_parent"
                  android:layout_height="wrap_content"
                  android:padding="@dimen/padding_regular"
                  android:text="@string/article_subtitle"
                  android:textAlignment="center"
                  android:textAppearance="@android:style/TextAppearance.DeviceDefault"
                  android:textColor="#8D6E63" />

              <TextView
                  android:id="@+id/article"
                  android:layout_width="wrap_content"
                  android:layout_height="wrap_content"
                  android:autoLink="web"
                  android:lineSpacingExtra="@dimen/line_spacing"
                  android:padding="@dimen/padding_regular"
                  android:text="@string/article_teks"
                  tools:ignore="VisualLintLongText" />
          </LinearLayout>
      </ScrollView>
  </RelativeLayout>
  ```
- **SianidaActivity.java**
  ```
  package com.example.tugassembilan;

  import android.os.Bundle;

  import androidx.appcompat.app.AppCompatActivity;

  public class SianidaActivity extends AppCompatActivity {
      @Override
      protected void onCreate(Bundle savedInstanceState){
          super.onCreate(savedInstanceState);
          setContentView(R.layout.activity_sianida);
      }
  }
  ```

## D. Project TwoActivity
- **activity_twoact.xml**
  ```
  <?xml version="1.0" encoding="utf-8"?>
  <androidx.constraintlayout.widget.ConstraintLayout
      xmlns:android="http://schemas.android.com/apk/res/android"
      android:layout_width="match_parent"
      android:layout_height="match_parent"
      xmlns:tools="http://schemas.android.com/tools"
      xmlns:app="http://schemas.android.com/apk/res-auto"
      tools:context=".TwoactActivity">

      <ImageView
          android:id="@+id/background"
          android:layout_width="match_parent"
          android:layout_height="match_parent"
          android:adjustViewBounds="true"
          android:scaleType="centerCrop"
          android:src="@drawable/bg_twoact" />

      <TextView
          android:id="@+id/text_header_reply"
          android:layout_width="wrap_content"
          android:layout_height="wrap_content"
          android:layout_marginStart="8dp"
          android:layout_marginLeft="8dp"
          android:layout_marginTop="16dp"
          android:text="@string/text_header_reply"
          android:textAppearance="@style/TextAppearance.AppCompat.Medium"
          android:textStyle="bold"
          android:visibility="invisible"
          app:layout_constraintStart_toStartOf="parent"
          app:layout_constraintTop_toTopOf="parent"/>

      <TextView
          android:id="@+id/text_message_reply"
          android:layout_width="wrap_content"
          android:layout_height="wrap_content"
          android:layout_marginStart="8dp"
          android:layout_marginLeft="8dp"
          android:layout_marginTop="8dp"
          android:visibility="invisible"
          app:layout_constraintStart_toStartOf="parent"
          app:layout_constraintTop_toBottomOf="@+id/text_header_reply" />

      <Button
          android:id="@+id/button_main"
          android:layout_width="wrap_content"
          android:layout_height="wrap_content"
          android:layout_marginBottom="16dp"
          android:layout_marginRight="16dp"
          android:text="@string/button_main"
          android:onClick="LaunchSecondActivity"
          app:layout_constraintBottom_toBottomOf="parent"
          app:layout_constraintRight_toRightOf="parent"
          tools:ignore="UsingOnClickInXml"/>

      <EditText
          android:id="@+id/editText_main"
          android:layout_width="0dp"
          android:layout_height="wrap_content"
          android:layout_marginStart="8dp"
          android:layout_marginEnd="8dp"
          android:layout_marginBottom="16dp"
          android:ems="10"
          android:hint="@string/editText_main"
          android:inputType="textLongMessage"
          android:minHeight="48dp"
          app:layout_constraintBottom_toBottomOf="parent"
          app:layout_constraintEnd_toStartOf="@+id/button_main"
          app:layout_constraintStart_toStartOf="parent" />
  </androidx.constraintlayout.widget.ConstraintLayout>
  ```
- **activity_twoact2.xml**
  ```
  <?xml version="1.0" encoding="utf-8"?>
  <androidx.constraintlayout.widget.ConstraintLayout
      xmlns:android="http://schemas.android.com/apk/res/android"
      android:layout_width="match_parent"
      android:layout_height="match_parent"
      xmlns:tools="http://schemas.android.com/tools"
      xmlns:app="http://schemas.android.com/apk/res-auto"
      tools:context=".Twoact2Activity">

      <ImageView
          android:id="@+id/background"
          android:layout_width="match_parent"
          android:layout_height="match_parent"
          android:adjustViewBounds="true"
          android:scaleType="centerCrop"
          android:src="@drawable/bg_twoact" />

      <TextView
          android:id="@+id/text_header"
          android:layout_width="wrap_content"
          android:layout_height="wrap_content"
          android:layout_marginStart="8dp"
          android:layout_marginLeft="8dp"
          android:layout_marginTop="16dp"
          android:text="@string/text_header"
          android:textAppearance="@style/TextAppearance.AppCompat.Medium"
          android:textStyle="bold"
          app:layout_constraintStart_toStartOf="parent"
          app:layout_constraintTop_toTopOf="parent" />

      <TextView
          android:id="@+id/text_message"
          android:layout_width="wrap_content"
          android:layout_height="wrap_content"
          android:layout_marginStart="8dp"
          android:layout_marginLeft="8dp"
          android:layout_marginTop="8dp"
          app:layout_constraintStart_toStartOf="parent"
          app:layout_constraintTop_toBottomOf="@+id/text_header" />

      <Button
          android:id="@+id/button_second"
          android:layout_width="wrap_content"
          android:layout_height="wrap_content"
          android:layout_marginBottom="16dp"
          android:layout_marginRight="16dp"
          android:text="@string/button_second"
          android:onClick="returnReply"
          app:layout_constraintBottom_toBottomOf="parent"
          app:layout_constraintRight_toRightOf="parent"
          tools:ignore="UsingOnClickInXml" />

      <EditText
          android:id="@+id/editText_second"
          android:layout_width="0dp"
          android:layout_height="wrap_content"
          android:layout_marginStart="8dp"
          android:layout_marginEnd="8dp"
          android:layout_marginBottom="16dp"
          android:ems="10"
          android:hint="@string/editText_second"
          android:inputType="textLongMessage"
          android:minHeight="48dp"
          app:layout_constraintBottom_toBottomOf="parent"
          app:layout_constraintEnd_toStartOf="@+id/button_second"
          app:layout_constraintStart_toStartOf="parent" />
  </androidx.constraintlayout.widget.ConstraintLayout>
  ```

- **TwoactActivity.java**
  ```
  package com.example.tugassembilan;

  import androidx.appcompat.app.AppCompatActivity;

  import android.content.Intent;
  import android.os.Bundle;
  import android.util.Log;
  import android.view.View;
  import android.widget.EditText;
  import android.widget.TextView;

  public class TwoactActivity extends AppCompatActivity {

      private static final String LOG_TAG = TwoactActivity.class.getSimpleName();

      public static final String EXTRA_MESSAGE = "com.example.android.Twoact2Activity.extra.MESSAGE";

      public static final int TEXT_REQUEST = 1;

      private EditText mMessageEditText;

      private TextView mReplyHeadTextView;

      private TextView mReplyTextView;

      @Override
      protected void onCreate(Bundle savedInstanceState) {
          super.onCreate(savedInstanceState);
          setContentView(R.layout.activity_twoact);

          mMessageEditText = findViewById(R.id.editText_main);
          mReplyHeadTextView = findViewById(R.id.text_header_reply);
          mReplyTextView = findViewById(R.id.text_message_reply);
      }

      public void LaunchSecondActivity(View view) {
          Log.d(LOG_TAG, "Button clicked!");
          Intent intent = new Intent(this, Twoact2Activity.class);
          String message = mMessageEditText.getText().toString();
          intent.putExtra(EXTRA_MESSAGE, message);
          startActivityForResult(intent, TEXT_REQUEST);
      }

      @Override
      public void onActivityResult(int requestCode, int resultCode, Intent data) {
          super.onActivityResult(requestCode, resultCode, data);

          if (resultCode == TEXT_REQUEST) {
              if (resultCode == RESULT_OK) {
              String reply = data.getStringExtra(Twoact2Activity.EXTRA_REPLY);

              mReplyHeadTextView.setVisibility(View.VISIBLE);

              mReplyHeadTextView.setText(reply);
              mReplyHeadTextView.setVisibility(View.VISIBLE);
              }
          }
      }
  }
  ```

- **Twoact2Activity.java**
  ```
  package com.example.tugassembilan;

  import android.content.Intent;
  import android.os.Bundle;
  import android.view.View;
  import android.widget.EditText;
  import android.widget.TextView;

  import androidx.appcompat.app.AppCompatActivity;

  public class Twoact2Activity extends AppCompatActivity {

      public static final String EXTRA_REPLY ="com.example.android.Twoact2Activity.extra.REPLY";

      private EditText mReply;

      @Override
      protected void onCreate(Bundle savedInstanceState){
          super.onCreate(savedInstanceState);
          setContentView(R.layout.activity_twoact2);

          mReply = findViewById(R.id.editText_second);

          Intent intent = getIntent();
          String message = intent.getStringExtra(TwoactActivity.EXTRA_MESSAGE);

          TextView textView = findViewById(R.id.text_message);
          textView.setText(message);
      }
      public void returnReply(View view){
          String reply = mReply.getText().toString();
          Intent replyIntent = new Intent();
          setResult(RESULT_OK, replyIntent);
          finish();
      }
  }
  ```
## E. Project Set Alarm
- Buat buttonnya terlebih dahulu didalam sebuah activity.xml, disini saya buat di **activity_main.xml**, bersama dengan tombol lainnya.
  ```
  <Button
        android:id="@+id/btnSetAlarm"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:onClick="btnSetAlarm"
        android:layout_below="@+id/btnTwoActivity"
        android:layout_centerHorizontal="true"
        android:layout_marginTop="20dp"
        android:text="@string/project_set_alarm"
        tools:ignore="UsingOnClickInXml" />
  ```
- Tambahkan code implicit intent pada .java nya.
  ```
              findViewById(R.id.btnSetAlarm).setOnClickListener(new View.OnClickListener() {
              @Override
              public void onClick(View v) {
                  // Panggil metode untuk mengatur alarm
                  setAlarm();
              }
          });
      }
      private void setAlarm() {
      Intent alarm = new Intent(android.provider.AlarmClock.ACTION_SET_ALARM);
      startActivity(alarm);
  }
  ```
- Buka **AndroidManifest.xml** dan tambahkan code untuk izin membuka Alarm
  ```
  <uses-permission android:name="com.android.alarm.permission.SET_ALARM" />
  ```
  Tambahkan code berikut didalam *application* agar set alarm dapat berjalan:
  ```
      <activity
          android:name=".MainActivity"
          android:exported="true">
          <intent-filter>
              <action android:name="android.intent.action.SET_ALARM" />
              <category android:name="android.intent.category.DEFAULT" />
          </intent-filter>
      </activity>
  ```

  ## Note
  Semua project diatas terdapat code untuk background, kalian bisa memakainya atau tidak. Jika kalian memutuskan memakainya, jangan lupa untuk menambahkan gambar backgroundnya di folder **drawable**.

  # Selesai
  Akhirnya telah selesai repository ini, jika ada kesalahan pengetikan dalam repository ini saya memohon maaf. Terimakasih sudah membaca.
