# ATEN CN8000 Java Viewer downloader/launcher

Launch the KVM viewer applet without using a web browser:

```shell-session
USER=... PASS=... cn8000 <host>
```

The script detects the CN8000 KVM type ("older"/"newer"), logs in to the web interface, downloads the JNLP file, and launches it.

The script is self-explanatory. You may need to install Oracle/Sun Java 6, 7, or 8 and set the `JAVAWS` variable accordingly, or configure IcedTea/OpenJDK to allow TLS 1.0 (likely impossible).

You may also need to run Java’s `bin/jcontrol` and, in the "Security" tab, add your KVM to the exception list.

Open an issue if the script doesn't work for your CN8000.
