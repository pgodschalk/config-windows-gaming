# Windows and application settings

<!-- markdownlint-disable MD024 -->

## Installation

- Ethernet physically disconnected
- Create maximum size NTFS partition

| Key                      | Value                   | Explanation |
| ------------------------ | ----------------------- | ----------- |
| Language to install      | English (United States) |             |
| Time and currency format | English (United States) |             |

<!-- markdownlint-disable MD013 -->

| Key                                                | Value            | Explanation |
| -------------------------------------------------- | ---------------- | ----------- |
| Is this the right country or region?               | Netherlands      |             |
| Is this the right keyboard layout or input method? | US-International |             |

<!-- markdownlint-enable MD013 -->

| Key                                        | Value | Explanation |
| ------------------------------------------ | ----- | ----------- |
| Enable Defender (recommended)              | True  |             |
| Default Windows Mitigations (recommended)  | True  |             |
| Disable Automatic Windows Updates          | True  |             |
| Disable Hibernation                        | True  |             |
| Maximum Performance (Disable Power Saving) | False |             |
| Disable Core Isolation                     | False |             |
| Remove Snipping Tool App                   | False |             |
| Remove Microsoft Edge                      | False |             |
| Install a Browser                          | False |             |
| Install Atlas Toolbox                      | True  |             |

Process idle tasks manually:

```powershell
Rundll32.exe advapi32.dll,ProcessIdleTasks
```

Disable co-installers:

<!-- markdownlint-disable MD013 -->

```powershell
Set-ItemProperty `
  -Path 'HKLM:\SOFTWARE\Microsoft\Windows\CurrentVersion\Device Installer' `
  -Name 'DisableCoInstallers' `
  -Value 1 `
  -Type DWord
```

<!-- markdownlint-enable MD013 -->

Ethernet reconnected again at this point.

## Windows Settings

### System

#### Display

##### HDR

<!-- markdownlint-disable MD013 -->

| Key                                                              | Value | Explanation |
| ---------------------------------------------------------------- | ----- | ----------- |
| HDR                                                              | On    |             |
| Turn off HDR when my PC is running on battery to help save power | False |             |
| Auto HDR                                                         | Off   |             |
| SDR content brightness                                           | 50    |             |

<!-- markdownlint-enable MD013 -->

#### Sound

##### Output

###### SteelSeries Alias Pro Stream

<!-- markdownlint-disable MD013 -->

| Key                         | Value                                         | Explanation |
| --------------------------- | --------------------------------------------- | ----------- |
| Set as default sound device | Not used as a default                         |             |
| Format                      | 2 channels, 24 bit, 48000 Hz (Studio Quality) |             |
| Spatial sound               | Off                                           |             |

<!-- markdownlint-enable MD013 -->

###### SteelSeries Sonar - Microphone

<!-- markdownlint-disable MD013 -->

| Key                         | Value                                         | Explanation |
| --------------------------- | --------------------------------------------- | ----------- |
| Set as default sound device | Not used as a default                         |             |
| Format                      | 2 channels, 24 bit, 48000 Hz (Studio Quality) |             |
| Spatial sound               | Off                                           |             |

<!-- markdownlint-enable MD013 -->

###### Headphones

<!-- markdownlint-disable MD013 -->

| Key                         | Value                                         | Explanation |
| --------------------------- | --------------------------------------------- | ----------- |
| Set as default sound device | Not used as a default                         |             |
| Format                      | 2 channels, 24 bit, 48000 Hz (Studio Quality) |             |
| Audio enhancements          | Off                                           |             |
| Spatial sound               | Off                                           |             |

<!-- markdownlint-enable MD013 -->

###### SteelSeries Sonar - Stream

<!-- markdownlint-disable MD013 -->

| Key                         | Value                                         | Explanation |
| --------------------------- | --------------------------------------------- | ----------- |
| Set as default sound device | Not used as a default                         |             |
| Format                      | 2 channels, 24 bit, 48000 Hz (Studio Quality) |             |
| Spatial sound               | Off                                           |             |

<!-- markdownlint-enable MD013 -->

###### SteelSeries Sonar - Media

<!-- markdownlint-disable MD013 -->

| Key                         | Value                                         | Explanation |
| --------------------------- | --------------------------------------------- | ----------- |
| Set as default sound device | Is default for audio                          |             |
| Format                      | 8 channels, 24 bit, 96000 Hz (Studio Quality) |             |
| Audio enhancements          | Off                                           |             |

<!-- markdownlint-enable MD013 -->

###### SteelSeries Alias Pro Personal

<!-- markdownlint-disable MD013 -->

| Key                         | Value                                         | Explanation |
| --------------------------- | --------------------------------------------- | ----------- |
| Set as default sound device | Not used as a default                         |             |
| Format                      | 2 channels, 24 bit, 48000 Hz (Studio Quality) |             |
| Audio enhancements          | Off                                           |             |
| Spatial sound               | Off                                           |             |

<!-- markdownlint-enable MD013 -->

###### SteelSeries Sonar - Gaming

<!-- markdownlint-disable MD013 -->

| Key                         | Value                                         | Explanation |
| --------------------------- | --------------------------------------------- | ----------- |
| Set as default sound device | Is default for audio                          |             |
| Format                      | 8 channels, 24 bit, 96000 Hz (Studio Quality) |             |
| Audio enhancements          | Off                                           |             |

<!-- markdownlint-enable MD013 -->

###### SteelSeries Sonar - Chat

<!-- markdownlint-disable MD013 -->

| Key                         | Value                                         | Explanation |
| --------------------------- | --------------------------------------------- | ----------- |
| Set as default sound device | Is default for communications                 |             |
| Format                      | 2 channels, 24 bit, 48000 Hz (Studio Quality) |             |
| Spatial sound               | Off                                           |             |

<!-- markdownlint-enable MD013 -->

###### SteelSeries Sonar - Aux

<!-- markdownlint-disable MD013 -->

| Key                         | Value                                         | Explanation |
| --------------------------- | --------------------------------------------- | ----------- |
| Set as default sound device | Is default for audio                          |             |
| Format                      | 8 channels, 24 bit, 96000 Hz (Studio Quality) |             |
| Audio enhancements          | Off                                           |             |

<!-- markdownlint-enable MD013 -->

##### Input

<!-- markdownlint-disable MD013 -->

###### SteelSeries Sonar - Stream

| Key                         | Value                                         | Explanation |
| --------------------------- | --------------------------------------------- | ----------- |
| Set as default sound device | Not used as a default                         |             |
| Format                      | 2 channels, 24 bit, 48000 Hz (Studio Quality) |             |

<!-- markdownlint-enable MD013 -->

###### SteelSeries Sonar - Microphone

| Key    | Value                                         | Explanation |
| ------ | --------------------------------------------- | ----------- |
| Format | 2 channels, 24 bit, 48000 Hz (Studio Quality) |             |

###### SteelSeries Alias Pro Input

<!-- markdownlint-disable MD013 -->

| Key                         | Value                                         | Explanation |
| --------------------------- | --------------------------------------------- | ----------- |
| Set as default sound device | Not used as a default                         |             |
| Format                      | 2 channels, 24 bit, 48000 Hz (Studio Quality) |             |
| Audio enhancements          | Off                                           |             |

<!-- markdownlint-enable MD013 -->

###### Microphone

| Key   | Value       | Explanation |
| ----- | ----------- | ----------- |
| Audio | Don't allow |             |

#### Power

| Key                     | Value    | Explanation |
| ----------------------- | -------- | ----------- |
| Power Mode (Plugged in) | Balanced |             |

##### Screen, sleep & hibernate timeouts

| Key                        | Value | Explanation |
| -------------------------- | ----- | ----------- |
| Turn my screen off after   | Never |             |
| Make my device sleep after | Never |             |

#### Storage

| Key           | Value | Explanation |
| ------------- | ----- | ----------- |
| Storage Sense | Off   |             |

#### Advanced

##### Terminal

<!-- markdownlint-disable MD013 -->

| Key                                                                                                                   | Value            | Explanation |
| --------------------------------------------------------------------------------------------------------------------- | ---------------- | ----------- |
| Terminal                                                                                                              | Windows Terminal |             |
| Change execution policy to allow local PowerShell scripts to run without signing. Require signing for remote scripts. | On               |             |
| Enable sudo                                                                                                           | On               |             |
| Configure how sudo runs applications                                                                                  | Inline           |             |

<!-- markdownlint-enable MD013 -->

#### Troubleshoot

| Key                                    | Value         | Explanation |
| -------------------------------------- | ------------- | ----------- |
| Recommended troubleshooter preferences | Don't run any |             |

#### Clipboard

| Key               | Value | Explanation |
| ----------------- | ----- | ----------- |
| Clipboard history | On    |             |

#### About

##### System Properties

###### Startup and Recovery

| Key                              | Value                      | Explanation |
| -------------------------------- | -------------------------- | ----------- |
| Write an event to the system log | True                       |             |
| Automatically restart            | False                      |             |
| Write debugging information      | Small memory dump (256 KB) |             |

### Bluetooth & Devices

#### Mouse

| Key                       | Value | Explanation |
| ------------------------- | ----- | ----------- |
| Mouse pointer speed       | 10    |             |
| Enhance pointer precision | Off   |             |

### Network & internet

#### Ethernet

| Key                  | Value           | Explanation |
| -------------------- | --------------- | ----------- |
| Network profile type | Private network |             |

### Apps

#### Startup

| Key                         | Value | Explanation |
| --------------------------- | ----- | ----------- |
| 1Password                   | Off   |             |
| Apple Mobile Device Process | Off   |             |
| G HUB                       | Off   |             |
| Terminal                    | Off   |             |
| Xbox                        | Off   |             |

#### Resume

| Key    | Value | Explanation |
| ------ | ----- | ----------- |
| Resume | Off   |             |

### Accounts

#### Passkeys

##### Advanced options

| Key       | Value | Explanation |
| --------- | ----- | ----------- |
| 1Password | On    |             |

### Accessibility

#### Mouse pointer and touch

| Key                 | Value  | Explanation |
| ------------------- | ------ | ----------- |
| Mouse pointer style | Custom |             |
| Recommended colors  | Yellow |             |

### Windows Update

#### Advanced options

| Key                                          | Value | Explanation |
| -------------------------------------------- | ----- | ----------- |
| Receive updates for other Microsoft products | On    |             |

## Control Panel

### BitLocker Drive Encryption

| Key       | Value | Explanation |
| --------- | ----- | ----------- |
| BitLocker | Off   |             |

## Device Manager

```powershell
# Disable power-down on every device that has the option
$devices = Get-PnpDevice | Where-Object {$_.Status -eq "OK"}

foreach ($device in $devices) {
  $deviceProperties = Get-PnpDeviceProperty `
    -InstanceId $device.InstanceId `
    -ErrorAction SilentlyContinue

  # Check if device has DEVPKEY_Device_PowerData with selective suspend
  # capability
  $powerCfg = (Get-CimInstance `
    -ClassName MSPower_DeviceEnable `
    -Namespace root\wmi `
    -ErrorAction SilentlyContinue |
    Where-Object {
      $_.InstanceName -like "*$($device.InstanceId)*"
    })

  if ($powerCfg -and $powerCfg.Enable) {
    try {
      $powerCfg.Enable = $false
      $powerCfg | Set-CimInstance
      Write-Host `
        "Disabled power-save on: $($device.FriendlyName)" `
        -ForegroundColor Green
    } catch {
      # Some devices don't support the change
    }
  }
}
```

### Network adapters

```powershell
$mmProfile = "HKLM:\SOFTWARE\Microsoft\Windows NT\CurrentVersion\Multimedia" + `
  "\SystemProfile"
Set-ItemProperty `
  -Path $mmProfile `
  -Name "NetworkThrottlingIndex" `
  -Value 0xFFFFFFFF `
  -Type DWord
```

#### Realtek Gaming 2.5GbE Family Controller

```powershell
Set-NetAdapterRSS -Name "Ethernet" `
  -BaseProcessorNumber 4 `
  -MaxProcessors 4 `
  -NumberOfReceiveQueues 4
```

#### Advanced

| Key                   | Value    | Explanation |
| --------------------- | -------- | ----------- |
| Green Ethernet        | Disabled |             |
| Power Saving Mode     | Disabled |             |
| Receive Buffers       | 2048     |             |
| Transmit Buffers      | 2048     |             |
| Wake on Magic Packet  | Disabled |             |
| Wake on pattern match | Disabled |             |

##### Power Management

<!-- markdownlint-disable MD013 -->

| Key                                                      | Value | Explanation |
| -------------------------------------------------------- | ----- | ----------- |
| Allow the computer to turn off this device to save power | Off   |             |

<!-- markdownlint-enable MD013 -->

## Power Options

### HYDRA - Change plan settings

#### Change advanced power settings

##### Hard disk

| Key                      | Value | Explanation |
| ------------------------ | ----- | ----------- |
| Turn off hard disk after | 0     |             |

##### USB settings

| Key                           | Value    | Explanation |
| ----------------------------- | -------- | ----------- |
| USB selective suspend setting | Disabled |             |

## Explorer

### Local Disk (C:)

#### Tools

##### Optimize Drives

###### Scheduled optimization

| Key       | Value | Explanation |
| --------- | ----- | ----------- |
| Frequency | Daily |             |

### Game Bar

#### Gaming Copilot

##### Privacy settings

| Key                        | Value | Explanation |
| -------------------------- | ----- | ----------- |
| Model training on text     | False |             |
| Model training on voice    | False |             |
| Personalization and memory | True  |             |

##### Hardware and hotkeys

| Key                         | Value | Explanation |
| --------------------------- | ----- | ----------- |
| Enable Push to Talk keybind | False |             |
| Enable launch app keybind   | False |             |

## HEVC Video Extensions

```powershell
winget install 9NMZLZ57R3T7
```

## Local Security Policy

### Security Settings

#### Local Policies

##### User Rights Assignment

| Key        | Value                             | Explanation           |
| ---------- | --------------------------------- | --------------------- |
| Principals | Administrators, Patrick Godschalk | Required for TestMem5 |

## Notepad

### Text Formatting

#### Font

| Key    | Value                   | Explanation |
| ------ | ----------------------- | ----------- |
| Family | JetBrainsMono Nerd Font |             |

#### Spelling

| Key         | Value | Explanation |
| ----------- | ----- | ----------- |
| Autocorrect | Off   |             |

## PowerShell

```powershell
winget install 9MZ2SNWT0N5D
```

## Services

| Name                          | Startup Type | Explanation |
| ----------------------------- | ------------ | ----------- |
| Flydigi Space Station Service | Manual       |             |
| LGHUB Updater Service         | Manual       |             |
| Logitech LampArray Service    | Manual       |             |
| Print Spooler                 | Manual       |             |
| Razer Game Manager Service    | Manual       |             |

## Terminal

See [dotfiles](https://github.com/pgodschalk/dotfiles)

## Visual Studio Code

```powershell
winget install Microsoft.VisualStudioCode
```

See [dotfiles](https://github.com/pgodschalk/dotfiles)

### Windows HDR Calibration

```powershell
winget install 9N7F2SM5D1LR
```

<!-- markdownlint-disable MD013 -->

| Key                           | Value                                  | Explanation |
| ----------------------------- | -------------------------------------- | ----------- |
| Minimum Luminance             | 0.0000                                 |             |
| Maximum Luminance             | 630                                    |             |
| Max Full Frame Luminance Test | 630                                    |             |
| Color Saturation              | 50                                     |             |
| Profile name                  | HDR Calibrated Profile \<date\> \<id\> |             |

<!-- markdownlint-enable MD013 -->

## Windows Security

```powershell
Add-MpPreference -ExclusionPath $env:LOCALAPPDATA"\NVIDIA\DXCache"
Add-MpPreference -ExclusionPath $env:LOCALAPPDATA"\NVIDIA\GLCache"
Add-MpPreference -ExclusionPath $env:LOCALAPPDATA"\AMD\DX9Cache"
Add-MpPreference -ExclusionPath $env:LOCALAPPDATA"\AMD\DxCache"
Add-MpPreference -ExclusionPath $env:LOCALAPPDATA"\AMD\DxcCache"
Add-MpPreference -ExclusionPath $env:LOCALAPPDATA"\AMD\OglCache"
Add-MpPreference -ExclusionPath `
  $env:windir"\SoftwareDistribution\Datastore\Datastore.edb"
Add-MpPreference -ExclusionPath `
  $env:windir"\SoftwareDistribution\Datastore\Logs\Edb*.jrs"
Add-MpPreference -ExclusionPath `
  $env:windir"\SoftwareDistribution\Datastore\Logs\Edb.chk"
Add-MpPreference -ExclusionPath `
  $env:windir"\SoftwareDistribution\Datastore\Logs\Tmp.edb"
Add-MpPreference -ExclusionPath `
  $env:windir"\SoftwareDistribution\Datastore\Logs\*.log"
Add-MpPreference -ExclusionPath $env:windir"\Security\Database\*.edb"
Add-MpPreference -ExclusionPath $env:windir"\Security\Database\*.sdb"
Add-MpPreference -ExclusionPath $env:windir"\Security\Database\*.log"
Add-MpPreference -ExclusionPath $env:windir"\Security\Database\*.chk"
Add-MpPreference -ExclusionPath $env:windir"\Security\Database\*.jrs"
Add-MpPreference -ExclusionPath $env:windir"\Security\Database\*.xml"
Add-MpPreference -ExclusionPath $env:windir"\Security\Database\*.csv"
Add-MpPreference -ExclusionPath $env:windir"\Security\Database\*.cmtx"
Add-MpPreference -ExclusionPath `
  $env:SystemRoot"\System32\GroupPolicy\Machine\Registry.pol"
Add-MpPreference -ExclusionPath `
  $env:SystemRoot"\System32\GroupPolicy\Machine\Registry.tmp"
Add-MpPreference -ExclusionPath $env:userprofile"\NTUser.dat"
Add-MpPreference -ExclusionPath $env:SystemRoot"\System32\sru\*.log"
Add-MpPreference -ExclusionPath $env:SystemRoot"\System32\sru\*.dat"
Add-MpPreference -ExclusionPath $env:SystemRoot"\System32\sru\*.chk"
Add-MpPreference -ExclusionPath `
  $env:SystemRoot"\System32\Configuration\MetaConfig.mof"
Add-MpPreference -ExclusionPath `
  $env:SystemRoot"\System32\winevt\Logs\*.evtx"
Add-MpPreference -ExclusionPath $env:windir"\apppatch\sysmain.sdb"
Add-MpPreference -ExclusionPath $env:windir"\EventLog\Data\lastalive?.dat"
Add-MpPreference -ExclusionProcess ${env:ProgramFiles(x86)}("\Windows Kits" + `
  "\10\Windows Performance Toolkit\WPRUI.exe")
Add-MpPreference -ExclusionProcess ${env:ProgramFiles(x86)}("\Windows Kits" + `
  "\10\Windows Performance Toolkit\wpa.exe")
Add-MpPreference -ExclusionPath `
  $env:SystemRoot"\System32\WindowsPowerShell\v1.0\Modules"
Add-MpPreference -ExclusionPath `
  $env:SystemRoot"\System32\Configuration\DSCStatusHistory.mof"
Add-MpPreference -ExclusionPath `
  $env:SystemRoot"\System32\Configuration\DSCEngineCache.mof"
Add-MpPreference -ExclusionPath `
  $env:SystemRoot"\System32\Configuration\DSCResourceStateCache.mof"
Add-MpPreference -ExclusionPath `
  $env:SystemRoot"\System32\Configuration\ConfigurationStatus"
Add-MpPreference -ExclusionPath "$env:LOCALAPPDATA\D3DSCache"
Add-MpPreference -ExclusionPath "$env:USERPROFILE\Documents\My Games"
```

### Virus & threat protection settings

| Key                         | Value | Explanation |
| --------------------------- | ----- | ----------- |
| Real-time protection        | On    |             |
| Dev Drive protection        | On    |             |
| Cloud-delivered protection  | On    |             |
| Automatic sample submission | On    |             |
| Tamper Protection           | On    |             |

#### Ransomware protection

| Key                      | Value | Explanation |
| ------------------------ | ----- | ----------- |
| Controlled folder access | Off   |             |

### App & browser control

#### Smart App Control

| Key               | Value | Explanation |
| ----------------- | ----- | ----------- |
| Smart App Control | Off   |             |

#### Reputation-based protection

<!-- markdownlint-disable MD013 -->

| Key                                                                                                               | Value | Explanation |
| ----------------------------------------------------------------------------------------------------------------- | ----- | ----------- |
| Check apps and files                                                                                              | On    |             |
| SmartScreen for Microsoft Edge                                                                                    | On    |             |
| Phishing protection                                                                                               | On    |             |
| Warn me about malicious apps and sites                                                                            | On    |             |
| Warn me about password reuse                                                                                      | Off   |             |
| Warn me about unsafe password storage                                                                             | Off   |             |
| Automatically collect website or app content when additional analysis is needed to help identify security threats | On    |             |
| Potentially unwanted app blocking                                                                                 | On    |             |
| Block apps                                                                                                        | On    |             |
| Block downloads                                                                                                   | On    |             |
| SmartScreen for Microsoft Store apps                                                                              | On    |             |

<!-- markdownlint-enable MD013 -->

#### Exploit protection

<!-- markdownlint-disable MD013 -->

| Key                                             | Value             | Explanation |
| ----------------------------------------------- | ----------------- | ----------- |
| Control flow guard (CFG)                        | Use default (On)  |             |
| Data Execution Prevention (DEP)                 | Use default (On)  |             |
| Force randomization for images (Mandatory ASLR) | Use default (Off) |             |
| Randomize memory allocation (Bottom-up ASLR)    | Use default (On)  |             |
| High-entropy ASLR                               | Use default (On)  |             |
| Validate exception chains (SEHOP)               | Use default (On)  |             |
| Validate heap integrity                         | Use default (On)  |             |

<!-- markdownlint-enable MD013 -->

### Device security

#### Core isolation

<!-- markdownlint-disable MD013 -->

| Key                                            | Value | Explanation                           |
| ---------------------------------------------- | ----- | ------------------------------------- |
| Memory integrity                               | On    |                                       |
| Kernel-mode Hardware-enforced Stack Protection | Off   | Incompatible with BattlEye anti-cheat |
| Local Security Authority protection            | On    |                                       |
| Microsoft Vulnerable Driver Blocklist          | On    |                                       |

<!-- markdownlint-enable MD013 -->

## Xbox

### App

#### Startup

| Key                                           | Value | Explanation |
| --------------------------------------------- | ----- | ----------- |
| Launch Xbox when I start my computer          | Off   |             |
| On close, minimize the app to the system tray | Off   |             |

#### Offline permissions

| Key                         | Value | Explanation |
| --------------------------- | ----- | ----------- |
| Offline permissions enabled | On    |             |

#### Feedback

| Key                                              | Value | Explanation |
| ------------------------------------------------ | ----- | ----------- |
| Ask me for feedback about the app on this device | Off   |             |

#### Audio

##### Input device

<!-- markdownlint-disable MD013 -->

| Key          | Value                                                                   | Explanation |
| ------------ | ----------------------------------------------------------------------- | ----------- |
| Input device | SteelSeries Sonar - Microphone (SteelSeries Sonar Virtual Audio Device) |             |

<!-- markdownlint-enable MD013 -->

##### Output device

<!-- markdownlint-disable MD013 -->

| Key           | Value                                                             | Explanation |
| ------------- | ----------------------------------------------------------------- | ----------- |
| Output device | SteelSeries Sonar - Chat (SteelSeries Sonar Virtual Audio Device) |             |

<!-- markdownlint-enable MD013 -->

##### Voice volume

| Key | Value | Explanation |
| --- | ----- | ----------- |
| 🎧️  | 100   |             |

## Applications

### 1Password

```powershell
winget install AgileBits.1Password
winget install AgileBits.1Password.CLI
```

#### General

| Key                                     | Value | Explanation |
| --------------------------------------- | ----- | ----------- |
| Keep 1Password in the notification area | False |             |
| Open 1Password on startup               | False |             |

##### Keyboard Shortcuts

| Key               | Value  | Explanation |
| ----------------- | ------ | ----------- |
| Show Quick Access | (null) |             |
| Lock 1Password    | (null) |             |
| Autofill          | (null) |             |

#### Security

##### Unlock

| Key                        | Value | Explanation |
| -------------------------- | ----- | ----------- |
| Unlock using Windows Hello | True  |             |

##### Windows Hello

| Key                                                 | Value | Explanation |
| --------------------------------------------------- | ----- | ----------- |
| Use your device's Trusted Platform Module to unlock | True  |             |

##### Auto-lock

| Key                                | Value | Explanation |
| ---------------------------------- | ----- | ----------- |
| Lock when device locks or sleeps   | False |             |
| Lock after the device is idle for: | Never |             |

#### Privacy

##### Watchtower

| Key                            | Value | Explanation |
| ------------------------------ | ----- | ----------- |
| Check for vulnerable passwords | True  |             |

### AIDA64 Extreme

```powershell
winget install FinalWire.AIDA64.Extreme
```

### Amazon Games

```powershell
winget install Amazon.Games
Add-MpPreference -ExclusionPath "$env:LOCALAPPDATA\Amazon Games"
Add-MpPreference `
  -ExclusionProcess "$env:LOCALAPPDATA\Amazon Games\App\Amazon Games.exe"
Add-MpPreference `
  -ExclusionProcess ("$env:LOCALAPPDATA\Amazon Games\App\Amazon Games " + `
    "Services\Amazon Games Services.exe")
Add-MpPreference `
  -ExclusionProcess ("$env:LOCALAPPDATA\Amazon Games\App\Amazon Games " + `
    "UI\Amazon Games UI.exe")
```

#### Application

<!-- markdownlint-disable MD013 -->

| Key                                                             | Value | Explanation |
| --------------------------------------------------------------- | ----- | ----------- |
| Launch Amazon Games App on system startup                       | False |             |
| Automatically update Amazon Games App when the computer is idle | False |             |

<!-- markdownlint-enable MD013 -->

### AMD BlueTooth Drivers

Sourced from
[MPG X670E CARBON WIFI](https://www.msi.com/Motherboard/MPG-X670E-CARBON-WIFI/support#driver)

### AMD Chipset Drivers

Sourced from
[X670E Drivers and Downloads - Latest Version](https://www.amd.com/en/support/downloads/drivers.html/chipsets/am5/x670e.html)

### AMD Ryzen Master

Sourced from
[AMD Ryzen™ Master Utility for Overclocking Control](https://www.amd.com/en/products/software/ryzen-master.html)

#### Settings

##### Preferences

###### Display Settings

| Key                         | Value | Explanation |
| --------------------------- | ----- | ----------- |
| Discard Confirmation Popups | True  |             |

###### Ad Banner

| Key            | Value | Explanation |
| -------------- | ----- | ----------- |
| Show Ad Banner | False |             |

##### General

###### Data & Analytics

| Key                         | Value | Explanation |
| --------------------------- | ----- | ----------- |
| AMD User Experience Program | False |             |

### Apple Devices

```powershell
winget install 9NP83LWLPZ9K
```

#### Settings

| Key                                         | Value | Explanation |
| ------------------------------------------- | ----- | ----------- |
| Check for new software update automatically | Off   |             |
| Send usage data to Apple                    | Off   |             |

### Apple Music

```powershell
winget install 9PFHDD62MXS1
```

#### General

| Key                                  | Value | Explanation |
| ------------------------------------ | ----- | ----------- |
| Sync library                         | On    |             |
| Download Dolby Atmos                 | On    |             |
| Always check for available downloads | Off   |             |
| Use listening history                | On    |             |
| iTunes Store                         | False |             |
| Star ratings                         | False |             |
| Songs list tickboxes                 | False |             |

#### Playback

<!-- markdownlint-disable MD013 -->

| Key                                   | Value                               | Explanation |
| ------------------------------------- | ----------------------------------- | ----------- |
| Crossfade songs                       | Off                                 |             |
| Sound enhancer                        | Off                                 |             |
| Sound check                           | On                                  |             |
| Lossless audio                        | On                                  |             |
| Streaming                             | Lossless (ALAC up to 24-bit/48 kHz) |             |
| Download                              | Lossless (ALAC up to 24-bit/48 kHz) |             |
| Dolby Atmos                           | Always On                           |             |
| Video playback quality                | Best (Up to 4K)                     |             |
| Video download quality                | Up to HD                            |             |
| Show Automatic Subtitles When Muted   | On                                  |             |
| Show Automatic Subtitles on Skip Back | On                                  |             |
| Send playback data to Apple           | Off                                 |             |

<!-- markdownlint-enable MD013 -->

#### Restrictions

| Key                  | Value | Explanation |
| -------------------- | ----- | ----------- |
| Allow Explicit Music | True  |             |
| Allow Music Videos   | True  |             |

#### Files

| Key                                               | Value | Explanation |
| ------------------------------------------------- | ----- | ----------- |
| Keep Media folder organized                       | On    |             |
| Copy files to Media folder when adding to library | On    |             |

#### Advanced

| Key                                          | Value      | Explanation |
| -------------------------------------------- | ---------- | ----------- |
| Add songs to Library when adding to          | Favourites |             |
| Keep Mini Player on top of all other windows | Off        |             |
| Share Apple Music app analytics              | Off        |             |

### Atlas Toolbox

#### Interface Tweaks

##### Context Menu

| Key                                           | Value         | Explanation |
| --------------------------------------------- | ------------- | ----------- |
| Add or remove terminals from the context menu | Add terminals |             |

#### Advanced Configuration

| Key                      | Value | Explanation |
| ------------------------ | ----- | ----------- |
| Install Process Explorer | True  |             |

### BCUninstaller

```powershell
winget install Klocman.BulkCrapUninstaller
```

### BlueStacks

```powershell
winget install BlueStack.BlueStacks
```

### Cinebench

```powershell
winget install 9PGZKJC81Q7J
```

### CoreCycler

Sourced from [CoreCycler](https://github.com/sp00n/corecycler/releases)

### Crucial Storage Executive

Sourced from
[Crucial Storage Executive Tool](https://www.crucial.com/support/storage-executive)

### CrystalDiskInfo

```powershell
winget install CrystalDewWorld.CrystalDiskInfo
```

#### Theme

| Key  | Value | Explanation |
| ---- | ----- | ----------- |
| Dark | True  |             |

### CrystalDiskMark

```powershell
winget install CrystalDewWorld.CrystalDiskMark
```

#### Settings

| Key      | Value | Explanation |
| -------- | ----- | ----------- |
| NVMe SSD | True  |             |

### Discord

```powershell
winget install Discord.Discord

Add-MpPreference -ExclusionPath "$env:LOCALAPPDATA\Discord"

# Discord installs to versioned subfolders like app-1.0.9001; wildcard handles
# version changes
Add-MpPreference -ExclusionProcess "$env:LOCALAPPDATA\Discord\app-*\Discord.exe"
Add-MpPreference -ExclusionProcess ("$env:LOCALAPPDATA\Discord\app-*" + `
  "\modules\discord_utils-1\discord_utils\DiscordSystemHelper.exe")
```

#### Notifications

##### Overview

| Key                          | Value | Explanation |
| ---------------------------- | ----- | ----------- |
| Enable Desktop Notifications | False |             |

##### Sounds

| Key         | Value | Explanation |
| ----------- | ----- | ----------- |
| New Message | False |             |

#### Clips

| Key             | Value | Explanation |
| --------------- | ----- | ----------- |
| Enable Clipping | False |             |

#### Voice & Video

##### Voice

| Key                                    | Value           | Explanation |
| -------------------------------------- | --------------- | ----------- |
| Microphone                             | Windows Default |             |
| Speaker                                | Windows Default |             |
| Input Profile                          | Custom          |             |
| Automatically Adjust Input Sensitivity | False           |             |
| Noise Suppression                      | None            |             |
| Echo Cancellation                      | False           |             |
| Push to Talk                           | False           |             |
| Automatic Gain Control                 | False           |             |
| Bypass System Audio Input Processing   | False           |             |
| No Audio Detected Warning              | False           |             |
| Quality Of Service                     | True            |             |

#### Appearance

##### Theme

| Key                          | Value            | Explanation |
| ---------------------------- | ---------------- | ----------- |
| Color Theme                  | Midnight Blurple |             |
| Sync theme across my devices | False            |             |

#### Keybinds

| Key          | Value     | Explanation |
| ------------ | --------- | ----------- |
| Save Clip    | False     |             |
| Push to Mute | RIGHT ALT |             |

#### Windows Settings

<!-- markdownlint-disable MD013 -->

| Key                                                     | Value | Explanation |
| ------------------------------------------------------- | ----- | ----------- |
| Automatically open Discord when your computer starts up | True  |             |
| Start Discord minimized                                 | True  |             |
| Minimize Discord to System Tray                         | True  |             |

<!-- markdownlint-enable MD013 -->

#### Game Overlay

| Key                   | Value | Explanation |
| --------------------- | ----- | ----------- |
| Enable Overlay        | False |             |
| Enable Legacy Overlay | False |             |

### DiskSpd

Sourced from [DiskSpd](https://github.com/microsoft/diskspd/releases)

### DroidCam Client

```powershell
winget install dev47apps.DroidCamOBSClient
```

### DroidCam OBS Plugin

```powershell
winget install dev47apps.DroidCamOBSPlugin
```

### EA

```powershell
winget install ElectronicArts.EADesktop

Add-MpPreference -ExclusionPath "C:\Program Files\Electronic Arts\EA Desktop"
Add-MpPreference -ExclusionPath "C:\Program Files\EA Games"
Add-MpPreference -ExclusionProcess ("C:\Program Files\Electronic Arts\EA " + `
  "Desktop\EA Desktop\EABackgroundService.exe")
Add-MpPreference -ExclusionProcess ("C:\Program Files\Electronic Arts\EA " + `
  "Desktop\EA Desktop\EACefSubProcess.exe")
Add-MpPreference -ExclusionProcess ("C:\Program Files\Electronic Arts\EA " + `
  "Desktop\EA Desktop\EADesktop.exe")
Add-MpPreference -ExclusionProcess ("C:\Program Files\Electronic Arts\EA " + `
  "Desktop\EA Desktop\EALocalHostSvc.exe")
```

#### My account

##### Privacy

| Key           | Value | Explanation |
| ------------- | ----- | ----------- |
| Usage sharing | False |             |

#### Application

##### Application settings

| Key                           | Value | Explanation |
| ----------------------------- | ----- | ----------- |
| Install updates automatically | False |             |
| Run on startup                | False |             |

##### In-game overlay

| Key                    | Value | Explanation |
| ---------------------- | ----- | ----------- |
| Enable in-game overlay | False |             |

#### Games

<!-- markdownlint-disable MD013 -->

| Key                                                           | Value | Explanation |
| ------------------------------------------------------------- | ----- | ----------- |
| Automatically update games when a new version is available    | False |             |
| Show toast notifications when a game installation is finished | False |             |

<!-- markdownlint-enable MD013 -->

### Epic Games Launcher

```powershell
winget install EpicGames.EpicGamesLauncher

Add-MpPreference -ExclusionPath "C:\Program Files\Epic Games"
Add-MpPreference -ExclusionPath "C:\Program Files (x86)\Epic Games"
Add-MpPreference -ExclusionProcess ("C:\Program Files\Epic Games\Launcher" + `
  "\Portal\Binaries\Win64\EpicGamesLauncher.exe")
Add-MpPreference -ExclusionProcess ("C:\Program Files\Epic Games\Launcher" + `
  "\Portal\Binaries\Win64\EpicWebHelper.exe")
Add-MpPreference -ExclusionProcess ("C:\Program Files\Epic Games\Launcher" + `
  "\Portal\Extras\Overlay\EOSOverlayRenderer-Win64-Shipping.exe")
Add-MpPreference -ExclusionProcess ("C:\Program Files (x86)\Epic Games" + `
  "\Epic Online Services\EpicOnlineServicesUserHelper.exe")
```

#### Preferences

| Key                         | Value | Explanation |
| --------------------------- | ----- | ----------- |
| Minimize To System Tray     | False |             |
| Run When My Computer Starts | False |             |

#### Desktop notifications

| Key                                       | Value | Explanation |
| ----------------------------------------- | ----- | ----------- |
| Show Free Game Notifications              | False |             |
| Show News and Special Offer Notifications | False |             |
| Show Chat Notifications                   | False |             |
| Show Game Invitation Notifications        | False |             |

### FanControl

```powershell
winget install Rem0o.FanControl

Add-MpPreference -ExclusionPath "C:\Program Files (x86)\FanControl"
Add-MpPreference -ExclusionProcess "C:\Program Files (x86)\FanControl\FanControl.exe"
```

- Add
  [FanControl.LiquidCtl](https://github.com/antoine-bouteiller/FanControl.LiquidCtl)
- Add [FanControl.Weather](https://github.com/pgodschalk/FanControl.Weather)

#### Controls

##### Pump

| Key   | Value    | Explanation |
| ----- | -------- | ----------- |
| Curve | P - Pump |             |

##### GPU front & rear

| Key   | Value    | Explanation |
| ----- | -------- | ----------- |
| Curve | GPU fans |             |

##### GPU center

| Key   | Value    | Explanation |
| ----- | -------- | ----------- |
| Curve | GPU fans |             |

##### Bottom intake front & rear, top exhaust center

<!-- markdownlint-disable MD013 -->

| Key   | Value                                                   | Explanation |
| ----- | ------------------------------------------------------- | ----------- |
| Curve | Wire 1 - Bottom intake front & rear, top exhaust center |             |

<!-- markdownlint-enable MD013 -->

##### Bottom intake center, top exhaust front & rear

<!-- markdownlint-disable MD013 -->

| Key   | Value                                                   | Explanation |
| ----- | ------------------------------------------------------- | ----------- |
| Curve | Wire 2 - Bottom intake center, top exhaust front & rear |             |

<!-- markdownlint-enable MD013 -->

##### Front intake center pull, front intake top & bottom push

<!-- markdownlint-disable MD013 -->

| Key   | Value                                                             | Explanation |
| ----- | ----------------------------------------------------------------- | ----------- |
| Curve | Wire 3 - Front intake center pull, front intake top & bottom push |             |

<!-- markdownlint-enable MD013 -->

##### Front intake top & bottom pull, front intake center push

<!-- markdownlint-disable MD013 -->

| Key   | Value                                                             | Explanation |
| ----- | ----------------------------------------------------------------- | ----------- |
| Curve | Wire 4 - Front intake top & bottom pull, front intake center push |             |

<!-- markdownlint-enable MD013 -->

##### Rear exhaust

| Key   | Value                 | Explanation |
| ----- | --------------------- | ----------- |
| Curve | Wire 5 - Rear exhaust |             |

#### Curves

##### A - Liquid ΔT

| Key                | Value                          | Explanation |
| ------------------ | ------------------------------ | ----------- |
| Temperature source | Liquid over ambient - Mix      |             |
| <= 4 °C            | 30%                            |             |
| 7 °C               | 42%                            |             |
| 10 °C              | 60%                            |             |
| 13 °C              | 80%                            |             |
| >= 16 °C           | 100%                           |             |
| Hysteresis         | ↑ 2 °C · 3 sec ↓ 2 °C · 10 sec |             |

##### P - Pump

<!-- markdownlint-disable MD013 -->

| Key                | Value                                                  | Explanation |
| ------------------ | ------------------------------------------------------ | ----------- |
| Temperature source | NZXT Kraken 2023 Elite: Liquid temperature - liquidctl |             |
| <= 33 °C           | 70%                                                    |             |
| 37 °C              | 80%                                                    |             |
| 40 °C              | 90%                                                    |             |
| >= 42 °C           | 100%                                                   |             |
| Hysteresis         | ↑↓ 2 °C · 1 sec                                        |             |

<!-- markdownlint-enable MD013 -->

##### G - GPU airflow

| Key                | Value                                  | Explanation |
| ------------------ | -------------------------------------- | ----------- |
| Temperature source | GPU Hot Spot - NVIDIA GeForce RTX 4090 |             |
| <= 55 °C           | 30%                                    |             |
| 68 °C              | 45%                                    |             |
| 78 °C              | 65%                                    |             |
| 84 °C              | 85%                                    |             |
| >= 90 °C           | 100%                                   |             |
| Hysteresis         | ↑ 3 °C · 2 sec ↓ 3 °C · 6 sec          |             |

##### Gpu - 4090 fans

| Key                | Value                                  | Explanation |
| ------------------ | -------------------------------------- | ----------- |
| Temperature source | GPU Hot Spot - NVIDIA GeForce RTX 4090 |             |
| <= 68 °C           | 0%                                     |             |
| 70 °C              | 35%                                    |             |
| 76 °C              | 55%                                    |             |
| 82 °C              | 75%                                    |             |
| 88 °C              | 90%                                    |             |
| >= 92 °C           | 100%                                   |             |
| Hysteresis         | ↑ 4 °C · 2 sec ↓ 4 °C · 6 sec          |             |

##### Gmem - VRAM safety

<!-- markdownlint-disable MD013 -->

| Key                | Value                                         | Explanation |
| ------------------ | --------------------------------------------- | ----------- |
| Temperature source | GPU Memory Junction - NVIDIA GeForce RTX 4090 |             |
| <= 72 °C           | 0%                                            |             |
| 80 °C              | 40%                                           |             |
| 86 °C              | 65%                                           |             |
| 90 °C              | 85%                                           |             |
| >= 94 °C           | 100%                                          |             |
| Hysteresis         | ↑ 2 °C · 2 sec ↓ 2 °C · 6 sec                 |             |

<!-- markdownlint-enable MD013 -->

##### D - DRAM floor

| Key                | Value                          | Explanation |
| ------------------ | ------------------------------ | ----------- |
| Temperature source | DRAM - Mix                     |             |
| <= 44 °C           | 0%                             |             |
| 48 °C              | 35%                            |             |
| 51 °C              | 60%                            |             |
| 54 °C              | 90%                            |             |
| >= 56 °C           | 100%                           |             |
| Hysteresis         | ↑ 2 °C · 3 sec ↓ 2 °C · 10 sec |             |

##### S - SSD floor

| Key                | Value                         | Explanation |
| ------------------ | ----------------------------- | ----------- |
| Temperature source | Temperature - CT2000T700SSD3  |             |
| <= 58 °C           | 0%                            |             |
| 66 °C              | 40%                           |             |
| 72 °C              | 70%                           |             |
| >= 78 °C           | 100%                          |             |
| Hysteresis         | ↑ 3 °C · 3 sec ↓ 3 °C · 8 sec |             |

##### V - VRM safety

<!-- markdownlint-disable MD013 -->

| Key                | Value                                         | Explanation |
| ------------------ | --------------------------------------------- | ----------- |
| Temperature source | VRM MOS - MSI MPG X670E CARBON WIFI (MS-7D70) |             |
| <= 75 °C           | 0%                                            |             |
| 85 °C              | 60%                                           |             |
| >= 95 °C           | 100%                                          |             |
| Hysteresis         | ↑ 3 °C · 3 sec ↓ 3 °C · 10 sec                |             |

<!-- markdownlint-enable MD013 -->

##### Wire 1 - Bottom intake front & rear, top exhaust center

<!-- markdownlint-disable MD013 -->

| Key        | Value                                                              | Explanation |
| ---------- | ------------------------------------------------------------------ | ----------- |
| Function   | Max                                                                |             |
| Fan curves | G - GPU airflow, Gmem - VRAM safety, D - DRAM floor, S - SSD floor |             |

<!-- markdownlint-enable MD013 -->

##### Wire 2 - Bottom intake center & top exhaust front & rear

<!-- markdownlint-disable MD013 -->

| Key        | Value                                                              | Explanation |
| ---------- | ------------------------------------------------------------------ | ----------- |
| Function   | Max                                                                |             |
| Fan curves | G - GPU airflow, Gmem - VRAM safety, D - DRAM floor, A - Liquid ΔT |             |

<!-- markdownlint-enable MD013 -->

##### Wire 3 - Front intake center pull, front intake top & bottom push

<!-- markdownlint-disable MD013 -->

| Key        | Value                                                                             | Explanation |
| ---------- | --------------------------------------------------------------------------------- | ----------- |
| Function   | Max                                                                               |             |
| Fan curves | A - Liquid ΔT, G - GPU Airflow, Gmem - VRAM safety, D - DRAM floor, S - SSD floor |             |

<!-- markdownlint-enable MD013 -->

##### Wire 4 - Front intake top & bottom pull, front intake center push

<!-- markdownlint-disable MD013 -->

| Key        | Value                                                                             | Explanation |
| ---------- | --------------------------------------------------------------------------------- | ----------- |
| Function   | Max                                                                               |             |
| Fan curves | A - Liquid ΔT, G - GPU Airflow, Gmem - VRAM safety, D - DRAM floor, S - SSD floor |             |

<!-- markdownlint-enable MD013 -->

##### Wire 5 - Rear exhaust

| Key        | Value                                          | Explanation |
| ---------- | ---------------------------------------------- | ----------- |
| Function   | Max                                            |             |
| Fan curves | A - Liquid ΔT, G - GPU Airflow, V - VRM safety |             |

##### GPU fans

| Key        | Value                               | Explanation |
| ---------- | ----------------------------------- | ----------- |
| Function   | Max                                 |             |
| Fan curves | Gpu - 4090 fans, Gmem - VRAM safety |             |

#### Custom Sensors

##### Room temperature floor constant

| Key       | Value          | Explanation |
| --------- | -------------- | ----------- |
| File name | floor22.sensor |             |

##### Ambient temperature

<!-- markdownlint-disable MD013 -->

| Key      | Value                                                              | Explanation |
| -------- | ------------------------------------------------------------------ | ----------- |
| Function | Max                                                                |             |
| Sensors  | Outside (Leiden) - Weather, Room temperature floor constant - File |             |

<!-- markdownlint-enable MD013 -->

##### Liquid over ambient

<!-- markdownlint-disable MD013 -->

| Key      | Value                                                                             | Explanation |
| -------- | --------------------------------------------------------------------------------- | ----------- |
| Function | Subtract                                                                          |             |
| Sensors  | NZXT Kraken 2023 Elite: Liquid temperature - liquidctl, Ambient temperature - Mix |             |

<!-- markdownlint-enable MD013 -->

##### DRAM

<!-- markdownlint-disable MD013 -->

| Key      | Value                                                                               | Explanation |
| -------- | ----------------------------------------------------------------------------------- | ----------- |
| Function | Max                                                                                 |             |
| Sensors  | DIMM #1 - G Skill Intl - F5-6000J3040G32G, DIMM #3 - G Skill Intl - F56000J3040G32G |             |

<!-- markdownlint-enable MD013 -->

#### Settings

##### General

| Key                          | Value        | Explanation |
| ---------------------------- | ------------ | ----------- |
| Start minimized              | True         |             |
| Start app at user log on     | 30 sec, True |             |
| Start service on boot        | False        |             |
| Notify for update at startup | False        |             |

##### Sensors

###### LibreHardwareMonitor

| Key                                | Value        | Explanation |
| ---------------------------------- | ------------ | ----------- |
| Motherboard                        | True         |             |
| CPU                                | True         |             |
| GPU                                | True         |             |
| Storage                            | True, 60 sec |             |
| Controller (various third parties) | False        |             |
| Memory                             | True         |             |
| PSU (only Corsair)                 | False        |             |
| Embedded AC (only ASUS)            | False        |             |
| Power Monitor                      | False        |             |

###### NVAPI (NVIDIA GPUs, at least GTX or RTX-based)

| Key                         | Value | Explanation |
| --------------------------- | ----- | ----------- |
| Enabled (will override LHM) | False |             |

###### NVIDIA 0% hardware curve override

| Key     | Value | Explanation |
| ------- | ----- | ----------- |
| Enabled | True  |             |

###### AMD ADLX (AMD GPUs, at least RDNA-based)

| Key                         | Value | Explanation |
| --------------------------- | ----- | ----------- |
| Enabled (will override LHM) | False |             |

###### Plugins

| Key       | Value | Explanation |
| --------- | ----- | ----------- |
| liquidctl | True  |             |
| Weather   | True  |             |

### Flawless Widescreen

```powershell
winget install FlawlessWidescreen.FlawlessWidescreen
```

#### Display Detection

| Key                  | Value | Explanation |
| -------------------- | ----- | ----------- |
| Enable AMD Detection | False |             |

### Flydigi Space Station 4.0

```powershell
winget install Flydigi.FlydigiSpaceStation
```

#### Common

| Key                      | Value        | Explanation |
| ------------------------ | ------------ | ----------- |
| Light mode               | Dynamic glow |             |
| Brightness               | 50           |             |
| Cycle time               | 16           |             |
| Grip vibration           | True         |             |
| Grip vibration intensity | 50%          |             |

#### Joystick

##### Left joystick

| Key                   | Value     | Explanation |
| --------------------- | --------- | ----------- |
| Circularity algorithm | Rectangle |             |
| Sensitivity curve     | Default   |             |

###### Joystick active range

| Key    | Value | Explanation |
| ------ | ----- | ----------- |
| Center | 0     |             |
| Edge   | 0     |             |

##### Right joystick

| Key                   | Value   | Explanation |
| --------------------- | ------- | ----------- |
| Circularity algorithm | Circle  |             |
| Sensitivity curve     | Default |             |

###### Joystick active range

| Key    | Value | Explanation |
| ------ | ----- | ----------- |
| Center | 0     |             |
| Edge   | 0     |             |

#### Gyro

| Key        | Value | Explanation |
| ---------- | ----- | ----------- |
| Mapping to | Close |             |

#### Trigger

##### Left trigger

| Key                       | Value | Explanation |
| ------------------------- | ----- | ----------- |
| Trigger Vibration Switch  | True  |             |
| Stroke Setting            | 0-255 |             |
| Vibration Intensity       | 50    |             |
| Trigger Amplitude         | 12-32 |             |
| Vibration Shielding Value | 5     |             |

##### Right trigger

| Key                       | Value | Explanation |
| ------------------------- | ----- | ----------- |
| Trigger Vibration Switch  | True  |             |
| Stroke Setting            | 0-255 |             |
| Vibration Intensity       | 50    |             |
| Trigger Amplitude         | 12-32 |             |
| Vibration Shielding Value | 5     |             |

#### Space Station Settings

| Key                     | Value               | Explanation |
| ----------------------- | ------------------- | ----------- |
| When Closing the Window | Close space station |             |
| GPU Acceleration        | True                |             |

#### Controller Settings

##### Joystick Global Settings

| Key                   | Value   | Explanation |
| --------------------- | ------- | ----------- |
| Fast Swap Config      | False   |             |
| Joystick debounce     | False   |             |
| Automatic calibration | False   |             |
| Rebounce algorithm    | False   |             |
| Accuracy              | 12 bit  |             |
| Joystick Polling Rate | 1000 Hz |             |
| Center sensitivity    | Fast    |             |

### GOG GALAXY

```powershell
winget install GOG.Galaxy

Add-MpPreference -ExclusionPath "C:\Program Files (x86)\GOG Galaxy"
Add-MpPreference -ExclusionPath "C:\GOG Games"
Add-MpPreference -ExclusionProcess ("C:\Program Files (x86)\GOG Galaxy" + `
  "\GalaxyClient.exe")
Add-MpPreference -ExclusionProcess ("C:\Program Files (x86)\GOG Galaxy" + `
  "\GalaxyClient Helper.exe")
Add-MpPreference -ExclusionProcess ("C:\Program Files (x86)\GOG Galaxy" + `
  "\GalaxyClientService.exe")
Add-MpPreference -ExclusionProcess ("C:\Program Files (x86)\GOG Galaxy" + `
  "\GOG Galaxy Notifications Renderer.exe")
Add-MpPreference -ExclusionProcess ("C:\ProgramData\GOG.com\Galaxy" + `
  "\redists\GalaxyCommunication.exe")
Add-MpPreference -ExclusionProcess ("C:\Program Files (x86)\GOG Galaxy" + `
  "\python\python.exe")
```

#### Integrations

| Key              | Value     | Explanation |
| ---------------- | --------- | ----------- |
| GOG.com          | Connected |             |
| Epic Games Store | Connected |             |
| Xbox Live        | Connected |             |

#### Features

##### Epic Games Store

| Key            | Value | Explanation |
| -------------- | ----- | ----------- |
| Closing client | True  |             |

#### General

##### General

| Key           | Value       | Explanation |
| ------------- | ----------- | ----------- |
| Bug reports   | False       |             |
| Auto start    | False       |             |
| Auto login    | True        |             |
| Starting page | Owned games |             |

#### Interface

##### Main window behaviour

| Key                     | Value           | Explanation |
| ----------------------- | --------------- | ----------- |
| When closing the window | Exit GOG GALAXY |             |

#### Notifications

| Key                         | Value        | Explanation |
| --------------------------- | ------------ | ----------- |
| Message received            | Desktop only |             |
| Friend invite               | Desktop only |             |
| Game invite                 | Desktop only |             |
| Friend comes online         | –            |             |
| Friend starts a game        | –            |             |
| Installing /updating status | –            |             |
| Wishlist                    | –            |             |
| Announcements               | –            |             |
| GOG Dreamlist               | –            |             |

#### Game features

##### Game data features

| Key               | Value | Explanation |
| ----------------- | ----- | ----------- |
| Auto-update games | False |             |

##### In-game features

| Key     | Value | Explanation |
| ------- | ----- | ----------- |
| Overlay | False |             |

### HWiNFO 64

```powershell
winget install REALiX.HWiNFO
```

### HYDRA

Sourced from [Yuri Bubliy](https://www.patreon.com/c/1usmus/posts?vanity=1usmus)

### JetBrains Mono Nerd Font

Sourced from [Nerd Fonts](https://www.nerdfonts.com)

### Legacy Games Launcher

```powershell
winget install LegacyGames.LegacyGamesLauncher

Add-MpPreference -ExclusionPath "C:\Program Files (x86)\Legacy Games"
Add-MpPreference -ExclusionProcess ("C:\Program Files (x86)\Legacy Games" + `
  "\Legacy Games Launcher.exe")
```

| Key                             | Value | Explanation |
| ------------------------------- | ----- | ----------- |
| Notifications                   | False |             |
| Automatically check for updates | False |             |

### LiveSplit

```powershell
winget install LiveSplit.LiveSplit
```

#### Hotkeys

| Key           | Value                | Explanation |
| ------------- | -------------------- | ----------- |
| Start / Split | Oem6, Shift, Control |             |

### Logitech G HUB

```powershell
winget install Logitech.GHUB

Add-MpPreference -ExclusionPath "C:\Program Files\LGHUB"
Add-MpPreference -ExclusionProcess "C:\Program Files\LGHUB\lghub.exe"
Add-MpPreference -ExclusionProcess "C:\Program Files\LGHUB\lghub_agent.exe"
Add-MpPreference -ExclusionProcess "C:\Program Files\LGHUB\lghub_updater.exe"
```

#### PRO X2 SUPERSTRIKE

##### Sensitivity

| Key                     | Value         | Explanation |
| ----------------------- | ------------- | ----------- |
| Advanced                | True          |             |
| DPI                     | 1600, default |             |
| Lift off distance       | High          |             |
| Wireless Report Rate    | 8000 Hz       |             |
| Wired Report Rate       | 1000 Hz       |             |
| Hero Sensor Calibration | None          |             |

##### Scroll Wheel

| Key              | Value | Explanation |
| ---------------- | ----- | ----------- |
| Enable BHOP Mode | False |             |

##### HITS Configuration

| Key             | Value | Explanation |
| --------------- | ----- | ----------- |
| Actuation Point | 2     |             |
| Rapid Trigger   | 1     |             |
| Click Haptics   | 1     |             |

##### Device Settings

| Key                 | Value | Explanation |
| ------------------- | ----- | ----------- |
| Gaming Surface Mode | On    |             |
| Onboard Mode        | True  |             |

#### Settings

##### General Settings

| Key                   | Value | Explanation |
| --------------------- | ----- | ----------- |
| Launch app on login   | False |             |
| Game lighting control | False |             |

###### Notifications

| Key             | Value | Explanation |
| --------------- | ----- | ----------- |
| Recommendations | False |             |

##### Updates

| Key                      | Value | Explanation |
| ------------------------ | ----- | ----------- |
| Enable Automatic Updates | False |             |

##### Beta Features

| Key   | Value | Explanation |
| ----- | ----- | ----------- |
| Games | False |             |

##### Analytics

<!-- markdownlint-disable MD013 -->

| Key                                                        | Value | Explanation |
| ---------------------------------------------------------- | ----- | ----------- |
| Share my usage data                                        | False |             |
| Send error logs automatically when G HUB encounters issues | False |             |

<!-- markdownlint-enable MD013 -->

### ludusavi

```powershell
winget install mtkennerly.ludusavi
```

### MSI Afterburner

```powershell
winget install Guru3D.Afterburner
```

#### General

##### Master graphics processor selection

| Key                                                  | Value | Explanation |
| ---------------------------------------------------- | ----- | ----------- |
| Synchronize settings for similar graphics processors | False |             |

##### Update checking properties

| Key                                 | Value | Explanation |
| ----------------------------------- | ----- | ----------- |
| Check for available product updates | Never |             |

### NanaZip

#### Editor

<!-- markdownlint-disable MD013 -->

| Key     | Value                                                                        | Explanation |
| ------- | ---------------------------------------------------------------------------- | ----------- |
| View:   | C:\Users\Patrick Godschalk\AppData\Local\Programs\Microsoft VS Code\Code.exe |             |
| Editor: | C:\Users\Patrick Godschalk\AppData\Local\Programs\Microsoft VS Code\Code.exe |             |

<!-- markdownlint-enable MD013 -->

#### Settings

| Key                    | Value | Explanation |
| ---------------------- | ----- | ----------- |
| Use large memory pages | True  |             |

### NVCleanstall

```powershell
winget install TechPowerUp.NVCleanstall

# Newer NV driver cache
Add-MpPreference -ExclusionPath "$env:LOCALAPPDATA\NVIDIA Corporation\NV_Cache"

# Instant Replay videos
Add-MpPreference -ExclusionPath "$env:USERPROFILE\Videos"
```

#### Select Components To Install

- [x] Display Driver (required)
- [x] Legacy Control Panel
- [ ] HD Audio via HDMI
- [x] Microsoft Visual C 2017 Runtimes
- [x] PhysX
- [ ] USB-C Driver
- [x] FrameView SDK
- [x] Virtual Audio
- [x] Telemetry
- [x] NV Platform Controllers
- [x] NVIDIA DLISR

##### NV App Components

- [x] NVIDIA App
- [x] NV Container
- [x] ShadowPlay
- [x] NV Backend
- [x] NVIDIA App MessageBus

#### Installation Tweaks

- [x] Disable Installer Telemetry & Advertising
- [x] Show Expert Tweaks
  - [x] Enable Message Signaled Interrupts
    - Interrupt Policy: All Close Processors
    - Interrupt Priority: High
  - [x] Disable HDCP

### NVIDIA App

#### Graphics

##### Program settings

Below are the specific overrides for _competitive_ play as the global settings
are oriented towards maximum visual quality. Some other specific non-competitive
games might also be overridden here, for example, forcing a specific
anti-aliasing for older games with buggy implementations.

| Key     | Value | Explanation |
| ------- | ----- | ----------- |
| RTX HDR | Off   |             |

<!-- markdownlint-disable MD013 -->

##### Global Settings

| Key                                            | Value                        | Explanation                                                                                                                                                                                                                                                                                                                                                                                            |
| ---------------------------------------------- | ---------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| DLSS Override - Model Presets                  | Recommended                  |                                                                                                                                                                                                                                                                                                                                                                                                        |
| DLSS Override - Super Resolution Mode          | Use 3D app setting (Default) |                                                                                                                                                                                                                                                                                                                                                                                                        |
| Smooth Motion                                  | Off (Default)                | Driver-level frame interpolation for games that don't natively support DLSS Frame Generation. Adds inserted frames using ML inference on the driver side. However, unlike frame gen, it's a terrible experience.                                                                                                                                                                                       |
| Low Latency Mode                               | Ultra                        | For games without native NVIDIA Reflex. Reduces the render queue to lower input-to-display latency. Reflex (when supported by the game) is better than Low Latency Mode and overrides it automatically. For games without Reflex, Ultra reduces render queue to absolute minimum — measurable latency reduction with no quality cost.                                                                  |
| CUDA - GPUs                                    | NVIDIA GeForce RTX 4090      | With one GPU, this setting effectively has no choice to make.                                                                                                                                                                                                                                                                                                                                          |
| Image Sharpening                               | Off (Default)                | Most modern games apply their own sharpening (FXAA, TAA-Sharpen, FidelityFX CAS, DLSS internal). Stacking driver sharpening on top creates over-sharpened, ringy textures.                                                                                                                                                                                                                             |
| Max Frame Rate                                 | 224 FPS                      | For G-Sync + V-Sync workflow (NVIDIA's canonical low-tearing config), you want frames to stay within the VRR range. Hitting your monitor's max refresh rate engages V-Sync's "wait for next refresh" behavior, adding latency.                                                                                                                                                                         |
| Monitor Technology                             | G-Sync Compatible (Default)  | This tells the driver which VRR mode to expect.                                                                                                                                                                                                                                                                                                                                                        |
| OpenGL GDI Compatibility                       | Auto (Default)               | Auto handles this correctly for both legacy and modern OpenGL apps.                                                                                                                                                                                                                                                                                                                                    |
| Power Management Mode                          | Prefer maximum performance   | GPU P-state transitions during gameplay cause frame-time variance — the GPU can dip to a lower clock briefly, causing a stutter. "Prefer Maximum Performance" keeps the GPU at high clocks while the app is active, eliminating those transitions.                                                                                                                                                     |
| RTX Dynamic Vibrance                           | Off (Default)                | RTX Dynamic Vibrance can over-saturate and disrupt the artist's intended color palette.                                                                                                                                                                                                                                                                                                                |
| RTX HDR                                        | On                           |                                                                                                                                                                                                                                                                                                                                                                                                        |
| Shader Cache - Cache Size                      | Unlimited                    | Larger shader cache = fewer in-game shader compile stutters across launches. The cost is only disk space.                                                                                                                                                                                                                                                                                              |
| Automatic Shader Compilation (Beta)            | Off (Default)                |                                                                                                                                                                                                                                                                                                                                                                                                        |
| Vertical Sync                                  | On                           | NVIDIA's recommended low-tearing config is G-Sync On + V-Sync On (driver, not in-game) + frame cap below max refresh. The frame cap keeps you within G-Sync's range, V-Sync only kicks in if you somehow exceed the cap, eliminating residual tearing. V-Sync setting should be at the driver level, not in-game. In-game V-Sync sometimes uses double/triple buffering that adds significant latency. |
| Virtual Reality - Variable Rate Super Sampling | Off (Default)                | Irrelevant for non-VR workloads. Leaves CPU/GPU cycles on the table if accidentally enabled.                                                                                                                                                                                                                                                                                                           |
| Vulkan/OpenGL Present Method                   | Auto (Default)               | Layered-on-DXGI (the modern path) generally has better G-Sync integration and lower latency than legacy direct presentation. Auto picks the right mode per-app.                                                                                                                                                                                                                                        |
| Anisotropic Filtering                          | 16x                          | Why: 16x AF has been "free" since the GTX 600 series. There's no rational reason to set it lower. Modern GPUs eat 16x AF without noticeable cost. Always 16x.                                                                                                                                                                                                                                          |
| Antialiasing - FXAA                            | Off (Default)                | FXAA was 2011-era anti-aliasing. It blurs everything indiscriminately (including text and UI elements). Driver-level FXAA stacks on top of in-game AA, creating over-blurred output. Always off.                                                                                                                                                                                                       |
| Antialiasing - Transparency                    | Off (Default)                | Setting Supersample is the high-quality choice for the rare titles that still use MSAA (older games, some sim titles). On a 4090, the perf cost is negligible. For 99% of modern games this setting does nothing. It's off, because the few games where this isn't a noop, it creates weird lighting effects.                                                                                          |
| Background Application Max Frame Rate          | Off (Default)                |                                                                                                                                                                                                                                                                                                                                                                                                        |
| Multi-Frame Sampled AA (MFAA)                  | Off (Default)                | MFAA only worked with MSAA-enabled titles. With MSAA effectively dead in modern games, MFAA has essentially no titles where it does anything.                                                                                                                                                                                                                                                          |
| PhysX                                          | NVIDIA GeForce RTX 4090      | PhysX is hardware-accelerated on NVIDIA GPUs and runs in parallel with rendering. CPU PhysX is significantly slower and ties up CPU cycles. The 4090 has more PhysX headroom than any PhysX-using game can saturate.                                                                                                                                                                                   |
| Texture Filtering - Negative LOD Bias          | Clamp                        | "Allow" lets games request sharper textures, which can introduce moiré/shimmer in motion. "Clamp" prevents this — slightly less crisp but stable. For visual quality, Clamp wins (no shimmer).                                                                                                                                                                                                         |
| Texture Filtering - Quality                    | High quality                 | High Quality enforces strict filtering (no shortcuts). Performance/High Performance enable optimizations that reduce filtering quality for older hardware. On a 4090, the perf cost of High Quality vs Quality is unmeasurable.                                                                                                                                                                        |

<!-- markdownlint-enable MD013 -->

#### System

##### Displays

###### Global Settings

| Key             | Value                        | Explanation |
| --------------- | ---------------------------- | ----------- |
| G-SYNC Settings | On, Full screen and windowed |             |

###### Display Settings

| Key               | Value                | Explanation |
| ----------------- | -------------------- | ----------- |
| G-SYNC Compatible | True                 |             |
| Resolution        | 5120 x 1440 (native) |             |
| Refresh Rate      | 240 Hz               |             |

###### Scaling

<!-- markdownlint-disable MD013 -->

| Key                                                 | Value        | Explanation |
| --------------------------------------------------- | ------------ | ----------- |
| Mode                                                | Aspect Ratio |             |
| Scaling Device                                      | GPU          |             |
| Override the scaling mode set by games and programs | True         |             |

<!-- markdownlint-enable MD013 -->

##### Video

###### Global Settings

<!-- markdownlint-disable MD013 -->

| Key              | Value                                                                         | Explanation |
| ---------------- | ----------------------------------------------------------------------------- | ----------- |
| Super Resolution | On                                                                            |             |
| Quality          | Manual, High                                                                  |             |
| HDR              | On, 630 nits peak brightness, 50 nits middle grey, 0% contrast, 0% saturation |             |

<!-- markdownlint-enable MD013 -->

#### Settings

##### Features

###### Overlay

| Key                         | Value | Explanation |
| --------------------------- | ----- | ----------- |
| NVIDIA overlay              | True  |             |
| Game filters and Photo mode | True  |             |

###### Drivers

<!-- markdownlint-disable MD013 -->

| Key                                                              | Value | Explanation |
| ---------------------------------------------------------------- | ----- | ----------- |
| Automatically download drivers and let me choose when to install | False |             |

<!-- markdownlint-enable MD013 -->

###### Games and Apps

<!-- markdownlint-disable MD013 -->

| Key                                               | Value                                                                  | Explanation |
| ------------------------------------------------- | ---------------------------------------------------------------------- | ----------- |
| Scan locations                                    | C:\Program Files, C:\Program Files (x86), C:\XboxGames, C:\AmazonGames |             |
| Automatically optimize newly added games and apps | False                                                                  |             |

<!-- markdownlint-enable MD013 -->

###### Theme

| Key   | Value  | Explanation |
| ----- | ------ | ----------- |
| Theme | System |             |

##### Notifications

###### Notifications

| Key               | Value | Explanation |
| ----------------- | ----- | ----------- |
| Driver updates    | False |             |
| Available rewards | False |             |

##### About

###### Privacy

| Key                                        | Value | Explanation |
| ------------------------------------------ | ----- | ----------- |
| Configuration, performance, and usage data | False |             |

#### NVIDIA overlay

##### Shortcuts

###### General

| Key                            | Value           | Explanation |
| ------------------------------ | --------------- | ----------- |
| Open/close the in-game overlay | Ctrl+Shift+Home |             |
| Toggle microphone on/off       | None            |             |
| Activate push-to-talk          | None            |             |

###### Statistics monitor

| Key                               | Value          | Explanation |
| --------------------------------- | -------------- | ----------- |
| Toggle statistics overlay on/off  | None           |             |
| Cycle through metrics shown       | None           |             |
| Toggle font size                  | None           |             |
| Start/stop logging                | None           |             |
| Reset averages                    | None           |             |
| Toggle record on/off              | None           |             |
| Toggle Instant Replay on/off      | None           |             |
| Save last 20 mins 0 secs recorded | Ctrl+Shift+End |             |

###### Capture

| Key               | Value | Explanation |
| ----------------- | ----- | ----------- |
| Save a screenshot | None  |             |

###### Game filters

| Key                     | Value | Explanation |
| ----------------------- | ----- | ----------- |
| Edit filters            | None  |             |
| Toggle profile 1 on/off | None  |             |
| Toggle profile 2 on/off | None  |             |
| Toggle profile 3 on/off | None  |             |

###### Photo mode

| Key                  | Value | Explanation |
| -------------------- | ----- | ----------- |
| Photograph the scene | None  |             |

##### Heads up display

###### Status indicators

| Key                | Value | Explanation |
| ------------------ | ----- | ----------- |
| Record             | None  |             |
| Instant Replay     | None  |             |
| Highlights         | None  |             |
| Microphone         | None  |             |
| Statistics logging | None  |             |

##### Notifications

| Key                        | Value | Explanation |
| -------------------------- | ----- | ----------- |
| Open/close in-game overlay | False |             |

##### Audio

###### Microphone

<!-- markdownlint-disable MD013 -->

| Key    | Value                                                               | Explanation |
| ------ | ------------------------------------------------------------------- | ----------- |
| Source | SteelSeries Sonar - Stream (SteelSeries Sonar Virtual Audio Device) |             |

<!-- markdownlint-enable MD013 -->

###### Audio tracks

| Key    | Value           | Explanation |
| ------ | --------------- | ----------- |
| Format | Separate tracks |             |

##### Video capture

| Key                   | Value   | Explanation |
| --------------------- | ------- | ----------- |
| Instant Replay length | 20:00   |             |
| Quality               | Custom  |             |
| Resolution            | In-game |             |
| Frame rate            | 120 FPS |             |
| Codec                 | AV1     |             |
| Bit rate (Mbps)       | 230     |             |

### NZXT CAM

```powershell
winget install NZXT.Cam

Add-MpPreference -ExclusionPath "C:\Program Files\NZXT CAM"
Add-MpPreference -ExclusionPath "$env:APPDATA\NZXT CAM"
Add-MpPreference -ExclusionProcess "C:\Program Files\NZXT CAM\NZXT CAM.exe"
```

#### Lighting

| Key      | Value       | Explanation |
| -------- | ----------- | ----------- |
| Lighting | NZXT Purple |             |

#### Settings

##### General

###### General

<!-- markdownlint-disable MD013 -->

| Key                                                        | Value | Explanation |
| ---------------------------------------------------------- | ----- | ----------- |
| Minimize NZXT CAM to tray when closing                     | False |             |
| Start NZXT CAM on Windows startup                          | False |             |
| Start NZXT CAM minimized when launching on Windows startup | False |             |
| Enable Dark Mode                                           | True  |             |

<!-- markdownlint-enable MD013 -->

###### Panels

| Key          | Value | Explanation |
| ------------ | ----- | ----------- |
| Keyboard     | False |             |
| Mouse        | False |             |
| Capture Card | False |             |
| Monitor      | False |             |
| Audio        | False |             |

###### Privacy

<!-- markdownlint-disable MD013 -->

| Key                                                                                                 | Value | Explanation |
| --------------------------------------------------------------------------------------------------- | ----- | ----------- |
| Allow NZXT CAM to collect, report, and analyze information about application performance and usage. | False |             |

<!-- markdownlint-enable MD013 -->

### OBS Studio

```powershell
winget install OBSProject.OBSStudio
```

#### General

##### Updates

| Key                                        | Value | Explanation |
| ------------------------------------------ | ----- | ----------- |
| Automatically check for updates on startup | False |             |

#### Stream

##### Multitrack Video

| Key                          | Value | Explanation |
| ---------------------------- | ----- | ----------- |
| Enable Enhanced Broadcasting | True  |             |

#### Output

##### Streaming

###### Streaming Settings

| Key              | Value              | Explanation |
| ---------------- | ------------------ | ----------- |
| Twitch VOD Track | True, 2            |             |
| Video Encoder    | NVIDIA NVENC H.264 |             |

###### Encoder Settings

<!-- markdownlint-disable MD013 -->

| Key                                   | Value                       | Explanation |
| ------------------------------------- | --------------------------- | ----------- |
| Bitrate                               | 15000 Kbps                  |             |
| Keyframe interval (seconds, 0 = auto) | 2s                          |             |
| Preset                                | P6: Slower (Better Quality) |             |
| Profile                               | main                        |             |
| B-Frames                              | 4                           |             |

<!-- markdownlint-enable MD013 -->

##### Recording

###### Recording Settings

| Key           | Value            | Explanation |
| ------------- | ---------------- | ----------- |
| Video Encoder | NVIDIA NVENC AV1 |             |

###### Encoder Settings

| Key          | Value                       | Explanation |
| ------------ | --------------------------- | ----------- |
| Rate Control | Constant QP                 |             |
| Constant QP  | 15                          |             |
| Preset       | P6: Slower (Better Quality) |             |
| B-Frames     | 4                           |             |

#### Video

<!-- markdownlint-disable MD013 -->

| Key                        | Value                                              | Explanation |
| -------------------------- | -------------------------------------------------- | ----------- |
| Base (Canvas) Resolution   | 2560x1440 (16:9 profile), 3440x1440 (21:9 profile) |             |
| Output (Scaled) Resolution | 2560x1440 (16:9 profile), 3440x1440 (21:9 profile) |             |
| Common FPS Values          | 60                                                 |             |

<!-- markdownlint-enable MD013 -->

### OCCT

```powershell
winget install OCBase.OCCT.Personal
```

#### Settings

##### General

| Key               | Value    | Explanation |
| ----------------- | -------- | ----------- |
| Check for updates | Disabled |             |

### Playnite

```powershell
winget install Playnite.Playnite
```

#### Add-ons

##### Generic

###### Ludusavi

| Key                                                 | Value | Explanation |
| --------------------------------------------------- | ----- | ----------- |
| Also restore save data for a game before playing it | True  |             |
| If not found, retry by normalizing the title        | True  |             |
| Check for Ludusavi updates automatically            | False |             |

#### General

<!-- markdownlint-disable MD013 -->

| Key                                                                    | Value | Explanation |
| ---------------------------------------------------------------------- | ----- | ----------- |
| Minimize Playnite to system tray when the application window is closed | True  |             |

<!-- markdownlint-enable MD013 -->

##### Updating

| Key                       | Value         | Explanation |
| ------------------------- | ------------- | ----------- |
| Update libraries          | Only manually |             |
| Scan emulation folders    | Only manually |             |
| Check for add-on updates  | Only manually |             |
| Check for program updates | Only manually |             |

##### Metadata

###### Web image search

| Key                            | Value                   | Explanation |
| ------------------------------ | ----------------------- | ----------- |
| Icon image search string       | "{Name}" game icon      |             |
| Cover image search string      | "{Name}" game cover     |             |
| Background image search string | "{Name}" game wallpaper |             |

#### Advanced

##### Performance

| Key                    | Value   | Explanation |
| ---------------------- | ------- | ----------- |
| Image rendering scaler | Quality |             |

#### Full-screen Mode

##### Settings

###### General

| Key                    | Value   | Explanation |
| ---------------------- | ------- | ----------- |
| Image rendering scaler | Quality |             |

### RAM Test

Sourced from a private download link from
[Karhu Software](https://www.karhusoftware.com)

### Realtek Ethernet Controller Driver

Sourced from
[Realtek PCIe FE / GbE / 2.5GbE / 5G / 10G Family Controller Software](https://www.realtek.com/Download/List?cate_id=584)

### Razer Synapse

```powershell
winget install RazerInc.RazerInstaller.Synapse4

Add-MpPreference -ExclusionPath "C:\Program Files (x86)\Razer"
Add-MpPreference -ExclusionPath "C:\Program Files\Razer"
Add-MpPreference -ExclusionPath "C:\ProgramData\Razer"
Add-MpPreference -ExclusionPath "$env:LOCALAPPDATA\Razer"
Get-Process |
  Where-Object { $_.Path -like "*Razer*" } |
  Select-Object -ExpandProperty Path -Unique |
  ForEach-Object {
    Add-MpPreference -ExclusionProcess $_
    Write-Host "Excluded: $_" -ForegroundColor Green
  }
```

#### Naga Pro

##### Performance

| Key          | Value | Explanation |
| ------------ | ----- | ----------- |
| Sensitivity  | 1600  |             |
| Polling rate | 1000  |             |

##### Lighting

| Key        | Value  | Explanation |
| ---------- | ------ | ----------- |
| Brightness | 100    |             |
| Effects    | Static |             |
| Color      | Green  |             |

##### Power

| Key                   | Value | Explanation |
| --------------------- | ----- | ----------- |
| Wireless power saving | 15    |             |
| Low power mode        | 5     |             |

##### Calibration

| Key                | Value | Explanation |
| ------------------ | ----- | ----------- |
| Manual Calibration | True  |             |

#### Settings

##### Auto-launch

| Key                                                  | Value | Explanation |
| ---------------------------------------------------- | ----- | ----------- |
| Start Razer Synapse automatically when system starts | False |             |
| Display on-screen notifications                      | False |             |
| Recommendations                                      | False |             |

### Samsung_MonSetup

Sourced from
[C49G93TSSR](https://www.samsung.com/nl/support/model/LC49G93TSSRXEN/#downloads)

### Steam

```powershell
winget install Valve.Steam

Add-MpPreference -ExclusionProcess (${env:ProgramFiles(x86)} + `
  "\Common Files\Steam\SteamService.exe")
```

#### Notifications

##### Client Notifications

| Key                                      | Value | Explanation |
| ---------------------------------------- | ----- | ----------- |
| When I unlock an achievement, show toast | False |             |
| When I unlock an achievement, play sound | False |             |

##### Friend Notifications

| Key                                    | Value | Explanation |
| -------------------------------------- | ----- | ----------- |
| When a friend joins a game, show toast | False |             |

##### Store News

| Key                        | Value | Explanation |
| -------------------------- | ----- | ----------- |
| There's a major sale, Feed | False |             |

#### Interface

<!-- markdownlint-disable MD013 -->

| Key                                                                                   | Value   | Explanation |
| ------------------------------------------------------------------------------------- | ------- | ----------- |
| 24-hour clock                                                                         | True    |             |
| Start Up Location                                                                     | Library |             |
| Run Steam when my computer starts                                                     | False   |             |
| Notify me about additions or changes to my games, new releases, and upcoming releases | False   |             |

<!-- markdownlint-enable MD013 -->

#### Downloads

##### Game Updates

<!-- markdownlint-disable MD013 -->

| Key                                           | Value                      | Explanation |
| --------------------------------------------- | -------------------------- | ----------- |
| Game update timing                            | Only update at game launch |             |
| Allow background processing of Vulkan shaders | True                       |             |

<!-- markdownlint-enable MD013 -->

#### In Game

##### The Steam Overlay

<!-- markdownlint-disable MD013 -->

| Key                                    | Value                  | Explanation |
| -------------------------------------- | ---------------------- | ----------- |
| Enable the Steam Overlay while in-game | True                   |             |
| Overlay shortcut key(s)                | Shift+Ctrl+PgUp        |             |
| Web browser home page                  | <https://www.kagi.com> |             |

<!-- markdownlint-enable MD013 -->

##### Screenshots

| Key               | Value  | Explanation |
| ----------------- | ------ | ----------- |
| Take a screenshot | (null) |             |

#### Controller

| Key             | Value               | Explanation |
| --------------- | ------------------- | ----------- |
| Controller Name | Flydigi VADER 4 Pro |             |

##### Advanced Settings

| Key                     | Value | Explanation |
| ----------------------- | ----- | ----------- |
| Left Joystick Deadzone  | 2000  |             |
| Right Joystick Deadzone | 2000  |             |
| Game Rumble             | True  |             |

#### Voice

| Key                          | Value           | Explanation |
| ---------------------------- | --------------- | ----------- |
| Voice Input Device           | Default         |             |
| Voice Output Device          | Communications  |             |
| Voice Transmission Type      | Open Microphone |             |
| Voice Transmission Threshold | Off             |             |

##### Advanced Settings

| Key                           | Value | Explanation |
| ----------------------------- | ----- | ----------- |
| Echo cancellation             | False |             |
| Noise cancellation            | False |             |
| Automatic volume/gain control | False |             |

#### Remote Play

| Key                | Value | Explanation |
| ------------------ | ----- | ----------- |
| Enable Remote Play | False |             |

#### Broadcast

| Key             | Value                 | Explanation |
| --------------- | --------------------- | ----------- |
| Privacy setting | Broadcasting disabled |             |

#### Music

| Key                               | Value | Explanation |
| --------------------------------- | ----- | ----------- |
| Download high quality audio files | True  |             |

### SteelSeries GG

```powershell
winget install SteelSeries.GG

Add-MpPreference -ExclusionPath "C:\Program Files\SteelSeries"
Add-MpPreference -ExclusionPath "C:\ProgramData\SteelSeries"
Add-MpPreference -ExclusionPath "$env:APPDATA\SteelSeries"
Add-MpPreference -ExclusionProcess ("C:\Program Files\SteelSeries\GG" + `
  "\SteelSeriesGG.exe")
Add-MpPreference -ExclusionProcess ("C:\Program Files\SteelSeries\GG" + `
  "\SteelSeriesGGClient.exe")
```

#### Engine

##### Gear

###### Alias Pro

| Key                        | Value             | Explanation |
| -------------------------- | ----------------- | ----------- |
| Mic Sidetone               | 0                 |             |
| Phantom power              | True              |             |
| Mic gain dial              | True              |             |
| Mic gain dial illumination | 10                |             |
| Ambient LED                | True              |             |
| Dial 2: volume             | Media - Personal  |             |
| Button 2: mute             | Master - Personal |             |

###### Arctis Nova Pro Wireless

| Key                       | Value    | Explanation |
| ------------------------- | -------- | ----------- |
| Mic volume                | 10       |             |
| Gain                      | High     |             |
| Mic sidetone              | Off      |             |
| Power options             | Off      |             |
| Mic muted brightness      | 0        |             |
| Bluetooth default enabled | False    |             |
| OLED screen brightness    | 9        |             |
| OLED dim screen timeout   | 1 Minute |             |
| OLED homescreen mode      | Detailed |             |
| 2.4G mode                 | Speed    |             |

##### Prism

| Key                 | Value             | Explanation |
| ------------------- | ----------------- | ----------- |
| When Monitor Sleeps | Lighting Disabled |             |
| Effects             | Single color      |             |
| Color               | 00FFFF            |             |

#### Sonar

##### Game

| Key           | Value            | Explanation |
| ------------- | ---------------- | ----------- |
| Preset        | Movie: Immersion |             |
| Spatial audio | True             |             |
| Tuning        | Immersion        |             |

##### Chat

| Key    | Value   | Explanation |
| ------ | ------- | ----------- |
| Preset | Clarity |             |

##### Media

| Key           | Value                               | Explanation |
| ------------- | ----------------------------------- | ----------- |
| Preset        | Music: Electronic Dance Music (EDM) |             |
| Spatial audio | True                                |             |
| Tuning        | Immersion                           |             |

##### Aux

| Key    | Value | Explanation |
| ------ | ----- | ----------- |
| Preset | Flat  |             |

##### Mic

| Key                             | Value                | Explanation |
| ------------------------------- | -------------------- | ----------- |
| Preset                          | Alias Pro - Boom Arm |             |
| Clearcast AI noise cancellation | True, 60             |             |
| Compressor                      | True, 0.30           |             |

#### Settings

##### General

| Key             | Value | Explanation |
| --------------- | ----- | ----------- |
| Sonar           | True  |             |
| Auto-Flatten EQ | True  |             |
| Auto-run        | True  |             |

##### Notifications

| Key                                     | Value | Explanation |
| --------------------------------------- | ----- | ----------- |
| Allow desktop notifications from Engine | False |             |

##### Game Detection

| Key                          | Value | Explanation |
| ---------------------------- | ----- | ----------- |
| Automatically scan for games | True  |             |

##### QuickSet - Overlays and Notifications

| Key              | Value | Explanation |
| ---------------- | ----- | ----------- |
| Display Overlays | False |             |

##### QuickSet - Presets

| Key                | Value | Explanation |
| ------------------ | ----- | ----------- |
| Sonar game presets | True  |             |

##### Engine - Overlays and Notifications

| Key              | Value | Explanation |
| ---------------- | ----- | ----------- |
| Display overlays | False |             |

##### Moments - Capture and Sound

<!-- markdownlint-disable MD013 -->

| Key                                                                    | Value | Explanation |
| ---------------------------------------------------------------------- | ----- | ----------- |
| Allow Moments to capture while gaming                                  | False |             |
| Allow Reaction Clipping                                                | False |             |
| Launch Moments and highlight clips after my most recent gaming session | False |             |

<!-- markdownlint-enable MD013 -->

##### Moments - Overlays and Notifications

| Key                   | Value | Explanation |
| --------------------- | ----- | ----------- |
| Display game overlays | False |             |
| Play sounds           | False |             |

##### Sonar - Overlays

| Key              | Value | Explanation |
| ---------------- | ----- | ----------- |
| Display overlays | False |             |

##### About and Privacy

| Key                        | Value | Explanation |
| -------------------------- | ----- | ----------- |
| Beta opt-in                | False |             |
| Use Data to Personalize GG | False |             |

### TestMem5

Sourced from [TestMem5](https://github.com/CoolCmd/TestMem5/releases)

| Key     | Value  | Explanation |
| ------- | ------ | ----------- |
| Use AWE | Always |             |

### Ubisoft Connect

```powershell
winget install Ubisoft.Connect

Add-MpPreference -ExclusionPath "C:\Program Files (x86)\Ubisoft"
Add-MpPreference -ExclusionProcess ("C:\Program Files (x86)\Ubisoft" + `
  "\Ubisoft Game Launcher\UbisoftConnect.exe")
Add-MpPreference -ExclusionProcess ("C:\Program Files (x86)\Ubisoft" + `
  "\Ubisoft Game Launcher\upc.exe")
Add-MpPreference -ExclusionProcess ("C:\Program Files (x86)\Ubisoft" + `
  "\Ubisoft Game Launcher\UplayWebCore.exe")
```

#### General

<!-- markdownlint-disable MD013 -->

| Key                                                                                  | Value | Explanation |
| ------------------------------------------------------------------------------------ | ----- | ----------- |
| Minimize Ubisoft Connect PC to the system tray when the application window is closed | False |             |
| Launch Ubisoft Connect PC when Windows starts                                        | False |             |
| Do not send crash reports                                                            | True  |             |

<!-- markdownlint-enable MD013 -->

#### Interface

| Key                                        | Value | Explanation |
| ------------------------------------------ | ----- | ----------- |
| Enable in-game overlay for supported games | False |             |

#### Downloads

<!-- markdownlint-disable MD013 -->

| Key                                                     | Value | Explanation |
| ------------------------------------------------------- | ----- | ----------- |
| Enable automatic game updates for recently played games | False |             |

<!-- markdownlint-enable MD013 -->

#### Notifications

| Key                               | Value | Explanation |
| --------------------------------- | ----- | ----------- |
| Enable in-game push notifications | False |             |

##### Social

| Key                          | Value | Explanation |
| ---------------------------- | ----- | ----------- |
| When a friend appears online | False |             |

##### Games

| Key   | Value | Explanation |
| ----- | ----- | ----------- |
| Games | False |             |

##### Progression

| Key         | Value | Explanation |
| ----------- | ----- | ----------- |
| Progression | False |             |

#### Other

| Key                       | Value          | Explanation |
| ------------------------- | -------------- | ----------- |
| Capture screenshot hotkey | Ctrl+Shift+F12 |             |

### USB Device Tree Viewer

```powershell
winget install UweSieber.USBTreeView
```

### WindowsMaintenance

Sourced from
[windows-maintenance](https://github.com/pgodschalk/windows-maintenance)

### y-cruncher

Sourced from
[y-cruncher - A Multi-Threaded Pi-Program](https://www.numberworld.org/y-cruncher/)

### ZenTimings

Sourced from [ZenTimings](https://zentimings.com)

<!-- markdownlint-enable MD024 -->
