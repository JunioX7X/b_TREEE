# 🌳 Árbol B (B-Tree) Implementation

[![Python Version](https://img.shields.io/badge/python-3.6%2B-blue)](https://python.org)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

Una implementación didáctica de un Árbol B en Python con visualización y explicaciones paso a paso.

## 📚 Contenidos
- [Características](#-características)
- [Instalación](#-instalación)
- [Uso](#-uso)
- [Estructura del Código](#-estructura-del-código)
- [Ejemplo](#-ejemplo)
- [Contribuir](#-contribuir)
- [Licencia](#-licencia)

## ✨ Características

✅ Implementación clara del Árbol B con grado configurable (`t`)  
✅ Inserción automática con división de nodos  
✅ Sistema de explicaciones paso a paso  
✅ Visualización por niveles del árbol  
✅ Búsqueda eficiente con complejidad O(log n)  
✅ Documentación detallada en español  

## 🛠️ Instalación

No se requieren dependencias externas. Solo Python 3.6+:

```bash
git clone https://github.com/tu-usuario/arbol-b.git
cd arbol-b

🚀 Uso Básico

from arbol_b import ArbolB

# Crear árbol con grado mínimo t=2 (hasta 3 claves/nodo)
arbol = ArbolB(t=2)

# Insertar datos
claves = [78, 393, 12, 90, 120]
for clave in claves:
    print(f"\nInsertando {clave}:")
    print(arbol.insertar(clave))  # Explicación
    print(arbol.imprimir_arbol()) # Visualización

# Buscar clave
if arbol.buscar(90):
    print("¡90 encontrado!")

🏗️ Estructura del Código
Clases Principales
Clase	Descripción
NodoArbolB	Nodo del árbol (hoja/no-hoja)
ArbolB	Implementación principal con operaciones

📊 Ejemplo Completo

Insertando 120:
- Navegando al hijo apropiado [78, 90, 99] para insertar 120.
- Insertado 120 en nodo hoja en la posición 3.

Nivel 0: [90] 
Nivel 1: [12 78] [99 120]


🎯 Complejidad

Operación	Complejidad

Búsqueda	O(log n)
Inserción	O(log n)
