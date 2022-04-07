## Builing

```
cmake \
              -DCMAKE_INSTALL_PREFIX=/usr \
              -DFORCE_COMPILE_FROM_TRUNK=TRUE \
              -DSTATE_INSTALL_DIR='/var/lib/telldus' \
              .
```

## Testing

Create /etc/tellstick.conf

mkdir /var/lib/telldus
chown $USER /var/lib/telldus

./service/telldusd --nodaemon --debug

/tdtool/tdtool --list
