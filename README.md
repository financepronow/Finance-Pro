<div align="center">

<img src="https://img.shields.io/badge/FinancePro-v1.0.0-7C3AED?style=for-the-badge&logo=python&logoColor=white" alt="FinancePro"/>

# 💰 FinancePro

**Control financiero personal completo para Windows**

Gestiona ingresos, metas, deudas, gastos fijos y mucho más — todo local, sin suscripciones, sin cuenta requerida.

[![Descargar](https://img.shields.io/badge/⬇%20Descargar-v1.0.0-%237C3AED?style=for-the-badge)](https://github.com/financepronow/Finance-Pro/releases/download/v1.0.0/FinancePro_Setup_v1.0.0.exe)
[![Ko-fi](https://img.shields.io/badge/☕%20Ko--fi-Apoyar-FF5E5B?style=for-the-badge&logo=ko-fi&logoColor=white)](https://ko-fi.com/setracus)
[![Windows](https://img.shields.io/badge/Windows-10%20%2F%2011-0078D4?style=for-the-badge&logo=windows&logoColor=white)](https://github.com/financepronow/Finance-Pro/releases)
[![Python](https://img.shields.io/badge/Python-3.14-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://python.org)
[![Licencia](https://img.shields.io/badge/Licencia-MIT-10B981?style=for-the-badge)](LICENSE)

</div>

---

## ✨ ¿Qué es FinancePro?

FinancePro es una app de escritorio nativa para Windows que centraliza toda tu vida financiera personal en un solo lugar. Sin Electron, sin navegador embebido — construida en Python puro con CustomTkinter, rápida y ligera.

> **100% local.** Tus datos nunca salen de tu computadora. Sin servidores, sin telemetría, sin suscripción.

---

## 🖥️ Capturas de pantalla

> *Agrega capturas de pantalla de la app aquí*

---

## 🚀 Instalación

### Requisitos
- Windows 10 / 11 (64-bit)
- No requiere Python instalado

### Pasos

1. **Descarga** el instalador desde [Releases](https://github.com/financepronow/Finance-Pro/releases/download/v1.0.0/FinancePro_Setup_v1.0.0.exe)
2. **Ejecuta** `FinancePro_Setup_v1.0.0.exe` — si Windows muestra una advertencia de SmartScreen, haz clic en **"Más información" → "Ejecutar de todas formas"**
3. **Sigue el wizard** — elige si quieres acceso directo en el escritorio
4. **¡Listo!** La app aparece en tu escritorio y menú inicio

Tus datos se guardan en:
```
C:\Users\TuNombre\AppData\Local\FinancePro\
```

---

## 📦 Módulos incluidos

| # | Módulo | Descripción |
|---|--------|-------------|
| 1 | 💰 **Nuevo movimiento** | Registra ingresos y gastos rápidamente con categorías y fechas |
| 2 | 📋 **Historial** | Todos los movimientos con filtros, búsqueda, edición y papelera |
| 3 | 📊 **Distribución** | Gráfico de torta con desglose de gastos por categoría |
| 4 | 📈 **Tendencias** | Evolución mensual de ingresos vs gastos con Matplotlib |
| 5 | 🎯 **Metas** | Metas de ahorro con objetivo, fecha límite y aportes progresivos |
| 6 | 💳 **Deudas** | Seguimiento de deudas, abonos, acreedores y fechas límite |
| 7 | 📆 **Gastos Fijos** | Arriendo, servicios, suscripciones — con proyección mensual automática |
| 8 | 🧾 **Evidencias** | Adjunta imágenes, PDFs o archivos como comprobante de cada pago |
| 9 | 🛡️ **Fondo de emergencia** | Gestiona tu colchón financiero con depósitos, retiros y objetivo |
| 10 | 📐 **Endeudamiento** | Calcula tu capacidad de crédito e indicadores de salud financiera |

---

## ☁️ Respaldo en Google Drive (opcional)

FinancePro permite conectar Google Drive para hacer respaldos automáticos. Esta función es completamente opcional.

**Cómo conectar:**
1. En la app ve a **⚙️ Config → Respaldo → Google Drive** y haz clic en **Conectar con Google**
2. El navegador se abre con la pantalla de inicio de sesión de Google — inicia sesión y otorga el permiso
3. ¡Listo! La sesión se guarda automáticamente

**Seguridad y privacidad:**
- Utiliza **OAuth 2.0** — FinancePro nunca accede a tu contraseña de Google
- El permiso solicitado es el scope restrictivo `drive.file` — la app **solo puede ver archivos que ella misma creó**
- Tus otros archivos en Google Drive **nunca son visibles ni modificados**
- Puedes revocar el acceso en cualquier momento desde [myaccount.google.com/permissions](https://myaccount.google.com/permissions)

---

## 🔧 Stack tecnológico

```
Python 3.14        →  Lenguaje principal
CustomTkinter      →  Interfaz gráfica nativa de Windows
Matplotlib         →  Gráficos y visualizaciones
Pandas             →  Procesamiento de datos
ReportLab          →  Exportación a PDF
OpenPyXL           →  Exportación a Excel (.xlsx)
Google Drive API   →  Respaldo en la nube (OAuth 2.0)
PyInstaller        →  Compilación del ejecutable
Inno Setup         →  Generación del instalador .exe
```

**Formatos de datos soportados:**

`CSV` · `JSON` · `ZIP (backup)` · `XLSX (export)` · `PDF (export)`

---

## 📁 Estructura del proyecto

```
Finance-Pro/
├── main.py                  # Punto de entrada
├── modules/
│   ├── historial.py
│   ├── metas.py
│   ├── deudas.py
│   ├── gastos_fijos.py
│   ├── emergencias.py
│   ├── evidencias.py
│   ├── graficos.py
│   ├── endeudamiento.py
│   └── gdrive.py
├── assets/
│   └── icons/
├── data/                    # Generado en runtime (no en repo)
└── requirements.txt
```

---

## 🛠️ Desarrollo local

Si quieres ejecutar desde el código fuente:

```bash
# 1. Clonar el repositorio
git clone https://github.com/financepronow/Finance-Pro.git
cd Finance-Pro

# 2. Crear entorno virtual
python -m venv venv
venv\Scripts\activate

# 3. Instalar dependencias
pip install -r requirements.txt

# 4. Ejecutar
python main.py
```

---

## 📄 Licencia

Este proyecto está bajo la licencia **MIT**. Consulta el archivo [LICENSE](LICENSE) para más detalles.

---

## ☕ Apoya el proyecto

Si FinancePro te ha sido útil, considera apoyar el desarrollo:

[![Ko-fi](https://img.shields.io/badge/☕%20Ko--fi-ko--fi.com%2Fsetracus-FF5E5B?style=for-the-badge&logo=ko-fi&logoColor=white)](https://ko-fi.com/setracus)

---

## 📬 Contacto

¿Tienes sugerencias, bugs o preguntas?

- 🐛 **Issues:** [github.com/financepronow/Finance-Pro/issues](https://github.com/financepronow/Finance-Pro/issues)
- ☕ **Ko-fi:** [ko-fi.com/setracus](https://ko-fi.com/setracus)
- 🌐 **Web:** [financepronow.github.io/Finance-Pro](https://www.financeproapp.online/)

---

<div align="center">

Hecho con ♥ en Python · by **Setracus**

</div>
