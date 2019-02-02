
## librdkafka
Cloned as a git submodule. 
```
git clone https://github.com/edenhill/librdkafka gmod/librdkfaka
```
Then
```
echo "Setting up librdkafka"
cd gmod/librdkfaka
./configure
make
sudo make install
cd ..
```



### Make Install output

(env) cicorias@cicoria-stealth2:/c/g/junk/eh-kafka/gmod/librdkafka$ sudo make install
[sudo] password for cicorias:
make[1]: Entering directory '/c/g/junk/eh-kafka/gmod/librdkafka/src'
Install librdkafka to /usr/local
install -d $DESTDIR/usr/local/include/librdkafka && \
install -d $DESTDIR/usr/local/lib && \
install rdkafka.h $DESTDIR/usr/local/include/librdkafka && \
install librdkafka.a $DESTDIR/usr/local/lib && \
install librdkafka.so.1 $DESTDIR/usr/local/lib && \
[ -f "rdkafka.pc" ] && ( \
        install -d $DESTDIR/usr/local/lib/pkgconfig && \
        install -m 0644 rdkafka.pc $DESTDIR/usr/local/lib/pkgconfig \
) && \
[ -f "rdkafka-static.pc" ] && ( \
        install -d $DESTDIR/usr/local/lib/pkgconfig && \
        install -m 0644 rdkafka-static.pc $DESTDIR/usr/local/lib/pkgconfig \
) && \
(cd $DESTDIR/usr/local/lib && ln -sf librdkafka.so.1 librdkafka.so)
make[1]: Leaving directory '/c/g/junk/eh-kafka/gmod/librdkafka/src'
make[1]: Entering directory '/c/g/junk/eh-kafka/gmod/librdkafka/src-cpp'
Install librdkafka++ to /usr/local
install -d $DESTDIR/usr/local/include/librdkafka && \
install -d $DESTDIR/usr/local/lib && \
install rdkafkacpp.h $DESTDIR/usr/local/include/librdkafka && \
install librdkafka++.a $DESTDIR/usr/local/lib && \
install librdkafka++.so.1 $DESTDIR/usr/local/lib && \
[ -f "rdkafka++.pc" ] && ( \
        install -d $DESTDIR/usr/local/lib/pkgconfig && \
        install -m 0644 rdkafka++.pc $DESTDIR/usr/local/lib/pkgconfig \
) && \
[ -f "rdkafka++-static.pc" ] && ( \
        install -d $DESTDIR/usr/local/lib/pkgconfig && \
        install -m 0644 rdkafka++-static.pc $DESTDIR/usr/local/lib/pkgconfig \
) && \
(cd $DESTDIR/usr/local/lib && ln -sf librdkafka++.so.1 librdkafka++.so)
make[1]: Leaving directory '/c/g/junk/eh-kafka/gmod/librdkafka/src-cpp'
(env) cicorias@cicoria-stealth2:/c/g/junk/eh-kafka/gmod/librdkafka$ ls -alt /usr/local | head -n 40

