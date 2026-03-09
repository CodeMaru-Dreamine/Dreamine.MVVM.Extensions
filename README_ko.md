
# Dreamine.MVVM.Extensions

Dreamine MVVM 프레임워크에서 사용하는 **유틸리티 확장 패키지**입니다.

이 패키지는 Dreamine MVVM 인프라와 WPF 런타임을 연결할 때 필요한 작은 헬퍼 기능들을 제공합니다.

[➡️ English Version](./README.md)

---

## 목적

`Dreamine.MVVM.Extensions`는 Dreamine MVVM 구성 요소의 동작을 보조하는 유틸리티 클래스를 제공합니다.

핵심 프레임워크 로직과 분리된 **작은 헬퍼 기능들을 모아놓은 패키지**입니다.

---

## 주요 구성 요소

### RegionBinderHelper

Region 기반 네비게이션 시스템에서 사용하는 헬퍼 클래스입니다.

주요 역할:

- Region 바인딩 로직 보조
- 네비게이션 관련 작업 단순화
- WPF Region 인프라 지원

사용 예시:

```csharp
RegionBinderHelper.SomeUtilityMethod();
```

---

## 설계 원칙

이 패키지는 Dreamine 전체에서 사용하는 다음 원칙을 따릅니다.

- 최소 의존성
- 가벼운 유틸리티
- 재사용 가능한 헬퍼 함수
- 핵심 프레임워크와 분리된 구조

Extensions 패키지는 핵심 MVVM 인프라를 깔끔하게 유지하기 위해 별도의 레이어로 분리되어 있습니다.

---

## Dreamine MVVM 구조 내 위치

```
Dreamine.MVVM.Interfaces
        ↑
Dreamine.MVVM.Locators
        ↑
Dreamine.MVVM.Locators.Wpf
        ↑
Dreamine.MVVM.Extensions
```

상위 모듈을 보조하는 유틸리티 레이어 역할을 합니다.

---

## 설치

```bash
dotnet add package Dreamine.MVVM.Extensions
```

또는 프로젝트 파일에 직접 추가합니다.

```xml
<PackageReference Include="Dreamine.MVVM.Extensions" Version="1.0.0" />
```

---

## 요구 사항

- .NET 8.0

---

## License

MIT License
