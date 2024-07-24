# Modelo De Campuslands

Este proyecto en Python simula una estructura básica para gestionar campers (estudiantes), trainers (instructores) y cursos dentro de una universidad ficticia.

## Clases

### Camper

La clase `Camper` representa a los estudiantes de la universidad.

- **Atributos**:
  - `nombre`: Nombre del camper.
  - `edad`: Edad del camper.
  - `cursos_inscritos`: Lista de cursos en los que el camper está inscrito.

- **Métodos**:
  - `inscribir_curso(curso)`: Permite al camper inscribirse en un curso específico.
  - `mostrar_informacion()`: Muestra la información básica del camper.

### Trainer

La clase `Trainer` representa a los instructores de la universidad.

- **Atributos**:
  - `nombre`: Nombre del trainer.
  - `especialidad`: Área de especialización del trainer.
  - `cursos_impartidos`: Lista de cursos que el trainer está encargado de impartir.

- **Métodos**:
  - `asignar_curso(curso)`: Asigna un curso al trainer para que lo imparta.
  - `mostrar_informacion()`: Muestra la información básica del trainer.

### Curso

La clase `Curso` representa los cursos ofrecidos por la universidad.

- **Atributos**:
  - `nombre`: Nombre del curso.
  - `descripcion`: Descripción breve del curso.

## Ejemplo de Uso

```python
# Ejemplo de uso del código
camper1 = Camper("Juan", 20)
camper2 = Camper("Maria", 22)

trainer1 = Trainer("Pedro", "Programación")
trainer2 = Trainer("Ana", "Matemáticas")

curso1 = Curso("Introducción a Python", "Curso introductorio de programación en Python")
curso2 = Curso("Cálculo I", "Curso de cálculo diferencial e integral")

# Inscribir campers en cursos
camper1.inscribir_curso(curso1)
camper2.inscribir_curso(curso2)

# Asignar trainers a cursos
trainer1.asignar_curso(curso1)
trainer2.asignar_curso(curso2)

# Mostrar información
camper1.mostrar_informacion()
trainer1.mostrar_informacion()
