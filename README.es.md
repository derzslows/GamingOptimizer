<div align="center">

# 🎮 Gaming Optimizer

[![Version](https://img.shields.io/badge/version-3.0.0-blue.svg)](https://github.com/derzslows/GamingOptimizer/releases/latest)
[![Windows](https://img.shields.io/badge/Windows-10%20%7C%2011%20(x64)-0078D6.svg?logo=windows)](#%EF%B8%8F-requisitos-del-sistema)
[![.NET](https://img.shields.io/badge/.NET%208%20%C2%B7%20WinUI%203-512BD4.svg?logo=dotnet)](#%EF%B8%8F-compilar-desde-el-código)
[![License](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)
[![Languages](https://img.shields.io/badge/i18n-English%20%7C%20Espa%C3%B1ol-orange.svg)](#)

**Un optimizador de Windows potente, moderno y totalmente reversible para gaming, rendimiento, latencia y privacidad.**

[English](README.md) · **Español**

</div>

> **Principio rector:** *todo lo que se desactiva se puede volver a activar.* Cada cambio captura su estado previo y es reversible —incluso tras reiniciar—, respaldado por un diario persistente y un punto de restauración de Windows opcional antes de los lotes.

<div align="center">

![Panel](https://github.com/user-attachments/assets/474d4e81-0031-4a40-8e52-e4c9daf4369e)

</div>

---

## 📋 Tabla de contenidos

- [Descripción](#-descripción)
- [Características](#-características)
- [Capturas](#-capturas)
- [Instalación](#-instalación)
- [Requisitos del sistema](#️-requisitos-del-sistema)
- [Novedades de la 3.0.0](#-novedades-de-la-300)
- [Compilar desde el código](#️-compilar-desde-el-código)
- [Reversibilidad y seguridad](#️-reversibilidad-y-seguridad)
- [Aviso](#️-aviso)
- [Licencia](#-licencia)
- [Autor](#-autor)

---

## 📝 Descripción

**Gaming Optimizer** ayuda a gamers y usuarios avanzados a exprimir Windows. Combina **diagnóstico**, **gestión de controladores**, un amplio catálogo de **optimizaciones reversibles**, **monitorización en tiempo real** y **herramientas de limpieza** en una única interfaz moderna y totalmente responsive —en **español e inglés**.

A diferencia de los "scripts de tweaks" de un solo uso, aquí cada optimización se aplica con un motor reversible: puedes experimentar con confianza y revertir cualquier cambio, individualmente o todos a la vez.

---

## ✨ Características

### 🎛️ Optimizaciones — más de 160, reversibles
Ajustes curados y documentados en **15 categorías**: Gaming, CPU, GPU, Memoria, Almacenamiento, Red, Energía, Latencia/timers, Entrada, Apariencia/DWM, Privacidad/Telemetría, Servicios, Inicio y Sistema. Con búsqueda y filtro, modos **Fácil / Avanzado**, *Aplicar recomendadas* y *Restaurar todo*. Sin *snake‑oil*: solo cambios reales y documentados.

### 📊 Panel
Vista general en tiempo real: nombres y modelos de hardware, todos los discos con su uso, red en vivo, datos de CPU/GPU/RAM, frecuencia base/núcleos/sockets, caché L1/L2/L3, velocidad de RAM/XMP, licencia/activación de Windows, sesiones activas y número de procesos.

### 🧰 Herramientas
- **🆔 Identificación de hardware** — todos los identificadores únicos del equipo en un sitio: BIOS/SMBIOS, placa base, CPU (ProcessorID, microcódigo, caché), GPU, módulos de RAM, discos (serie / ID único / GUID), volúmenes, particiones, monitores (EDID + SHA‑256), MAC/GUID de red, Bluetooth, audio, controladoras USB, TPM, Secure Boot, Product ID de Windows, Machine GUID y SID — con **Copiar informe** en un clic.
- **🧩 Drivers** — detector, inspector y gestor completo de controladores: dispositivos, kernel/servicios y módulos kernel cargados, con info de firma y de terceros, **detección de anomalías** y desinstalación de paquetes de terceros.
- **🖥️ Pantalla** — modelo real del monitor, soporte **HDR**, resolución nativa, escala, frecuencia de refresco, rotación y cambio de pantalla principal, leídos del EDID de cada monitor.
- **⚡ Planes de energía y GPU** — revela/gestiona planes (incl. Rendimiento máximo) y utilidades de GPU/driver.
- **🌐 Red** — monitor de tráfico en tiempo real, **inspector de conexiones por proceso** y herramientas de red (DNS, ping, diagnóstico).
- **🚀 Inicio** — gestiona qué arranca con Windows.

### 🧹 Mantenimiento
- **📦 Apps & Debloat** — instala más de 150 apps curadas vía `winget` (navegadores, gaming, desarrollo, monitorización, seguridad…) con búsqueda y categorías; quita bloatware UWP preinstalado.
- **🧽 Limpieza** — recupera espacio en disco de forma segura.

### 🔒 Módulo Seguridad ↔ Rendimiento *(Avanzado, opt‑in)*
Permite desactivar opcionalmente **VBS**, **Integridad de memoria (HVCI)**, **mitigaciones Spectre/Meltdown**, **Credential Guard** y el **hipervisor** — cada uno con avisos claros y totalmente reversible. Oculto en modo Fácil y con confirmación explícita.

### Además
♻️ Motor totalmente reversible · 🖼️ **UI responsive** moderna (se adapta a ultrawide/alta resolución) · 🌍 Español e inglés · 🔄 Actualizaciones automáticas.

---

## 📸 Capturas

| Panel | Optimizaciones |
|---|---|
| ![Panel](https://github.com/user-attachments/assets/474d4e81-0031-4a40-8e52-e4c9daf4369e) | ![Optimizaciones](https://github.com/user-attachments/assets/db89651e-5563-49b1-9aeb-7388f95f3e1b) |
| **Herramientas de red** | **Instalador de apps** |
| ![Herramientas de red](https://github.com/user-attachments/assets/4f1969de-54ba-4230-9b52-7365fb29059c) | ![Instalador de apps](https://github.com/user-attachments/assets/26254cb3-97bc-41de-b4dd-1fbac9d14e79) |

---

## 📥 Instalación

1. Descarga **`GamingOptimizer-x.y.z.msi`** desde la [última release](https://github.com/derzslows/GamingOptimizer/releases/latest).
2. Ejecuta el instalador (se te pedirá confirmar permisos de administrador).
3. Si ya tienes una versión anterior, se **actualiza automáticamente**.

La app es autónoma: el runtime de .NET va incluido, no hay que instalar nada más.

---

## ⚙️ Requisitos del sistema

| | |
|---|---|
| **SO** | Windows 10 o Windows 11 (64 bits) |
| **Privilegios** | Administrador (la app corre elevada) |
| **Runtime** | Ninguno — incluido en el instalador |

---

## 🚀 Novedades de la 3.0.0

- 🆕 Dos herramientas nuevas: **Identificación de hardware** y gestor de **Drivers**.
- ⚡ Catálogo de optimizaciones casi duplicado (**86 → 166**), más un módulo avanzado **Seguridad ↔ Rendimiento**.
- 🖼️ **UI totalmente responsive** en todas las páginas (reflujo en varias columnas en pantallas anchas).
- 🖥️ **Arreglos de Pantalla** — HDR, resolución nativa y año de fabricación ahora se leen bien del EDID.

<details>
<summary>2.0.0</summary>

- Panel mucho más completo; más optimizaciones de gaming/rendimiento/privacidad.
- Monitor de tráfico de red e inspector de conexiones por proceso.
- Apps & Debloat, Limpieza e Inicio rediseñados.

</details>

---

## 🛠️ Compilar desde el código

**Stack:** WinUI 3 / Windows App SDK 1.8 · .NET 8 · `win-x64` (desempaquetado) · CommunityToolkit.Mvvm · Microsoft.Extensions.Hosting (DI) · WiX Toolset v3 (MSI).

**Requisitos:** [.NET 8 SDK](https://dotnet.microsoft.com/download), la carga *Windows App SDK* y (para el instalador) [WiX Toolset v3](https://wixtoolset.org/).

```powershell
# Compilar (Debug)
dotnet build .\GamingOptimizer.App\GamingOptimizer.App.csproj -c Debug

# Ejecutar (pide UAC — corre elevada)
Start-Process ".\GamingOptimizer.App\bin\Debug\net8.0-windows10.0.19041.0\win-x64\GamingOptimizer.App.exe"

# Tests
dotnet test .\GamingOptimizer.Tests\GamingOptimizer.Tests.csproj
```

Para versionar, publicar y generar el MSI hay una pequeña herramienta con interfaz —**`builder.ps1`**— que sube la versión en todos los sitios, compila la app + el updater (self‑contained), regenera la lista de archivos y produce el instalador (incluida la elección en compilación del agente opcional NG Sentinel: *nunca / opcional / marcado por defecto*).

> ⚠️ Para recompilar el `.exe`, **cierra antes la app** — si está abierta, el código compila pero falla la copia del ejecutable (`MSB3021/3027`).

### Estructura del proyecto

| Proyecto | Rol |
|---|---|
| `GamingOptimizer.App` | UI WinUI 3 (MVVM Toolkit, MS.Extensions.Hosting DI) |
| `GamingOptimizer.Core` | Contratos/abstracciones, enums, `ITweak` / `ISystemChange` |
| `GamingOptimizer.Platform` | Implementaciones Windows: motor, primitivas de cambio, tweaks, GPU/red/energía… |
| `GamingOptimizer.Update` | Updater independiente (descarga la release de GitHub) |
| `GamingOptimizer.Installer` | WiX (MSI) — fuera del `.sln` |
| `GamingOptimizer.Tests` | xUnit (motor + diario + catálogo) |

---

## ♻️ Reversibilidad y seguridad

Las optimizaciones pasan por un motor reversible: `ITweak → ISystemChange → diario persistente`. Cada cambio registra el valor previo antes de aplicarse, así puede revertirse después —incluso entre reinicios—. Los cambios de registro restauran el valor exacto anterior; los de comando/directiva restauran los valores por defecto de Windows. Los lotes pueden crear un **punto de restauración de Windows** antes. **No hay "limpiador" de registro**, y no se tocan Microsoft Defender / BitLocker / los servicios de Windows Update.

---

## ⚠️ Aviso

Esta herramienta modifica ajustes del sistema. Aunque todo cambio es reversible, algunas optimizaciones —en especial las del módulo **Seguridad ↔ Rendimiento**— reducen protecciones o afectan a la estabilidad y están pensadas para equipos personales y de confianza. Úsala bajo tu responsabilidad y crea un punto de restauración antes de aplicar lotes grandes.

---

## 📄 Licencia

Publicado bajo la **licencia MIT** — ver [LICENSE](LICENSE).

---

## 👤 Autor

**derzslows** — [@derzslows](https://github.com/derzslows)

<div align="center">

⭐ *Si este proyecto te resulta útil, ¡considera dejar una estrella!*

Hecho con ❤️ para gamers y usuarios avanzados de Windows.

</div>
