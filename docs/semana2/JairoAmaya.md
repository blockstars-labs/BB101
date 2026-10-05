# Historias de usuario individuales

**Nombre:** Jairo Enrique Amaya Celis

**Usuario de GitHub:** [@jairoamayac](https://github.com/jairoamayac)

---

<p align="center"><img src="assets/portada-jairo.svg" width="100%" alt="Entregable 2, Diseñar: siete historias de usuario para dos problemas"></p>

Trabajamos con los dos problemas que trajo Emanuel en la semana 1: **liquidar activos sin exponer la operación** y **anticipos de obra sin garantía**. Parecen de mundos distintos, pero tienen el mismo nudo: dos partes que no se tienen confianza y una plata que solo debería moverse cuando cada una cumple lo suyo.

Escribí historias desde los dos lados de cada intercambio y desde quien tiene que vigilar que todo sea limpio.

<p align="center"><img src="assets/hu-mapa.svg" width="100%" alt="En los dos problemas hay dos partes que no confían entre sí y un pago que solo debería moverse cuando se cumple lo acordado"></p>

---

## Mis historias de usuario

1. Como **familia que va a remodelar** quiero **dejar la plata de la obra en una garantía que solo se libera cuando yo apruebe cada etapa** para **no perder el anticipo si el maestro no cumple**.
2. Como **maestro de obra** quiero **ver que la plata del cliente ya está depositada y bloqueada antes de empezar** para **trabajar tranquilo, sabiendo que me van a pagar cada etapa que entregue**.
3. Como **familia o maestro** quiero **que lo que acordamos (etapas, montos, fechas y fotos del avance) quede registrado sin que nadie lo pueda cambiar** para **tener cómo probar lo que pasó si terminamos peleando**.
4. Como **mediador que las dos partes escogieron** quiero **revisar la evidencia de una etapa en disputa y decidir si la plata va para el maestro o vuelve a la familia** para **resolver el conflicto en días y no en años de juicio**.
5. Como **gestor de un fondo que vende facturas o bonos tokenizados** quiero **liquidar la venta en un solo paso, activo contra pago, en segundos y a cualquier hora** para **no depender de la cadena de intermediarios ni esperar días con la plata quieta**.
6. Como **tesorero de una empresa que compra esos activos** quiero **que el precio y el monto de mi operación no queden a la vista del mercado** para **que la competencia no copie mi estrategia ni se adelante a mis movimientos**.
7. Como **auditor o supervisor** quiero **poder ver, con permiso, el detalle de las operaciones confidenciales** para **verificar que todo cumple la norma sin que esa información sea pública**.

### Vistas por problema

| # | Problema | Rol | El riesgo que le quitamos | Criterio de la Sesión 1 |
|:-:|:-:|---|---|---|
| 1 | 🧱 Obra | 🏠 Familia | Perder el anticipo | 🤝 Partes que no confían entre sí |
| 2 | 🧱 Obra | 👷 Maestro | Trabajar semanas y no cobrar | 🤝 Partes que no confían entre sí |
| 3 | 🧱 Obra | 🏠👷 Ambos | Que sea un chat contra otro chat | 🔒 Histórico inalterable |
| 4 | 🧱 Obra | ⚖️ Mediador | Decidir sin pruebas | ✂️ Reemplaza a la fiducia que no está al alcance |
| 5 | 📈 Liquidación | 📈 Fondo vendedor | Días de espera y una comisión por eslabón | ✂️ Un intermediario que concentra la confianza |
| 6 | 📈 Liquidación | 💼 Tesorero comprador | Que el mercado vea su jugada | 🤝 Partes que no confían entre sí |
| 7 | 📈 Liquidación | 🔍 Auditor | Que la privacidad tape el cumplimiento | 🔒 Histórico inalterable |

---

## La más importante y por qué

| Orden de importancia | Historia # | Por qué |
| :---: | :---: | --- |
| 1 (la más importante) | 1 | Es el dolor más concreto y más cercano: familias que pierden millones y luego siguen pagando arriendo. Si la plata queda en garantía y solo sale cuando la familia aprueba, el problema central desaparece. |
| 2 | 2 | Es la otra mitad de la misma garantía. Si el maestro no ve la plata bloqueada antes de empezar, no tiene motivo para aceptar el sistema y no hay producto. |
| 3 | 5 | Es el corazón del problema de liquidación: activo contra pago en un solo paso y sin intermediarios. Va después de la obra porque toca el mercado de valores, que tiene más reglas. |
| 4 | 6 | Sin confidencialidad, un fondo no se mueve a una red pública. Ya existen las piezas en Stellar (tokens confidenciales), pero siguen en etapa de prueba, por eso no va más arriba. |
| 5 | 3 | Es lo que convierte la garantía en prueba. Hace falta, pero se construye casi solo cuando ya existen las historias 1 y 2. |
| 6 | 4 | Las disputas van a pasar, pero no en cada obra. Al principio se pueden resolver con un acuerdo simple antes de tener un flujo de mediación completo. |
| 7 (la menos importante) | 7 | Es clave para salir a producción con fondos regulados, pero en una demostración en testnet no la necesitamos. |

> 🔍 **Lo que todavía tengo que validar:** si un maestro de obra aceptaría cobrar desde una billetera (aunque reciba pesos al final), y si un fondo que hoy liquida con Deceval movería aunque sea una parte de su operación a una red pública con privacidad.
