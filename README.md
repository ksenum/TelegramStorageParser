# TelegramDesktopLocalStorage
Program to decrypt and parse Telegram Desktop's storage

This project relies on OpenSSL for AES-IGE and PBKDF2 implementations. See their [license here](https://www.openssl.org/source/license.txt).

To use copy the tdata directory (found in "AppData\Roaming\Telegram Desktop" by default) into the working directory or change the location in the Constants.cs file.

Useful references - Telegram Desktop source code:
Most relevant files:
-[localstorage.cpp](https://github.com/telegramdesktop/tdesktop/blob/dev/Telegram/SourceFiles/storage/localstorage.cpp)
-[auth_key.cpp](https://github.com/telegramdesktop/tdesktop/blob/dev/Telegram/SourceFiles/mtproto/auth_key.cpp)
-[auth_key.h](https://github.com/telegramdesktop/tdesktop/blob/dev/Telegram/SourceFiles/mtproto/auth_key.h)

MapPasscodeBruteForce.cs coitains a sample implementation for brute forcing a passcode by eliminating as much excess code as possible