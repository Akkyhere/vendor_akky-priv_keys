# Personal-priv_keys-template

# Usage

```bash
git clone https://github.com/Akkyhere/vendor_akky-priv_keys vendor/akky-priv/keys
```

```bash
cd vendor/akky-priv/keys
```

```
./keys.sh
```

# Testing

Included `check_keys.py` script checks whether all apk/apex/capex files in the build out are signed with keys within its directory. Be aware that some targets are **expected** to be signed with vendor key, for example `com.android.apex.cts.shim.v1_prebuilt`.

```
$ ./check_keys.py ~/your_rom/out/target/product/device_codename
/home/ab/your_rom/out/target/product/device_codename/obj/ETC/com.android.apex.cts.shim.v1_prebuilt_intermediates/com.android.apex.cts.shim.apex is signed with an unknown key!
```


@Credits: Evolution X
