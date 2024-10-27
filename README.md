# Arquitectura API REST
## API Bibloteca

### REQUEST
## [GET]https://console.firebase.google.com/negocio/bibloteca

### RESPONSE
    "bibloteca":[

                 "id 1": {
                            "Autor": "John Kennedy Toole",
                            
                            "Categoria": "categorías / 2",
                            
                            "Libro": "La conjura de los necios",
                            
                            "Precio": 14000,
                            
                            "Stock": true
                        },
      
                "id 2": {
                          "Autor": "Cavan Scott",
                          
                          "Categoria": "categorías / 1",
                          
                          "Libro": "Star Wars: Tormenta Creciente",
                          
                          "Precio": 20000,
                          
                          "Stock": true
                        },
      
                "id 3": {
                          "Autor": "Ayanta Barilli",
                          
                          "Categoría": "categorías / 3",
                          
                          "Libro": "Si no amaneciera",
                          
                          "Precio": 12000,
                          
                          "Stock": true
                      },
      
              "id 4": {
                        "Autor": "Felipe Pigna",
                        
                        "Categoria": "categorías / 4",
                        
                        "Libro": "Los Guemes",
                        
                        "Precio": 24000,
                        
                        "Stock": true
                      }

              ]

### REQUEST
## [POST]://console.firebase.google.com/negocio/bibloteca
    header: { 
              "token": "eyJhbGciO" 
            },
      body: {
              "Autor": "Michal Witkowski",
              "Categoria": "categorías / 2",
              "Libro": "el leñador",
              "Precio": 23000,
              "Stock": true
            }
      
### RESPONSE
    header: {
              "token": "eyJhbGciO"
              "status code": 200
            },
      body: {
              "Autor": "Michal Witkowski",
              "Categoria": "categorías / 2",
              "Libro": "el leñador",
              "Precio": 23000,
              "Stock": true
            }
        
### REQUEST
## [PUT]https://console.firebase.google.com/negocio/bibloteca?ID=2

    header: { 
              "token": "eyJhbGciOdfgdfgadasdasdf"
            },

    body: {
            "Autor": "Cavan Scott",
            
            "Categoria": "categorías / 1",
            
            "Libro": "Star Wars: Tormenta Creciente",
            
            "Precio": 30000,
            
            "Stock": true
          }
        
### RESPONSE

    header: { 
              "token": "eyJhbGciOdfgdfgadasdasdf"
              "status code": 200
            },

    body: {
            "Autor": "Cavan Scott",
            
            "Categoria": "categorías / 1",
            
            "Libro": "Star Wars: Tormenta Creciente",
            
            "Precio": 30000,
            
            "Stock": true
          }

### REQUEST
## [DELETE]https://console.firebase.google.com/negocio/bibloteca?ID=3

### RESPONSE

    {
      "message": "El recurso con ID 3 se ha eliminado exitosamente."
    }