<!-- ==================== PROGRAMACIÓN ==================== -->
<h2>Programación (Python)</h2>

<div class="pedagogical-block">
    <span class="level-badge level-resolver">🔴 RESOLVER</span>
    <h3>Manejo de Estructuras y Archivos</h3>

    <div class="pedagogical-step">
        <span class="pedagogical-step-title">1. 🎯 Objetivo:</span> Procesar cadenas de texto o secuencias utilizando estructuras de datos y lectura de archivos.
    </div>

    <div class="pedagogical-step">
        <span class="pedagogical-step-title">2. 🧩 Patrón de código: Frecuencia de elementos</span>
        <div class="code-block"><pre>secuencia = "ATGCGTAC"
conteo = {}
for base in secuencia:
    conteo[base] = conteo.get(base, 0) + 1

print(conteo)  # Muestra: {'A': 2, 'T': 2, 'G': 2, 'C': 2}</pre></div>
    </div>

    <div class="pedagogical-step">
        <span class="pedagogical-step-title">3. 🧩 Lectura segura de archivos:</span>
        <div class="code-block"><pre>with open("datos.csv", "r") as archivo:
    lineas = archivo.readlines()
    for linea in lineas:
        print(linea.strip())</pre></div>
    </div>

    <div class="warning-box">
        <strong>⚠️ Precisión técnica sobre algoritmos:</strong> Ordenar los datos no acelera la búsqueda mágicamente por sí solo; lo que hace es habilitar el uso de métodos de búsqueda mucho más eficientes, como la <em>búsqueda binaria</em> ($O(\log n)$).
    </div>
</div>
