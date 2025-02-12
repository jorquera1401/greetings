# Saludos en go

Este paquete proporciona una forma simple de obtener saludos personalizados en GO

### Instalacion
Ejecuta el siguiente comando para instalar el paquete:
```bash
go get -u github.com/jorquera1401/greetings
```

## Uso 
Aqui tiens un ejemplo de como utilizar el paquete en tu codigo:

```go
package main

import (
	"fmt"
	"log"

	"github.com/jorquera1401/greetings"
)

func main() {
	log.SetPrefix("greetings: ")

	names := []string{"Alex", "Jorge", "Juan"}
	messages, err := greetings.Hellos(names)
	if err != nil {
		log.Fatal(err)
	}
	fmt.Println(messages)
}

```

