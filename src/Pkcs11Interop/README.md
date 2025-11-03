# Pkcs11Interop

Managed .NET wrapper for unmanaged PKCS#11 libraries.

- Target Framework: `net10.0`
- NativeAOT: AOT-friendly delegate marshalling and generic `Marshal` APIs.
- Trimming: Library marked `IsTrimmable=true`.

## Install

```
PM> Install-Package Pkcs11Interop
```

## Features

- Low‑level and high‑level PKCS#11 APIs
- Cross‑platform dynamic loading (`dlopen`/`LoadLibraryEx`)
- Strongly-typed mechanism parameter helpers

## NativeAOT

Consuming app publish example:

```
dotnet publish -c Release -r win-x64 -p:PublishAot=true
```

Linux/macOS için: `-r linux-x64` veya `-r osx-x64`.

## Links

- Project: https://www.pkcs11interop.net/
- Repo: https://github.com/Pkcs11Interop/Pkcs11Interop
