# Ubuntu-Note

## fcitx5

```
sudo apt install 'fcitx5*' kde-config-fcitx5
```

- 在 ~/.pam_environment 文件中尾部插入：
```
 GTK_IM_MODULE DEFAULT=fcitx5
 QT_IM_MODULE  DEFAULT=fcitx5
 XMODIFIERS    DEFAULT=@im=fcitx5
```

-Certain distribution may not provide such a file. If not, you can simply copy /usr/share/applications/org.fcitx.Fcitx5.desktop to ~/.config/autostart
```
mkdir -p ~/.config/autostart && cp /usr/share/applications/org.fcitx.Fcitx5.desktop ~/.config/autostart
```
