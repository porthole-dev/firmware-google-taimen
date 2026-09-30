# Pixel 2 XL firmware from the Google factory image

[Website](https://porthole-dev.github.io/porthole/) · [Downloads](https://porthole-dev.github.io/porthole/images/) · [Device support](https://porthole-dev.github.io/porthole/devices/)

This repository holds the Taimen modem files and optional fingerprint trustlet
that are absent from TheMuppets' vendor tree. The Nura `firmware-google-taimen`
aport uses these files alongside the pinned TheMuppets source.

The inputs were extracted from Google's final Pixel 2 XL factory archive,
`taimen-rp1a.201005.004.a1-factory-2f5c4987.zip`. The modem files came from
`radio-taimen-g8998-00034-2006052136.img`; the fingerprint files came from
`vendor.img`. `modem.mbn` was assembled from `modem.mdt` and its segments with
`pil-squasher`. `SHA256SUMS` records every published byte.

The fingerprint trustlet remains an optional APK subpackage. Installing it
does not prove the sensor works; hardware validation is still required.
