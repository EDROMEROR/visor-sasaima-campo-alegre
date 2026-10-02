VISOR WEB SASAIMA — Campo Alegre (doble clic, funciona sin internet, todo local)
Actualizado: 2026-10-01 con productos vigentes (DSM/DTM/lindero/curvas/capas).
==============================================================================
- visor_unificado.html ★ (NUEVO, recomendado): UN SOLO VISOR 2D + 3D.
  Botones "3D Terreno" / "2D Mapa" en el mismo archivo, mismas capas y datos.
  3D: malla DSM/DTM 20 cm con ortofoto 5 cm + curvas drapeadas + nubes + cámaras.
  2D: mapa cenital (relieve DSM/DTM a color o hillshade gris + ortofoto stretch
  2-98%) + vectores. Pan/zoom sin rotación, norte arriba. Clic en cono = foto.
- visor.html: orientación (nube dispersa/densa + 97 cámaras + trayectoria).
- visor_terreno.html: ORTOFOTO 5 cm sobre malla DSM/DTM + lindero + cámaras.
- visor_2d.html: MAPA 2D cenital (relieve + hillshade + ortofoto + lindero).

Datos (todos regenerados el 2026-10-01 salvo nubes/orientación):
- DSM: dsm_CampoAlegre.tif (20 cm, 1487.7–1578.6 msnm) | DTM: dtm2_CampoAlegre.tif
  (20 cm, 1486.5–1564.6 msnm). Grilla visor 252×273, alturas relativas a H0=1534.3.
  NOTA: terreno.js ahora guarda 'h' PLANO (antes filas anidadas: la malla 3D vieja
  salía plana; corregido).
- Ortofoto: Ortofoto_CampoAlegre_5cm.tif (5 cm, 6030×6548, stretch 2-98%).
- Lindero CAMPO ALEGRE: 0.2425 ha (2424.95 m²), perímetro 313.64 m, 40 vértices
  (anillo 42 pts únicos + cierre). Altura lindero drapeada del DSM.
- Curvas de nivel 1 m: 81 líneas, cotas 1490–1563 (simplificadas 0.15 m).
- Construcciones 17 · Carreteras 3 · Colindantes 7 · Vértices lindero 40 ·
  Fotocontrol 4 + Puntos base 2 · Cartera estación unificada 129 pts.
- Nube dispersa: 59,181 tie points (coloreados por altura relativa).
- Nube densa RGB: muestra de 350,000 pts (de 41,769,709, calidad ALTA).
  LAS completo: ..\05_PRODUCTOS\03_NUBE_DE_PUNTOS\NUBE_SASAIMA_ALTA.las.
- 97 cámaras orientadas (de 98; DJI_0291 sin orientar) + trayectoria de vuelo.
- Sistema: ENU local en metros (E=E9377-4841844.105, N=N9377-2104376.129,
  z=H-1534.3). Origen: lat 4.943108, lon -74.427002, h 1534.3 (ver datos.js).
  Todo en MAGNA-SIRGAS Origen Nacional EPSG:9377.

Archivos:
- visor_unificado.html + datos.js/datos.json + datos_densa.js + terreno.js +
  vectores.js (NUEVO: lindero/curvas/capas en ENU) + lindero.js + hill_img.js +
  elev_img.js + orto_img.js + *.png + vendor/three.min.js + OrbitControls.js.
- Leyenda de altura del visor unificado en msnm (absolutas).

Fase 2 (cuando entrenes splats en GPU externa): el .ply de gaussianas se integra
en este mismo visor para recorrido fotorrealista.
