# Ubuntu tips

## macOS远程桌面连接到Ubuntu

1. 配置`Desktop sharing`

   ![desktop sharing setup](resources/desktop-sharing.png)

   `Require the user to enter this password`必须要填一个密码。

2. 安装`dconf-editor`

   ```shell
   sudo apt install dconf-editor
   ```

3. 禁用加密，取消勾选`require-encryption`

   ![disable encryption](resources/disable-encryption.png)

4. 使用macOS自带的`Screen sharing`应用连接，输入密码为步骤1中设置的密码

   ```shell
   vnc://allen@192.168.1.23
   ```

   