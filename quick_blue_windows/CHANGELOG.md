## 0.3.2+3

- Windows: catch `winrt::hresult_error` in every `fire_and_forget` coroutine. An exception escaping one (e.g. `FromBluetoothAddressAsync` returning E_FAIL during a scan) called `winrt::terminate` and fail-fasted the host process (0xC000027B). Scan results now fall back to the advertisement `LocalName`; a failed connect reports `disconnected` instead of hanging.

## [0.3.2+2] - 2022.5.18

- Revert to 0.3.2

## [0.3.2+1] - 2022.5.18

- Fix discoverServices on Windows

## [0.3.2] - 2022.3.22

- Refactor `manufacturerData` to `manufacturerDataHead`

## [0.3.1+1] - 2022.3.10

- Fix version typo
- Fix missing writeOptions on Windows

## [0.3.1] - 2022.3.10

- Impl `readValue`

## [0.3.0-dev.0] - 2022.3.3

- Migerate to Null-Safety

## [0.2.0] - 2020.11.22

- Impl `connect` & `disconnect`
- Impl `onConnectionChanged`

- Impl `discoverServices` with `TODO`

- Impl `writeValue`

- Impl `setNotifiable`
- Impl `onValueChanged`

## 0.1.1 - 2020.11.17

* Impl `scanResultStream`

## 0.1.0 - 2020.11.11

* Impl `startScan` & `stopScan`
