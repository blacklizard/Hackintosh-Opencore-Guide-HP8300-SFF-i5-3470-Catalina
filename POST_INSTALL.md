# Post Install

## For sleep to work properly

```
sudo pmset hibernatemode 0
sudo pmset proximitywake 0
```

## iServices
To make sure you will be able to get iServices to work, skip signing in during installtion process.\
Generate an invalid serial using `GenSMBIOS` for `iMac15,1`, be really sure that the generated serial is invalid by cross checking it in apple webiste.

Once its validated to be invalid, use the generated serial, board serial and SmUUID in your `config.plist` under `PlatformInfo` section.\

Restart and sign in to your apple account, you should be able to use all the iServices
