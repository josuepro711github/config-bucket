# config-bucket

# DETALLE PIZZERIA
 create table detalle_pizzeria(
     id_pizza int NOT NULL,
     id_pizzeria int NOT NULL,
      FOREIGN KEY( id_pizzeria ) REFERENCES pizzerias (id_pizzeria )  on delete cascade on update cascade,
     FOREIGN KEY( id_pizza ) REFERENCES pizzas ( id_pizza )  on delete cascade on update cascade
 );
 
 # DETALLE CLIENTES
  create table detalle_clientes(
     id_pizza int NOT NULL,
     id_cliente int NOT NULL,
      FOREIGN KEY( id_cliente ) REFERENCES clientes (id_cliente )  on delete cascade on update cascade,
     FOREIGN KEY( id_pizza ) REFERENCES pizzas ( id_pizza )  on delete cascade on update cascade
 )
 
