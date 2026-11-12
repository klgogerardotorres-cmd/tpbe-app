# TPBE App

Webapp de una sola página (`index.html`) para completar el Test de Provocación Bronquial con Ejercicio (TPBE) durante la atención de pacientes pediátricos.

## Qué hace
- Formulario del test: datos del paciente, VEF1 basal, SatO2 y FC, y mediciones a 1, 3, 5, 7, 10, 15, 20 y 30 min más post-β2, con sibilancias y tos por punto.
- Cronómetro desde el fin del ejercicio que indica cuándo medir.
- Cálculo automático de % de caída del VEF1 (gráfico en negativo, umbral -10%), VEF1 teórico GLI 2012 (3 a 25 años) y FC máxima teórica 208 - (0,7 x edad).
- Evolución para ficha clínica generada automáticamente, editable y copiable con un botón.
- PDF descargable: página 1 TPBE, página 2 espirometría (PDF adjunto opcional, arrastrar y soltar).

## Criterio
Positivo: caída del VEF1 >= 10% respecto al basal (ATS 2013, Am J Respir Crit Care Med 187: 1016-27). Los síntomas se registran pero no cambian el resultado. La app no emite conclusión: la interpretación es del médico.

## Privacidad
Los datos viven solo en la pestaña del navegador (sessionStorage) y no se envían a ningún servidor. La espirometría adjunta se procesa en el dispositivo.

## Fuentes
- ATS 2013: Parsons et al., Exercise-induced Bronchoconstriction.
- GLI 2012: Quanjer et al., Eur Respir J 2012; 40: 1324-43. Tablas de FEV1 tomadas de los datos del paquete abierto rspiro.

Librerías cargadas desde cdnjs: jsPDF 2.5.1 y pdf-lib 1.17.1.
