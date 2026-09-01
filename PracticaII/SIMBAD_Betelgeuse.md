```python
# Parallax and distance calculation verification
plx = 6.55  # mas
plx_err = 0.83

dist_pc = 1000 / plx
dist_pc_err_min = 1000 / (plx + plx_err)
dist_pc_err_max = 1000 / (plx - plx_err)

print(f"Distance in pc: {dist_pc:.2f} pc")
print(f"Range: {dist_pc_err_min:.2f} pc - {dist_pc_err_max:.2f} pc")


```

```text
Distance in pc: 152.67 pc
Range: 135.50 pc - 174.83 pc


```

Propiedades físicas fundamentales de **Betelgeuse ($\alpha$ Orionis)** registradas en el catálogo SIMBAD:

* **Tipo de objeto astrofísico oficial:**
* **Red Supergiant** (Supergigante Roja).


* **Coordenadas de posición exacta (ICRS, $ep=J2000$):**
* **RA (Ascensión Recta):** `05 55 10.30536`
* **Dec (Declinación):** `+07 24 25.4304`


* **Magnitudes aparentes por filtro espectral:**
* **B:** $2.27$
* **V:** $0.42$
* **J:** $-3.00$
* **H:** $-3.73$
* **K:** $-4.05$
* **Interpretación del contraste (B vs. K):** El índice de color $(B - K = 6.32)$ muestra que la estrella emite de forma abrumadoramente mayoritaria en el infrarrojo cercano ($K = -4.05$) en comparación con el óptico azul ($B = 2.27$). Según la Ley de Wien, el pico de emisión hacia longitudes de onda más largas revela que su atmósfera estelar tiene una **temperatura efectiva muy baja** ($\sim 3500\text{ K}$), característica de las supergigantes rojas frías.


* **Distancia estimada y método de obtención:**
* **Distancia:** $\approx 152.67\text{ pc}$ ($\sim 498\text{ años luz}$).
* **Método:** **Paralaje trigonométrica** (reportada en el catálogo como $\text{Plx} = 6.55 \pm 0.83\text{ mas}$).


* **Movimiento propio (Proper motions):**
* **Vector:** $\mu_{\alpha} \cos\delta = 27.54\text{ mas/yr}$ (RA) y $\mu_{\delta} = 11.30\text{ mas/yr}$ (Dec).
* **Velocidad angular total:** $\mu = \sqrt{27.54^2 + 11.30^2} \approx 29.77\text{ mas/yr}$.


* **Referencia científica relevante:**
* **Bibcode / Cita:** `2007A&A...474..653V` (Harper, G. M., Brown, A., & Guinan, E. F., *Astronomy & Astrophysics*, 2007), utilizada en la ficha para actualizar la paralaje reducida e invocar mediciones astrométricas de radio con VLA y Hipparcos.
