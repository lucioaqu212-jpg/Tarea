# Tarea
# Importamos sympy con el nombre corto 'sp'
import sympy as sp

# Creamos la variable simbólica 'x'
x = sp.symbols('x')

# Definimos el numerador y el denominador de la fracción
numerador = 2*x**3 + 2*x**2 + 4*x - 3
denominador = x**4 + x**2

# Construimos la fracción
fraccion = numerador / denominador

# Mostramos la fracción original como lo pidió el profe
print("Esta es la fracción que nos puso el profe:")
sp.pprint(fraccion, use_unicode=True)

# Separamos la fracción en fracciones parciales
resultado = sp.apart(fraccion)

# Mostramos el resultado final
print("\nY así queda ya separada en fracciones parciales:")
sp.pprint(resultado, use_unicode=True)
