# ⚡ QUICK START - Inicio Rápido

## 🎯 3 Opciones para Comenzar

### ✅ Opción 1: Demo Instant (2 segundos)
```bash
# Simplemente abre el archivo
index.html
```
**Resultado:** Verás el mapa completo con 11 pueblos interactivos en tu navegador.

---

### ✅ Opción 2: WordPress/ACF (5 minutos)

**Paso 1:** Copiar archivo PHP
```bash
Copiar: wordpress-acf-integration.php
A: /wp-content/themes/tuTema/inc/
```

**Paso 2:** Incluir en functions.php
```php
// En wp-content/themes/tuTema/functions.php
require_once get_template_directory() . '/inc/wordpress-acf-integration.php';
```

**Paso 3:** Importar campos ACF
1. Ir a **WordPress Dashboard**
2. **ACF → Tools → Import**
3. Seleccionar **acf-config.json**
4. Click **Import ACF JSON**

**Paso 4:** Usar en template
```php
<?php
// En template-homepage.php o donde quieras mostrar el mapa
raiz_nativa_render_mapa_heroes();
?>
```

**Resultado:** El mapa se mostrará en la página con URLs configurables desde ACF.

---

### ✅ Opción 3: Headless CMS (Flexible)
```javascript
// Importar lógica en tu aplicación
// Ajustar URLs y estilos según tu stack
// Los archivos son modular-friendly
```

---

## 📱 Verificación Rápida

### Desktop
1. Abrir `index.html` en navegador
2. Mover mouse sobre marcadores naranjas
3. Tooltip aparece ✅
4. Click abre URL (console.log en demo) ✅

### Mobile
1. Abrir `index.html` en teléfono
2. Toccar marcador
3. Tooltip aparece en tap ✅
4. Tap nuevamente ejecuta acción ✅

### Teclado
1. Presionar `Tab`
2. Focus se mueve a marcadores ✅
3. Presionar `Enter` o `Space`
4. Se ejecuta acción ✅

---

## 🎨 Customización en 1 Minuto

### Cambiar Color Interactivo
En `index.html`, busca:
```css
.marker.interactive .marker-icon {
    background: linear-gradient(135deg, #ff6b35 0%, #f7931e 100%);
}
```
Reemplaza `#ff6b35` y `#f7931e` con tus colores.

### Cambiar URLs
En `index.html`, busca:
```javascript
const pueblos = [
    {
        id: 'mapuche',
        url: '/pueblo/mapuche',  // ← Cambiar aquí
    }
];
```

### Cambiar Tamaño
En `index.html`, busca:
```css
.marker.interactive .marker-icon {
    width: 56px;   /* ← Cambiar tamaño */
    height: 56px;
}
```

---

## 📚 Documentación por Caso de Uso

### "Quiero ver cómo se ve rápido"
→ Abre `index.html` en navegador

### "Quiero integrarlo en WordPress"
→ Lee `GUIA-IMPLEMENTACION.md`

### "Quiero entender la arquitectura"
→ Lee `COMPONENTE-MAPA.md`

### "Quiero customizar los colores"
→ Lee sección "Customización" en `GUIA-IMPLEMENTACION.md`

### "Tengo un error"
→ Lee `GUIA-IMPLEMENTACION.md` sección "Troubleshooting"

### "Quiero probar interactividad"
→ Abre `TESTING.html` en navegador

---

## ✨ Features Principales

```
✅ 11 Pueblos Originarios
✅ 3 Pueblos Interactivos
✅ Completamente Responsivo
✅ Accesible (WCAG AA)
✅ 0 Dependencias Externas
✅ Performance Optimizado
✅ Integración ACF Completa
```

---

## 🔗 Pueblos Interactivos

| Pueblo | URL Default | Cambiar en |
|--------|------------|-----------|
| Mapuche | `/pueblo/mapuche` | ACF o `index.html` |
| Selk'Nam | `/pueblo/selknam` | ACF o `index.html` |
| Rapa Nui | `/pueblo/rapa-nui` | ACF o `index.html` |

---

## 📞 Ayuda Rápida

| Pregunta | Respuesta |
|----------|-----------|
| ¿Cómo veo el mapa? | Abre `index.html` |
| ¿Cómo lo uso en WordPress? | Sigue `GUIA-IMPLEMENTACION.md` |
| ¿Cómo cambio colores? | Edita CSS en `index.html` |
| ¿Es accesible? | Sí, WCAG 2.1 AA |
| ¿Funciona en mobile? | Sí, completamente responsivo |
| ¿Tiene dependencias? | No, 0 dependencias |
| ¿Puedo customizar? | Sí, totalmente modular |

---

## ✅ Checklist de Verificación

- [ ] Abro `index.html` y veo 11 marcadores
- [ ] 3 marcadores son naranjas (interactivos)
- [ ] 8 marcadores son azules (estáticos)
- [ ] Hover muestra tooltip
- [ ] Click en naranja funciona
- [ ] Tab navega entre marcadores
- [ ] Redimensiono ventana → layout adapta
- [ ] Mobile zoom automático
- [ ] Sin errores en console (F12)

---

## 🎯 Próximas Acciones

1. **Ahora:** Abre `index.html` y explora
2. **Luego:** Lee documentación según necesidad
3. **Integra:** Sigue `GUIA-IMPLEMENTACION.md`
4. **Personaliza:** Cambia colores/URLs/tamaños
5. **Deploy:** Sube a producción

---

## 📞 ¿Dudas?

1. **Error/Bug:** Revisar `GUIA-IMPLEMENTACION.md` → Troubleshooting
2. **Cómo instalar:** Revisar `GUIA-IMPLEMENTACION.md` → Instalación
3. **Especificaciones:** Revisar `COMPONENTE-MAPA.md`
4. **Validar:** Abrir `TESTING.html`

---

**¡Listo! Disfruta tu mapa interactivo. 🎉**

*Última actualización: Diciembre 2024*
