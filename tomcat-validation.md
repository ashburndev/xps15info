6:52 AM 8/29/2018

```
https://tomcat.apache.org/download-80.cgi
http://www-eu.apache.org/dist/tomcat/tomcat-8/v8.5.33/README.html

8.5.33

Please see the README file for packaging information. It explains what every distribution contains.
Binary Distributions

    Core:
        zip (pgp, sha512)
        tar.gz (pgp, sha512)
        32-bit Windows zip (pgp, sha512)
        64-bit Windows zip (pgp, sha512)
        32-bit/64-bit Windows Service Installer (pgp, sha512)
    Full documentation:
        tar.gz (pgp, sha512)
    Deployer:
        zip (pgp, sha512)
        tar.gz (pgp, sha512)
    Extras:
        JMX Remote jar (pgp, sha512)
        Web services jar (pgp, sha512)
    Embedded:
        tar.gz (pgp, sha512)
        zip (pgp, sha512)


https://tomcat.apache.org/download-90.cgi
http://www-us.apache.org/dist/tomcat/tomcat-9/v9.0.11/README.html

9.0.11

Please see the README file for packaging information. It explains what every distribution contains.
Binary Distributions

    Core:
        zip (pgp, sha512)
        tar.gz (pgp, sha512)
        32-bit Windows zip (pgp, sha512)
        64-bit Windows zip (pgp, sha512)
        32-bit/64-bit Windows Service Installer (pgp, sha512)
    Full documentation:
        tar.gz (pgp, sha512)
    Deployer:
        zip (pgp, sha512)
        tar.gz (pgp, sha512)
    Extras:
        JMX Remote jar (pgp, sha512)
        Web services jar (pgp, sha512)
    Embedded:
        tar.gz (pgp, sha512)
        zip (pgp, sha512)


08/29/2018  06:53 AM            37,537 KEYS.txt
08/29/2018  06:53 AM        10,211,559 apache-tomcat-8.5.33.zip
08/29/2018  06:54 AM               849 apache-tomcat-8.5.33.zip.asc
08/29/2018  06:54 AM               154 apache-tomcat-8.5.33.zip.sha512
08/29/2018  06:54 AM         9,621,331 apache-tomcat-8.5.33.tar.gz
08/29/2018  06:54 AM               849 apache-tomcat-8.5.33.tar.gz.asc
08/29/2018  06:55 AM               157 apache-tomcat-8.5.33.tar.gz.sha512
08/29/2018  06:55 AM        10,936,767 apache-tomcat-8.5.33-windows-x86.zip
08/29/2018  06:55 AM               849 apache-tomcat-8.5.33-windows-x86.zip.asc
08/29/2018  06:55 AM               166 apache-tomcat-8.5.33-windows-x86.zip.sha512
08/29/2018  06:56 AM        11,232,621 apache-tomcat-8.5.33-windows-x64.zip
08/29/2018  06:56 AM               849 apache-tomcat-8.5.33-windows-x64.zip.asc
08/29/2018  06:56 AM               166 apache-tomcat-8.5.33-windows-x64.zip.sha512
08/29/2018  06:57 AM         9,895,312 apache-tomcat-8.5.33.exe
08/29/2018  06:57 AM               849 apache-tomcat-8.5.33.exe.asc
08/29/2018  06:57 AM               154 apache-tomcat-8.5.33.exe.sha512
08/29/2018  07:01 AM        10,514,400 apache-tomcat-9.0.11.zip
08/29/2018  07:02 AM               849 apache-tomcat-9.0.11.zip.asc
08/29/2018  07:02 AM               154 apache-tomcat-9.0.11.zip.sha512
08/29/2018  07:02 AM         9,904,915 apache-tomcat-9.0.11.tar.gz
08/29/2018  07:03 AM               849 apache-tomcat-9.0.11.tar.gz.asc
08/29/2018  07:03 AM               157 apache-tomcat-9.0.11.tar.gz.sha512
08/29/2018  07:03 AM        11,239,606 apache-tomcat-9.0.11-windows-x86.zip
08/29/2018  07:03 AM               849 apache-tomcat-9.0.11-windows-x86.zip.asc
08/29/2018  07:04 AM               166 apache-tomcat-9.0.11-windows-x86.zip.sha512
08/29/2018  07:04 AM        11,535,460 apache-tomcat-9.0.11-windows-x64.zip
08/29/2018  07:04 AM               849 apache-tomcat-9.0.11-windows-x64.zip.asc
08/29/2018  07:04 AM               166 apache-tomcat-9.0.11-windows-x64.zip.sha512
08/29/2018  07:04 AM        10,246,376 apache-tomcat-9.0.11.exe
08/29/2018  07:04 AM               849 apache-tomcat-9.0.11.exe.asc
08/29/2018  07:05 AM               154 apache-tomcat-9.0.11.exe.sha512
```

Looking further into the 32-bit vs 64-bit tomcat issue, I decided to look at the Windows Registry for the JDK keys associated with my installation of (multiple version) Oracle's Java JDK.  Note that I have never installed a 32-bit version of the JDK on my Windows 10 Dell XPS15 laptops.  Also note that I have never explicitly installed the Java JRE on this laptop (though installing the JDK results in the installation of the JRE).

```
HKEY_LOCAL_MACHINE\SOFTWARE\JavaSoft\Java Development Kit\1.8.0_131
HKEY_LOCAL_MACHINE\SOFTWARE\JavaSoft\Java Development Kit\1.8.0_144
HKEY_LOCAL_MACHINE\SOFTWARE\JavaSoft\Java Development Kit\1.8.0_162
HKEY_LOCAL_MACHINE\SOFTWARE\JavaSoft\Java Development Kit\1.8.0_172

HKEY_LOCAL_MACHINE\SOFTWARE\JavaSoft\Java Runtime Environment\1.8.0_131
HKEY_LOCAL_MACHINE\SOFTWARE\JavaSoft\Java Runtime Environment\1.8.0_144
HKEY_LOCAL_MACHINE\SOFTWARE\JavaSoft\Java Runtime Environment\1.8.0_162
HKEY_LOCAL_MACHINE\SOFTWARE\JavaSoft\Java Runtime Environment\1.8.0_172

HKEY_LOCAL_MACHINE\SOFTWARE\JavaSoft\JDK\9.0.4
HKEY_LOCAL_MACHINE\SOFTWARE\JavaSoft\JDK\10.0.1

HKEY_LOCAL_MACHINE\SOFTWARE\JavaSoft\JRE\9.0.4
HKEY_LOCAL_MACHINE\SOFTWARE\JavaSoft\JDK\10.0.1

HKEY_LOCAL_MACHINE\SOFTWARE\WOW6432Node\JavaSoft
```

As to where I installed Java (the default location or a location of my choosing), I have had a different approach for some of the JDK installations I have performed.

```
C:\Program Files\Java>dir /o:gd
 Volume in drive C has no label.
 Volume Serial Number is 4603-A8D3

 Directory of C:\Program Files\Java

06/08/2017  02:35 PM    <DIR>          jre1.8.0_131
06/08/2017  02:35 PM    <DIR>          jdk1.8.0_131
03/15/2018  09:42 AM    <DIR>          jdk1.8.0_162
03/15/2018  09:44 AM    <DIR>          ..
03/15/2018  09:44 AM    <DIR>          .
03/15/2018  09:47 AM    <DIR>          jdk-9.0.4
               0 File(s)              0 bytes
               6 Dir(s)  371,690,299,392 bytes free

C:\Program Files\Java>

C:\LocalApps\Java>dir /o:gd
 Volume in drive C has no label.
 Volume Serial Number is 4603-A8D3

 Directory of C:\LocalApps\Java

03/15/2018  09:38 AM    <DIR>          jre1.8.0_144
03/15/2018  09:38 AM    <DIR>          jdk1.8.0_144
03/15/2018  09:42 AM    <DIR>          jre1.8.0_162
03/15/2018  09:47 AM    <DIR>          jre-9.0.4
03/15/2018  09:52 AM    <DIR>          jre1.8.0_131
03/15/2018  09:52 AM    <DIR>          jdk1.8.0_131
03/15/2018  09:53 AM    <DIR>          jdk1.8.0_162
03/15/2018  09:53 AM    <DIR>          jdk-9.0.4
06/19/2018  03:57 PM    <DIR>          jre-10.0.1
06/19/2018  03:58 PM    <DIR>          jdk-10.0.1
06/19/2018  06:24 PM    <DIR>          ..
06/19/2018  06:24 PM    <DIR>          .
06/19/2018  06:24 PM    <DIR>          jre1.8.0_172
06/19/2018  06:24 PM    <DIR>          jdk1.8.0_172
               0 File(s)              0 bytes
              14 Dir(s)  371,689,791,488 bytes free

C:\LocalApps\Java>
```

```
C:\Users\David Holberton\Downloads>dir  /o:gd jdk-*-x64.exe
 Volume in drive C has no label.
 Volume Serial Number is 4603-A8D3

 Directory of C:\Users\David Holberton\Downloads

06/08/2017  08:35 AM       207,649,848 jdk-8u131-windows-x64.exe
08/02/2017  06:21 AM       207,382,584 jdk-8u144-windows-x64.exe
08/02/2017  06:29 AM       207,387,192 jdk-8u141-windows-x64.exe
08/02/2017  06:31 AM       205,004,856 jdk-8u121-windows-x64.exe
08/02/2017  06:35 AM       204,607,032 jdk-8u112-windows-x64.exe
08/02/2017  06:37 AM       204,139,576 jdk-8u102-windows-x64.exe
08/02/2017  06:39 AM       146,893,216 jdk-7u80-windows-x64.exe
08/02/2017  06:40 AM       146,861,984 jdk-7u79-windows-x64.exe
03/15/2018  08:01 AM       216,544,312 jdk-8u161-windows-x64.exe
03/15/2018  08:04 AM       216,804,920 jdk-8u162-windows-x64.exe
05/30/2018  06:11 AM       217,342,912 jdk-8u171-windows-x64.exe
05/30/2018  06:12 AM       217,370,560 jdk-8u172-windows-x64.exe
07/24/2018  07:34 AM       212,582,768 jdk-8u181-windows-x64.exe
              13 File(s)  2,610,571,760 bytes
               0 Dir(s)  371,693,105,152 bytes free

C:\Users\David Holberton\Downloads>
```
