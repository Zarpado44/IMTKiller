# IMTKiller — Eliminar IMTLazarus de Windows

> **¿Tienes instalado IMTLazarus en tu PC y no sabes cómo quitarlo?**  
> IMTKiller es la herramienta gratuita y open source para eliminarlo completamente.

---

## ¿Qué es IMTLazarus?

IMTLazarus (también conocido como **IMTWin.exe**) es un software de vigilancia y control que:

- Se instala sin consentimiento real del usuario
- **Bloquea el Administrador de tareas** para que no puedas cerrarlo
- **Bloquea el CMD** (símbolo del sistema)
- Instala la extensión **IMTLazarusV3** en Google Chrome sin permiso
- Desactiva el modo incógnito y el modo desarrollador de Chrome
- Aplica políticas de empresa forzadas en el navegador
- Se reinstala solo si intentas borrarlo manualmente
- Se ejecuta en segundo plano como servicio de Windows

---

## ¿Cómo quitar IMTLazarus? — Solución con IMTKiller

IMTKiller elimina IMTLazarus de forma **completamente automática** en pocos segundos.

### Descarga

👉 **[Descargar IMTKiller.exe — Última versión](../../releases/latest)**

### Uso

1. Descarga `IMTKiller.exe`
2. Ejecuta como **Administrador** (clic derecho → Ejecutar como administrador)
3. Selecciona **Opción 1** — Eliminación del Programa
4. Cuando termine, selecciona **Opción 2** — Limpieza de Destrozo
5. Reinicia el PC

---

## ¿Qué elimina IMTKiller?

| Elemento | Descripción |
|---|---|
| `IMTWin.exe` | Proceso principal de vigilancia |
| `C:\IMTWin` | Carpeta de instalación |
| Extensión Chrome | `cgigopjakkeclhggchgnhmpmhghcbnaf` (IMTLazarusV3) |
| Registro `HKLM\SOFTWARE\Google` | Políticas forzadas de Chrome |
| Registro `HKLM\SOFTWARE\Policies\Google` | Control del navegador |
| Registro `HKCU\SOFTWARE\Google\Chrome` | Configuración bloqueada |
| `DisableTaskMgr` | Restaura el Administrador de tareas |
| `DisableCMD` | Restaura el CMD |
| Servicio de Windows | Elimina el servicio que relanza el proceso |
| Archivos temporales | Limpia restos en `C:\Windows\Temp` |

---

## Menú del programa

```
  [1]  Eliminacion del Programa     ← mata IMTWin.exe y borra C:\IMTWin
  [2]  Limpieza de Destrozo         ← limpia registro, Chrome, servicios
  [3]  Creditos
  [4]  Buscar Actualizaciones
  [5]  Salir
```

---

## Preguntas frecuentes

**¿Es seguro usarlo?**  
Sí. El código fuente es público y está disponible en este repositorio para que cualquiera lo revise.

**¿Necesito desinstalar Chrome?**  
No. IMTKiller limpia las políticas y extensiones forzadas sin tocar tu Chrome ni tus datos.

**¿Funciona en Windows 10 y 11?**  
Sí, compatible con Windows 10 y Windows 11 (64 bits).

**¿Tengo que reinstalar Windows?**  
No. IMTKiller limpia todo sin necesidad de formatear.

**¿Por qué vuelve a aparecer IMTWin.exe?**  
Porque IMTLazarus tiene un proceso vigilante que lo relanza. La Opción 1 lo mata continuamente hasta que confirma que no vuelve.

---

## Compilar desde el código fuente

```bash
# Requiere MinGW-w64
gcc -O2 -o IMTKiller.exe IMTKiller.c IMTKiller.rc -lpsapi -lshell32 -lwininet -ladvapi32 -lshlwapi
```

---

## Palabras clave

`IMTLazarus` · `IMTWin.exe` · `quitar IMTLazarus` · `desinstalar IMTLazarus` · 
`eliminar IMTLazarus Windows` · `IMTLazarus no se puede desinstalar` · 
`IMTWin proceso segundo plano` · `IMTLazarusV3 extension Chrome` · 
`bloquea administrador de tareas` · `software vigilancia Windows eliminar`

---

## Licencia

MIT License — Copyright (c) 2025 Zarpado44  
Código libre para usar, modificar y distribuir. El crédito al autor original debe mantenerse.
