# 🚨 PASOS EXACTOS PARA RESTAURAR TU PORTAFOLIO

## PROBLEMA: Sitio web CAÍDO 
Tu https://portafolio-c14.pages.dev/ muestra página en blanco

## SOLUCIÓN: Subir archivos a GitHub (2 minutos)

---

## MÉTODO 1: GitHub Web Interface (MÁS FÁCIL)

### Paso 1: Ir a tu repositorio
1. Abre tu navegador
2. Ve a: `https://github.com/kafe1994/Portafolio`
3. Inicia sesión en GitHub si es necesario

### Paso 2: Subir archivos
1. En la página del repositorio, haz clic en "uploading an existing file"
2. O simplemente arrastra los archivos desde la carpeta `cloudflare-pages`
3. **IMPORTANTE**: Necesitas subir TODOS estos archivos:
   ```
   ✅ index.html
   ✅ favicon.svg  
   ✅ INSTRUCCIONES.md
   ✅ RESUMEN_EMERGENCIA.md
   ✅ assets/images/profile-photo.svg
   ✅ assets/images/skills/react.png
   ✅ assets/images/skills/javascript.png
   ✅ assets/images/skills/typescript.png
   ✅ assets/images/skills/css.png
   ✅ assets/images/skills/html.png
   ✅ assets/images/skills/python.png
   ✅ assets/images/skills/nodejs.png
   ✅ assets/images/skills/security.png
   ✅ assets/images/skills/design.png
   ✅ assets/images/skills/github.png
   ```

### Paso 3: Confirmar cambios
1. En "Commit message" escribe: `Emergency restore: portfolio restoration`
2. Haz clic en "Commit changes"
3. **¡Listo!** Tu sitio estará online en 1-2 minutos

---

## MÉTODO 2: Git Command Line

```bash
# 1. Clonar repositorio
git clone https://github.com/kafe1994/Portafolio.git
cd Portafolio

# 2. Copiar todos los archivos de cloudflare-pages aquí
# (Haz esto manualmente copiando cada archivo)

# 3. Subir cambios
git add .
git commit -m "Emergency restore: portfolio restoration"
git push origin main
```

---

## ✅ VERIFICACIÓN
Después de subir los archivos:
1. ✅ Ve a https://portafolio-c14.pages.dev/
2. ✅ Debe cargar tu portafolio completo
3. ✅ Los iconos de skills deben ser visibles
4. ✅ Debe funcionar el cambio de idioma (ES/EN)

## 🆘 SI ALGO SALE MAL
- WhatsApp: +54 3572 408 928
- Tiempo estimado: 2-5 minutos total

---
**URGENCIA**: Hazlo AHORA, tu sitio está caído