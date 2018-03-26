# Java - ściąga
#### Kompilowanie pliku .java
```bash
javac HelloWorld.java
java HelloWorld
```
#### Czytanie pliku .txt
```java
String everything;
try(BufferedReader br = new BufferedReader(new FileReader("out/production/untitled1/haha.txt"))) { //Copy relative path się tutaj przydaje :)
    StringBuilder sb = new StringBuilder();
    String line = br.readLine();

    while (line != null)    {
        sb.append(line);
        sb.append(System.lineSeparator());
        line = br.readLine();
    }

    everything = sb.toString();
}
System.out.println(everything);
```



