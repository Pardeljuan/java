package carritotp5;

class Producto {
	String prodNombre;
	int prodCantidad;
	double prodPrecio;
	
	public Producto(String prodNombre, int prodCantidad, double prodPrecio) {
		this.prodNombre = prodNombre;
		this.prodCantidad = prodCantidad;
		this.prodPrecio = prodPrecio;
	}
}

class itemCarrito extends Producto{
	 double itemPrecioTotal;
	 
	 public itemCarrito(String prodNombre, int prodCantidad, double prodPrecio, double itemPrecTotal ){
		 
		 super(prodNombre, prodCantidad, prodPrecio);
		 this.itemPrecioTotal = itemPrecTotal;
	 }
}

class Descuento extends itemCarrito {
	 double descuento;
	 
	 public Descuento(String prodNombre, int prodCantidad, double prodPrecio, double itemPrecTotal, double descuento) {
		 super(prodNombre,prodCantidad,prodPrecio,itemPrecTotal);
		 this.descuento = descuento;
	 }
}
