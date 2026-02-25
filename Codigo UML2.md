# 3F261@startuml

class Steve
class Esqueleto
class Zombie
class Creeper
class Araña
class Pico
class Espada
class Hacha
class Madera
class Tierra
class Piedra
class Personaje
class Objeto
class Herramienta
class Diamante 
class Carbon
class Esmeralda
class Redstone
class Hierro
class Mineral
class Pollo
class Vaca
class Cerdo
class Lobo
class Obeja
class Abeja
class Gato
class Animal


Steve *-- Personaje
Zombie *-- Mounstruo
Esqueleto *-- Mounstruo
Araña *-- Mounstruo
Creeper *-- Mounstruo
Tierra *-- Objeto
Piedra *-- Objeto
Madera *-- Objeto
Espada *-- Herramienta
Pico *-- Herramienta
Hacha *-- Herramienta
Redstone *-- Mineral
Diamante *-- Mineral
Hierro *-- Mineral
Carbon *-- Mineral
Esmeralda *-- Mineral
Pollo *-- Animal
Vaca *-- Animal
Cerdo *-- Animal
Lobo *-- Animal
Obeja *-- Animal
Abeja *-- Animal
Gato *-- Animal

Mineral "1" o-- "64" Diamante
Mineral "1" o-- "64" Carbon
Mineral "1" o-- "64" Redstone
Mineral "1" o-- "64" Esmeralda
Mineral "1" o-- "64" Hierro

Animal "1" o-- "*" Pollo
Animal "1" o-- "*" Vaca
Animal "1" o-- "*" Cerdo
Animal "1" o-- "*" Lobo
Animal "1" o-- "*" Obeja
Animal "1" o-- "*" Abeja
Animal "1" o-- "*" Gato

Herramienta "1" o-- "1" Espada
Herramienta "1" o-- "1" Pico
Herramienta "1" o-- "1" Hacha

Mounstruo "1" o-- "1" Zombie
Mounstruo "1" o-- "1" Esqueleto
Mounstruo "1" o-- "1" Creeper
Mounstruo "1" o-- "1" Araña

Personaje "1" o-- "1" Steve


@enduml