Descripsi Project :
Tugas  pembuatan gradle dan pembuatan libary di gradle
Cara run project : 
1. Masukan task
   task greetingTask() { // subuah task yang di jalankan akan mengisi data yang sesuai di terminal
    doLast {
        String nama = project.hasProperty('nama') ? project.property('nama') : 'Gradle User'
        println "Hello, $nama! Welcome to Gradle World!"
    }
}
2. Klik Terminal
3. Masukan ./gradlew greetingTask -Pnama=Rizkika
4. Klik Enter
5. Akan muncul hasil seperti di bawah ini
   ![image](https://github.com/Kikamn/BelajarGradle/assets/157001435/04a0243b-1abc-4eac-bcf4-02f354658247)

Cara membuat libary di gradel:
1. Tingal masukan Code
   dependencies {
  implementation 'com.google.guava:guava:29.0-jre'
  testImplementation 'junit:junit:4.13'
  }
2. Tingal Save
