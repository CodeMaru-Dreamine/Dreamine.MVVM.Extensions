
# Dreamine.MVVM.Extensions

Utility extensions for the Dreamine MVVM framework.

This package provides helper utilities that simplify integration between the Dreamine MVVM infrastructure and WPF runtime components.

[➡️ 한국어 문서 보기](./README_ko.md)

---

## Purpose

`Dreamine.MVVM.Extensions` contains small but useful helper classes that extend the behavior of the core Dreamine MVVM components.

These utilities are intentionally lightweight and independent so they can be reused across different Dreamine modules.

---

## Key Components

### RegionBinderHelper

Helper utilities used by region navigation systems.

Responsibilities include:

- assisting region binding logic
- simplifying navigation-related operations
- supporting WPF region infrastructure

Typical usage:

```csharp
RegionBinderHelper.SomeUtilityMethod();
```

---

## Design Goals

This package follows several principles used across Dreamine:

- minimal dependencies
- lightweight utilities
- reusable helper functions
- separation from core framework logic

Extensions are placed in a separate package so the core MVVM infrastructure remains clean and focused.

---

## Architecture Role

Within the Dreamine MVVM ecosystem this package belongs to the **Utility Layer**.

```
Dreamine.MVVM.Interfaces
        ↑
Dreamine.MVVM.Locators
        ↑
Dreamine.MVVM.Locators.Wpf
        ↑
Dreamine.MVVM.Extensions
```

It provides supporting helpers used by higher-level modules.

---

## Installation

```bash
dotnet add package Dreamine.MVVM.Extensions
```

Or add to the project file:

```xml
<PackageReference Include="Dreamine.MVVM.Extensions" Version="1.0.0" />
```

---

## Requirements

- .NET 8.0

---

## License

MIT License
