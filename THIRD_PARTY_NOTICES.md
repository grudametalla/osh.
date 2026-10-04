# Сторонние компоненты и исходный код

**Русский** · [English](THIRD_PARTY_NOTICES_EN.md)

osh. является закрытым приложением, но включает сторонние компоненты
с собственными лицензиями. Наличие этих лицензий не означает, что весь
закрытый код osh. распространяется на их условиях; обязательства применяются
к соответствующим компонентам согласно тексту каждой лицензии.

## UniFFI

Android-сборка использует UniFFI 0.32.0 под MPL-2.0:
`uniffi`, `uniffi_core`, `uniffi_internal_macros`, `uniffi_macros`,
`uniffi_meta` и `uniffi_pipeline`.

Исходный код соответствующей версии доступен в upstream-репозитории:
https://github.com/mozilla/uniffi-rs

Точная версия: `v0.32.0`.
Закреплённый commit:
`5c7b73906358e1a7acdc1bdc7bf5cd86fb27e44c`.

Архив исходного кода:
https://github.com/mozilla/uniffi-rs/archive/refs/tags/v0.32.0.tar.gz

Текст MPL-2.0 и эти же инструкции также включены непосредственно в APK.

## Другие компоненты

В APK также присутствуют лицензии/уведомления для ByeDPI, HEV socks5 tunnel,
JNA и runtime-зависимостей Android/Rust. Release-gate проверяет наличие
и целостность этих notice-файлов в каждой публикуемой сборке.
